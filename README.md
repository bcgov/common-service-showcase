# Common-Service-Showcase
Website for user documentation and marketing of the common services built by the Common Service Showcase Team

## Build with Jekyll
1. Install a full Ruby development environment (2.6 works).
For Windows users, visit https://rubyinstaller.org/downloads/ and download latest version WITH Devkit option. Install the installer (when prompted, just tap enter to use defaults - may happen twice)

1. Install Jekyll and bundler gems.
Open a console window with directory at root of this repo and run:
    ```
    gem install bundler
    gem install jekyll
    bundle install
    ```
1. Build and serve site (locally)
    ```
    bundle exec jekyll build
    bundle exec jekyll serve
    ```

1. Go to site: http://localhost:4000/common-service-showcase

### Add Content
Look under _cards.  _Cards is a collection that is iterated over and used to build the single page site.  See index.md for how the collection is rendered.