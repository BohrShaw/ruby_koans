# A sample Guardfile
# More info at https://github.com/guard/guard#readme

#notification :tmux,
  #:display_message => true,
  #:timeout => 5, # in seconds
  #:default_message_format => '%s >> %s',
  ## the first %s will show the title, the second the message
  ## Alternately you can also configure *success_message_format*,
  ## *pending_message_format*, *failed_message_format*
  #:line_separator => ' > ', # since we are single line we need a separator
  #:color_location => 'status-left-bg' # to customize which tmux element will change color

guard 'shell' do
  #watch(/(.*).txt/) {|m| `tail #{m[0]}` }
  watch(%r{koans/.*\.rb$}) { `rake` }
end
