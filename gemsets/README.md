
# Gems
http://guides.rubygems.org/

### What are RubyGems?

The RubyGems software allows you to easily download, install, and use ruby software packages on your system. The software package is called a "gem" and contains a package Ruby application or library.

Gems can be used to extend or modify functionality in Ruby applications. Commonly they're used to distribute reusable functionality that is shared with other Rubyists for use in their applications and libraries. Some gems provide command line utilities to help automate tasks and speed up your work.

Ruby 1.9 and newer ships with RubyGems built-in, so you can just use the gem command anywhere.

### Rubygems

There are almost one hundred thousand gems available for you to use in your ruby programs. Luckily for you, most of these gems are already indexed thanks to the guys at [RubyGems](https://rubygems.org/).

```
#gem help search

Usage: gem search [STRING] [options]

  Options:
    -i, --[no-]installed             Check for installed gem
    -I                               Equivalent to --no-installed
    -d, --[no-]details               Display detailed information of gem(s)
        --[no-]versions              Display only gem names
    -a, --all                        Display all gem versions

  Local/Remote Options:
    -l, --local                      Restrict operations to the LOCAL domain
    -r, --remote                     Restrict operations to the REMOTE domain
    -b, --both                       Allow LOCAL and REMOTE operations

  Common Options:
    -h, --help                       Get help on this command

  Arguments:
    STRING        fragment of gem name to search for

  Summary:
    Display remote gems whose name contains STRING

  Description:
    The search command displays remote gems whose name contains the given string.

    The --details option displays additional details from the gem but will take a little longer to complete as it must download the information  individually from the index.

    To list local gems use the list command.

  Defaults:
    --remote --no-details
```

RubyGems is the _de facto_ master repository of all gems.

### Ruby-toolbox

As the number of gems grew exponentially in the past, other sites like [Ruby Toolbox](https://www.ruby-toolbox.com) help you find gems in a different way in categories and see how active they are in github, open issues, etc.

[Ruby Toolbox Categories](https://www.ruby-toolbox.com/categories/by_group)
```
Active Record Plugins
Background Processing
Code Quality
Communication
Content Management & Blogging
CSS
Data Persistence
Developer Tools
Documentation Tools
Documents & Reports
E-Commerce and Payments
Fun
Graphics
HTML & Markup
JavaScript
Maintenance & Monitoring
Package & Dependency Management
Provision, Deploy & Host
Rails Plugins
Security
Testing
Time & Space
Web Apps, Services & Interaction
```

### Installing gems
```
gem install <GEM_NAME>
```

### Listing installed gems
```
gem list
```

https://www.ruby-lang.org/en/libraries/

# Gemsets

RVM gives you compartmentalized independent ruby setups. This means that ruby, gems and irb are all separate and self-contained - from the system, and from each other.

You may even have separate named gemsets, which will allow you to manage a set of gems for each application, avoiding potencial conflicts and

Let's say, for example, that you are testing two versions of a gem, with ruby 2.1.1. You can install one to the default 2.1.1, then create a named gemset for the other version, and switch between them easily.

```
$ rvm gemset create gemset_name    # create a gemset
$ rvm ruby_version@gemset_name  # specify Ruby version and our new gemset
```
- rvm gemset list
- rvm gemset create
- rvm gemset use
- rvm gemset delete

http://rvm.io/gemsets
https://wiki.archlinux.org/index.php/RVM
