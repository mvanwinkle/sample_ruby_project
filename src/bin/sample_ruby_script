#!/usr/bin/ruby

realbin=__FILE__
if File.lstat(realbin).symlink?
	realbin=File.readlink(__FILE__)
end

$:.unshift('/opt/company/lib/ruby2')
$:.unshift(File.expand_path('../lib/ruby2/',File.dirname(realbin)))

require 'hello_ruby/hello_repo_layout'

app = HelloRuby::HelloRepoLayout.new

app.hello()
