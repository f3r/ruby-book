#Ruby

## Ruby Implementations

- Explain difference between Ruby Core Language and it's various implementations
- Understand the pros and cons of each alternative

http://rvm.io/rubies

### Ruby Lang references

- [Ruby core language reference](http://www.ruby-doc.org/core-2.1.3/)
- [Ruby 2.1.3 Standard Library Documentation](http://www.ruby-doc.org/stdlib-2.1.3/) defines
- [RubySpec](http://rubyspec.org/overview/) is a project to write an executable specification for the Ruby Programming Language that is compatible with [RSpec](http://rspec.info/).

You can see a full list of all the implementations available with rvm using:

```
$ rvm list known
```

Ruby -or MRI ([Matz's Ruby Interpreter](http://en.wikipedia.org/wiki/Ruby_MRI)) ruby- is a series of ruby interpreters. This is the original, canonical implementation of Ruby from which the standards (ruby-spec) are being extracted.

[Rubinius (rbx)](http://rubini.us/) ([Github](https://github.com/rubinius/)) is an implementation of Ruby designed for concurrency using native threads to run Ruby code on all the CPU cores. Rubinius includes a bytecode virtual machine, Ruby syntax parser, bytecode compiler, generational garbage collector, just-in-time (JIT) native machine code compiler, and Ruby Core and Standard libraries, which are built using Ruby, making a smaller, consistent system that's easier for Ruby programmers to understand and modify.

[JRuby](http://jruby.org/) ([Github](https://github.com/jruby/jruby/wiki)) is a Java implementation of the Ruby programming language atop the [Java Virtual Machine](http://en.wikipedia.org/wiki/Java_virtual_machine) (JVM), which provides High performance, Real threading and a Vast array of libraries. For the very curious, here is a list of differences between [MRI and JRuby](https://github.com/jruby/jruby/wiki/DifferencesBetweenMriAndJruby).

[MacRuby](http://rvm.io/interpreters/macruby) ([Github](https://github.com/MacRuby/MacRuby/blob/master/README.rdoc)) is an implementation of Ruby 1.9 directly on top of Mac OS X core technologies such as the Objective-C runtime and garbage collector, the LLVM compiler infrastructure and the Foundation and ICU frameworks. It is the goal of MacRuby to enable the creation of full-fledged Mac OS X applications which do not sacrifice performance in order to enjoy the benefits of using Ruby.

[RubyMotion](http://www.rubymotion.com/) implements the Ruby language on top of the core technologies that power iOS, Android and OS X.
RubyMotion apps are also statically compiled into optimized machine code using an ahead-of-time compiler. Code is never interpreted.

[IronRuby](http://ironruby.net/) is an open-source implementation of the Ruby programming language which is tightly integrated with the .NET Framework. IronRuby can use the .NET Framework and Ruby libraries, and other .NET languages can use Ruby code just as easily.


[RubyEnterpriseEdition](http://www.rubyenterpriseedition.com/documentation.html#_overview_of_ruby_enterprise_edition_ree) (REE) is a server-oriented distribution of the official Ruby interpreter, and includes various additional enhancements to increase security and scalability.

## Using RVM to manage rubies

To see all the different ruby implementations that you have installed in your computer, you can use [rvm list](http://rvm.io/rubies/list):

```
$ rvm list [default]

   jruby-1.7.16 [ x86_64 ]
   ruby-2.1.0   [ x86_64 ]
=* ruby-2.1.2   [ x86_64 ]

# => - current
# =* - current && default
#  * - default
```

To install a new implementation or version of ruby

```
$ rvm install [ruby-]version

Examples
rvm install 2.1.0         ==> defaults to MRI ruby
rvm install jruby-1.7.16  ==> install
rvm install jruby         ==>
```

To switch to have a different implementation _(and have it as default)_

```
$ rvm use 2.1.0 --default
```

And of course, we can check that ruby is working and which version by running:

```
$ ruby --version

ruby 2.1.2p95 (2014-05-08 revision 45877) [x86_64-darwin13.0]
```
