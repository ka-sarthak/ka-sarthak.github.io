# Personal website

Hi there. This repo contains the templates and content powering my personal website at
[ka-sarthak.github.io](https://ka-sarthak.github.io/).

It is build using [Jekyll](https://jekyllrb.com/) and hosted on GitHub pages.

## Feeling inspired?
You might find the following steps helpful to fork this repo and start adding your stuff 
to it. Much of these steps are inspired from 
<a href="https://jekyllrb.com/docs/" target="_blank">here</a>.

### Necessary installations for macOS 

1. Installing Brew - ```brew``` comes handy to install packages in MacOS. Use it to 
install a bunch of following packges.

```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

2. Installing Ruby - ```chruby``` is light-weight a version-management package for Ruby.
```ruby-install``` allows you to compile and install different versions of Ruby. Finally
we use ```ruby-install``` to install the latest version of Ruby. 

```
brew install chruby ruby-install
ruby-install ruby  
```

3. Next, configure your shell to automatically use ```chruby```.


```
echo "source $(brew --prefix)/opt/chruby/share/chruby/chruby.sh" >> ~/.zshrc
echo "source $(brew --prefix)/opt/chruby/share/chruby/auto.sh" >> ~/.zshrc
echo "chruby ruby-3.1.2" >> ~/.zshrc
```

4. Install the following Ruby gems.

```
gem install jekyll
gem install jekyll bundler add webrick  
```

### Fork it

1. Fork this repository (helpful 
<a href="https://docs.github.com/en/github-ae@latest/get-started/quickstart/fork-a-repo" target="_blank">link</a>)

2. Initialize bundle within the local directory. Then, use bundle to host the website on
a local server, so that you can see how it looks while your work on it.

```
bundle init
bundle exec jekyll serve --livereload
```

Finally, add your work to the website, commit and push it to your public repository 
named <br>```<<your-git-username>>.github.io```, and GitHub will automatically pick 
your code to host the website on <br>```https://<<your-git-username>>.github.io```.


### Voila! You have your website!
