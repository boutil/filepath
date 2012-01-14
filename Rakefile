# This is free and unencumbered software released into the public domain.
# See the `UNLICENSE` file or <http://unlicense.org/> for more details.

begin
	require 'bones'
rescue LoadError
	abort '### Please install the "bones" gem ###'
end

Bones {
	name     'filepath'
	authors  'Gioele Barabucci'
	email    'gioele@svario.it'
	url      'http://github.com/gioele/filepath'

	ignore_file  '.gitignore'
}

require File.join(File.dirname(__FILE__), 'spec/tasks')

task :default => 'spec:run'
task 'gem:release' => 'spec:run'

task 'spec:run' => 'spec:fixtures:gen'
