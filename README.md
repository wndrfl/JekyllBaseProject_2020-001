[![Vincent V. Toscano](http://vflux.biz/assets/imgs/global/VincentVToscanoTM2015_300x300.png)](http://vflux.biz)

# JekyllBaseProject_2020-001

Static website that can be used as a scafoldding for marketing, trailer, or other static website needs. This project utilizes [Jekyll](https://jekyllrb.com) to generate pages based on layouts and layout partials. Additionally, it processes your SCSS files.

## Install
#### Requirments:
- GNU/Linu, Unix, or macOS  
- Ruby version 2.6.5 >  
- RubyGems  
- GCC & Make  

##### * On macOS, install install ***rbenv*** Ruby version manager to upgrade your version of Ruby. Once installed check the version with:
``brew doctor``  
If brew doctor comes up with any issues, fix them first.

Upgrade Ruby [do not use brew to install Ruby – use rbenv instead]  
``brew update && brew upgrade``  
``brew install rbenv ruby-build``  
``echo 'if which rbenv > /dev/null; then eval "$(rbenv init -)"; fi' >> ~/.bash_profile``

Add PATH (may not be needed so check path first with ``echo $PATH``):  
``export PATH="~/.rbenv/shims:$PATH"``

First, find the desired version:  
``rbenv install -l``  

Install that version (e.g. 2.6.5):  
``rbenv install 2.6.5``  

Then set the global version to the desired Ruby version:  
``rbenv global 2.6.5``  

At this point you should see the desired version set with the following command:  
``rbenv versions``  
Expected output:  
>system  
  \* 2.6.5 (set by /Users/USERNAME/.rbenv/version)

### Install Jekyll (>= 3.8.5) and Bundler through RubyGems (Perform only once, not every project).
``gem install bundler``  
``cd /YOUR_PATH_TO_REPO/``  
``bundle install``

#### Check install
``
jekyll --version && bundler --version  
``  
* Alternatively you may use bundler to check where all Gems are installed:  
``bundle info bundler``  
``bundle info jekyll``  
In the event one of the two cannot be found when typing --verion, but you can see it's been installed with the bundle command – restart the computer and try checking the version number again.

## Build
### Build only:
```
JEKYLL_ENV=prod bundle exec jekyll build  
JEKYLL_ENV=stage bundle exec jekyll build  
JEKYLL_ENV=dev bundle exec jekyll build

```  

### Build & serve the website locally on the preview server with environment:
```
JEKYLL_ENV=prod bundle exec jekyll serve  
JEKYLL_ENV=stage bundle exec jekyll serve  
JEKYLL_ENV=dev bundle exec jekyll serve
```

#### Browse current build (after you have run ``bundle exec jekyll serve`` ): 
- [http://localhost:4000](http://localhost:4000) or  
- [http://127.0.0.1:4000](http://127.0.0.1:4000)

## Documentation
- [Jekyll](https://jekyllrb.com)  
- [Jekyll Forums](http://talk.jekyllrb.com)  
- [Liquid template engine](http://shopify.github.io/liquid/)
- [Bundler](http://bundler.io)  
- [Bundler - Updating Gems](http://bundler.io/v1.12/updating_gems.html)  

## Deploy & Test
Continuous integration and continuous delivery (CI/CD) pipeline has yet to be established.  

The URLs are ready. 
### On ***dev*** branch
TBD

### On ***stage*** branch
TBD

### On ***master*** branch
TBD

