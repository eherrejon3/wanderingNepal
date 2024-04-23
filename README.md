# wanderingNepal

This is my travel blog. I write here about places I visit, to share with friends and family.


## Building Site
* If using Ubuntu, run the following to install [prerequisites](https://jekyllrb.com/docs/installation/ubuntu/) for Jekyll site.
    ```
    sudo apt-get install ruby-full build-essential zlib1g-dev
    ```
* Avoid installing RubyGems packages (called gems) as the root user. Instead, set up a gem installation directory for your user account. The following commands will add environment variables to your ~/.bashrc file to configure the gem installation path:
  ```
    echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
    echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
    echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
    source ~/.bashrc
  ```
* If **error installeing bundler**: 
  ```
    gem install sass-embedded -v 1.54
    gem install bundler -v 2.4.22
    gem install jekyll
  ```
* Else, install Jekyll and Bundler:
    ```
    gem install jekyll bundler
    ```
* Compile site:
    ```
    bundle install
    ```
  * If GemNotFound: Could not find liquid-4.0.3.gem for installation
    ```
    gem install liquid -v 4.0.3
    ```
* [Build local version of site](https://jekyllrb.com/docs/):
    ```
    bundle exec jekyll serve
    ```
    * click on **server address** on terminal