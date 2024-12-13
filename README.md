# lukebogner.github.io


## One-time Setup

These instructions tested on MacOS Sequoia 15.1.1

1. (optionally) Fix XCode after MacOS 15.x install.  This needs to be done before installing Ruby.

	```
	sudo xcode-select -s /Applications/Xcode.app/Contents/Developer
	sudo xcodebuild -license
	```

1. Install chruby and ruby-install

	```
	brew install chruby ruby-install
	```

1. Install the latest version of Ruby supported by Jekyll

	```
	ruby-install ruby 3.3.5

1. Add the following to ~/.zshrc

	```
	# Set up ruby
	source $(brew --prefix)/opt/chruby/share/chruby/chruby.sh
	source $(brew --prefix)/opt/chruby/share/chruby/auto.sh
	chruby ruby-3.3.5
	````

1. Install bundler and jekyll

	```
	gem install bundler jekyll
	bundle install
	```

## Running the site locally

	```
	bundle exec jekyll serve
	```
