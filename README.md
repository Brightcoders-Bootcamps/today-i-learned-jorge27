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

## Week 2

### Mon 27, July 2020 *[How works the controllers?]*
Rais is a MVC framework, which means that is composed by three principles elements, Models, Views and Controllers. Today i read about controllers, how create them.
When framework is used, we create some files for use like the controllers,we dont know if the files create affect how framework works. For this purpose, some frameworks have integrated tools for created yours elements.
Rails Generator create many elements, like models, assets and controllers, in this case, I will generate a controller. How I'm using `bundle gem`, when I want to generate a controller, after opening the working directory in the console, i execute
```sh
$ bundle exec rails generate controller Test
```
After this, the console show a list with the files created and modified, like see in the next image

![MYFIRSTCONTROLLER](img/myfirstcontroller.png)

In addition to our controller, also are create a view folder in `app/views/test`, a test file in `test/controllers/test_controller_test.rb`, a sass file in `app/assets/stylesheets/test.scss`, and an helper class in `app/helpers/test_helper.rb`. This extra files I will explain them in a future.
When our controller are created, our file is in `app/controllers` named `test_controller.rb` looks like:

```sh
1   class TestController < ApplicationController
2   end
3   
```
And it's done our controller are created. But for now, it does nothing. we will continue working with this file, in a future entrances.
