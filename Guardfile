# A sample Guardfile
# More info at https://github.com/guard/guard#readme

guard 'rspec', {
      cmd: 'bundle exec rspec',
      cmd_additional_args: '--colour',
      focus: true,
      all_on_start: false,
      all_after_pass: false,
      failed_mode: :none } do
  watch(%r{^spec/.+_spec\.rb$})
  watch(%r{^lib/(.+)\.rb$})     { |m| "spec/lib/#{m[1]}_spec.rb" }
  watch('spec/spec_helper.rb')  { "spec" }
end

