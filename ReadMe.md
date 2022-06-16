# Some helpful Comments

## Fork it! 

Personal website is a great way to showcase your interests, work, and your creativity, all in one place. 
To do so for yourself is fairly simply. Use this jekyll-based template-cum-website as a starting point for your own website and host it on GitHub pages for free. 

You might find the following steps helpful to fork this repo and start adding your stuff to it.

## Necessary installations

1. Installing brew - brew comes handy to install packages in MacOS. Use it to install a bunch of following packges.
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

2. Installing Ruby - chruby is light-weight a version-management package for Ruby. ruby-install allows you to compile and install different versions of Ruby. Finally we use ruby-install to install the latest version of Ruby. 
Installing chruby, ruby-install and ruby
brew install chruby ruby-install
ruby-install ruby  

3. Next, configure your shell to automatically use chruby. This allows the system to use the version of Ruby currently hosted by chruby.
echo "source $(brew --prefix)/opt/chruby/share/chruby/chruby.sh" >> ~/.zshrc
echo "source $(brew --prefix)/opt/chruby/share/chruby/auto.sh" >> ~/.zshrc
echo "chruby ruby-3.1.2" >> ~/.zshrc

4. Install Jekyll and Bundler gems
gem install jekyll
gem install jekyll bundler add webrick  

## Forking 

1. Fork this repository

2. Initialize bundle within the local directory. Then, use bundle to host the website on a local server, so that you can see how it looks while your work on it.
bundle init
bundle exec jekyll serve --livereload

Finally, add your work to the website, commit and push it to your public repository named <your-git-username>.github.io, and GitHub will automatically pick your code to host the website on https://<your-git-username>.github.io.


### Voila! You have your website! 


