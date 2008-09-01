require 'rubygems'
require 'rake'
require 'rake/gempackagetask'


gem_spec = Gem::Specification.new do |gem|
			gem.name = "Zliby"
			gem.version = "0.0.5"
			gem.author = "Michael Letterle"
			gem.email = "theprokrammer@prokrams.com"
			gem.homepage = "http://zliby.rubyforge.org/"
			gem.platform = Gem::Platform::RUBY
			gem.summary = "Compression Library In Pure Ruby"
			gem.rubyforge_project = "zliby"
			gem.files = FileList["{bin,lib}/**/*"].to_a
			gem.require_path = "lib"
			gem.test_files = FileList["{specs}/**/*spec.rb"].to_a
			gem.has_rdoc = true
			gem.extra_rdoc_files = ["README", "CHANGES", "LICENSE", "TODO"]
		end
	
	Rake::GemPackageTask.new(gem_spec) do |package|
		package.need_tar = true
		package.need_zip = true
	end

task :doc do
	sh 'rdoc README TODO CHANGES lib/zliby.rb --template jamis --title "Zliby -- All Zlib, Pure Ruby" --inline-source -U'
end

	