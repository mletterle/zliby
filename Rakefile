require 'rubygems'
require 'rake'
task :doc do
	if File.exists? "doc" then 	sh 'rm -r doc' end
	sh 'rdoc README zliby.rb --template jamis --title "Zliby -- All Zlib, Pure Ruby" --inline-source'
end