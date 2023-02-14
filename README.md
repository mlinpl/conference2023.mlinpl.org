# conference2023.mlinpl.org

## Quick-start - running this repo locally

### Install deps

On Ubuntu:
```
sudo apt install ruby-full build-essential zlib1g-dev
sudo gem install jekyll bundler
```

On Mac:
```
brew install chruby ruby-install xz
ruby-install ruby
echo "source $(brew --prefix)/opt/chruby/share/chruby/chruby.sh" >> ~/.zshrc
echo "source $(brew --prefix)/opt/chruby/share/chruby/auto.sh" >> ~/.zshrc
echo "chruby ruby" >> ~/.zshrc
source ~/.zshrc # or restart your session
gem install jekyll bundler
```

Then:
```
bundle install
```

On Windows:

1. Install RubyInstaller with DevKit from https://rubyinstaller.org/. Follow the step-by-step instructions and install the default components.
2. Open a command prompt or PowerShell window and navigate to the project directory.
3. Install the required version of bundler and dependencies by running the following commands:
```
gem install jekyll
gem install bundler -v '2.4.5'
bundle _2.4.5_ install
```
> Note: By default, `bundle install` may try to run a `bundle.js` file in your root directory. If this happens, you may want to move this file temporarily. 


### Run server with livereload
After bundler has finished installing the required gems, you can start the Jekyll server by running:
```
bundle exec jekyll serve --livereload
```
This should start the server and make your website available at http://localhost:4000.