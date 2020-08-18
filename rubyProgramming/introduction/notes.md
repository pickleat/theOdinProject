# Introduction Notes

## [Preparations of Launch](https://launchschool.com/books/ruby/read/preparations#usingacodeeditor) School’s *Introduction to Programming with Ruby*

- They are hardcore about 2 spaces for indentation
- `#` is how they leave comments
- filenames, variables, and methods should be named with "snake case" e.g. `this_is_the_name_of_the_file.rb`
- constands are named with ALLCAPS `VARIABLENAME = 'this will never change'`
- multiline `do/end` blocks only use `{  }` when the entire expression fits on one line. 

``` rb
# multi-line
[1, 2, 3,].each do |i|
  # do stuff
end

# one line
[1, 2, 3].each { |i| do_some_stuff }

```

- classes are named with "CamelCase" e.g. 

``` rb
class MyFirstClass
# what it does
end
```

- more style rules: [https://github.com/bbatsov/ruby-style-guide](Ruby Style Guide)
- In the documentation methods are listed out with either a `::` or a `#`
  - `::` are *class methods*
  - `#` are *instance methods*
  - Small gotcha: these are completely different from how these symbols are used in Ruby code, so don't worry about them too much.
- Ruby has a built in interactive environment called "irb" much like `node` or `python`
- if you type `irb` to start it, then `puts 'hello andy'` it will return something like: 

``` 
hello andy
  =>
irb: 001 >
```

- type `exit` or ctrl+d to get out of the irb
- if you have a ruby file you want to run type `ruby file_name.rb` and it will run whatever is in that file.

### Gems

- [rubygems.org](RubyGems) seems to operate similarly to NPM.
- to install a gem type `gem install <gem name>`
- a `gemfile` is a solution to organizing gems and their dependencies, like a `package.json`

### Debugging with Pry

- Pry is a library that is similar to irb, but offers more features.
- Specifically Pry is useful for debugging.
