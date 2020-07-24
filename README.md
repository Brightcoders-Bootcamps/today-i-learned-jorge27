# Today I Learned by *Jorge Garcia*

[This Github Page is here](https://jorge27.github.io)

Ruby and Rails official documentation reading personal journal

## Week 1

### Thu 23, July 2020 *[Get started with ruby]*
Today, I read about how to install rails, the classic "Get started", it's really easy!, after I read it, I installed it by my own, I did two practices, using bundler and rails gem

***By Bunder***

First, create my `Gemfile` with
```sh
$ bundle init 
```
After this, a `Gemfile` is regularly created with the next lines
```sh
1   # frozen_string_literal: true
2
3   source "https://rubygems.com"
4   
5   git_source(:github) { |repo_name| "https://github.com/#{repo_name}" }   
6   
7   # gem "rails"
...
```
I only uncomment the line `7` and run

```sh
$ bundle install
```
After this, ruby downloaded many gems, but rails was not install yet. To finish I executed
```sh
$ bundle exec rails new .
```
And it's done, rails created some files, those files are the skeleton for our app

***By rails***

For install by gem `rails`, I only executed
```sh
$ rails new app
```
And create the files in the folder `app`