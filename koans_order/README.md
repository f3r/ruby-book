# Automating Tests

[Watchr](https://github.com/mynyml/watchr) is an [agile development](http://en.wikipedia.org/wiki/Agile_software_development) tool that monitors a directory tree, and triggers a user defined action whenever an observed file is modified. Its most typical use is continuous testing, and as such it is a more flexible alternative to [autotest](https://github.com/autotest/autotest) -which is used to test the linux kernel.

To install it just run:

```
$ gem install watchr

Fetching: watchr-0.7.gem (100%)
Successfully installed watchr-0.7
Parsing documentation for watchr-0.7
Installing ri documentation for watchr-0.7
Done installing documentation for watchr after 0 seconds
1 gem installed
```

The best way get an application to suscribe to change notifications in a filesystem is [fsevents](http://en.wikipedia.org/wiki/FSEvents) for MacOS and [libenv](http://software.schmorp.de/pkg/libev.html) for linux

```
MacOS  $ gem install ruby-fsevent
Linux: $ gem install rev
```

```
$ watchr karma
```


## Koans count
- about_array_assignment.rb: 8 exercises
- about_arrays.rb: 8 exercises
- about_asserts.rb: 5 exercises
- about_blocks.rb: 9 exercises
- about_class_methods.rb: 16 exercises
- about_classes.rb: 16 exercises
- about_constants.rb: 7 exercises
- about_control_statements.rb: 15 exercises
- about_dice_project.rb: 5 exercises
- about_exceptions.rb: 5 exercises
- about_hashes.rb: 12 exercises
- about_inheritance.rb: 7 exercises
- about_iteration.rb: 9 exercises
- about_java_interop.rb: 14 exercises
- about_keyword_arguments.rb: 2 exercises
- about_message_passing.rb: 13 exercises
- about_methods.rb: 14 exercises
- about_modules.rb: 5 exercises
- about_nil.rb: 3 exercises
- about_objects.rb: 7 exercises
- about_open_classes.rb: 3 exercises
- about_proxy_object_project.rb: 11 exercises
- about_regular_expressions.rb: 27 exercises
- about_sandwich_code.rb: 5 exercises
- about_scope.rb: 9 exercises
- about_scoring_project.rb: 8 exercises
- about_strings.rb: 28 exercises
- about_symbols.rb: 13 exercises
- about_to_str.rb: 5 exercises
- about_triangle_project.rb: 3 exercises
- about_triangle_project_2.rb: 1 exercises
- about_true_and_false.rb: 4 exercises
- neo.rb: 3 exercises

## Koans for WDI Class
#### Fundamentals
- about_asserts.rb
- about_true_and_false.rb
- about_nil.rb
- about_objects.rb
- about_strings.rb
- about_symbols.rb
- about_constants.rb

#### Data Structures and functions
- about_arrays.rb
- about_array_assignment.rb
- about_hashes.rb
- about_methods.rb
- about_keyword_arguments.rb
- about_control_statements.rb
- about_iteration.rb

#### Classes & Modules
- about_classes.rb
- about_open_classes.rb
- about_inheritance.rb
- about_modules.rb
- about_scope.rb
- about_class_methods.rb

#### Skiping until the end
- about_regular_expressions.rb
- about_exceptions.rb
- about_triangle_project_2.rb
- about_blocks.rb
- about_sandwich_code.rb
- about_triangle_project.rb
- about_scoring_project.rb
- about_dice_project.rb
- about_message_passing.rb
- about_proxy_object_project.rb
- about_to_str.rb
- about_extra_credit.rb
