# Ruby Koans

A [kōan](http://en.wikipedia.org/wiki/K%C5%8Dan) (_公案 /ˈkoʊ.ɑːn/_) is a story, dialogue, question, or statement, which is used in Zen practice to provoke the **great doubt** and test a student's progress in Zen practice.


## Ruby Koans

### What are Ruby Koans

The Ruby Koans walk you along the path to enlightenment in order to learn Ruby. The goal is to learn the Ruby language, syntax, structure, and some common functions and libraries.

We also teach you culture by basing the koans on tests. Testing is not just something we pay lip service to, but something we live. Testing is essential in your quest to learn and do great things in Ruby.

### The Structure

The koans are broken out into areas by file, hashes are covered in +about_hashes.rb+,modules are introduced in +about_modules.rb+, <em>etc</em>.  They are presented in order in the +path_to_enlightenment.rb+ file.

Each koan builds up your knowledge of Ruby and builds upon itself. It will stop atthe first place you need to correct.

Some koans simply need to have the correct answer substituted for an incorrect one. Some, however, require you to supply your own answer.

(HINT) **If you see the method +__+ (a double underscore) listed, it is a hint to you to supply your own code in order to make it work correctly.**

## Get Started

### Fork the repository

Go to the [wdi rubyKoans](https://github.com/wdi-hk-sep-2014/ruby_koans) repository  and [git fork it](https://help.github.com/articles/fork-a-repo) into your personal github account by clicking on the fork button right.

  You should have something like this:
  ```
  https://github.com/__YourGithubUser__/ruby_koans
  ```

### Clone the repository

[Git Clone](http://git-scm.com/docs/git-clone) your repository to your laptop, so you can start working on it locally

  ```
  git clone git@github.com:__YourGithubUser__/ruby_koans.git
  ```

  _Tip:_ In UNIX systems (including Linux and MacOS) you can get help on most of the available console commands by using the ["man"](http://www.linfo.org/man.html) command (ie. "man top"). To read about git subcommands (clone, push, add), you'll have to type "man git-clone" or "man git-add"

### Let's get started

A fresh checkout of the koans repository will not include your personal koans, you will need to generate them by running

```
$ rake gen
mkdir -p koans
cp src/neo.rb koans/neo.rb
cp README.rdoc koans/README.rdoc
```

and we can also re-generate them (will loose all your progress!) with:

```
$ rake regen
```

### Red, Green, Refactor

In test-driven development the mantra has always been **red, green, refactor**:
* Write a failing test and run it (**red**),
* Make the test pass (**green**)
* Look at the code and consider if you can make it any better (**refactor**).

While walking the path to Ruby enlightenment you will need to run the koan and see it fail (**red**), make the test pass (<em>green</em>), then take a moment and reflect upon the test to see what it is teaching you and improve the code to better communicate its intent (<em>refactor</em>).

### You have not yet reached enlightenment

The very first time you run the koans you will see the following output:

```
$ cd koans
$ ruby path_to_enlightenment.rb
AboutAsserts#test_assert_truth has damaged your karma.

The Master says:
  You have not yet reached enlightenment.

The answers you seek...
  Failed assertion.

Please meditate on the following code:
  /Users/___/ruby_koans/koans/about_asserts.rb:10:in `test_assert_truth'

mountains are merely mountains
your path thus far [X_________________________________________________] 0/282
```

You have come to your first stage. Notice it is telling you where to look for the first solution:

```
    Please meditate on the following code:

    ./about_asserts.rb:10:in `test_assert_truth'

    path_to_enlightenment.rb:38:in `each_with_index'
    path_to_enlightenment.rb:38
```

### Expand your awereness

Open the +about_asserts.rb+ file and look at the first test:

```
    # We shall contemplate truth by testing reality, via asserts.
    def test_assert_truth
      assert false                # This should be true
    end
```

Change the +false+ to +true+ and re-run the test.  After you are
done, think about what you are learning.  In this case, ignore everything except the method name (+test_assert_truth+) and the parts inside the method (everything before the +end+).

In this case the goal is for you to see that if you pass a value to the +assert+ method, it will either ensure it is +true+ and continue on, or fail if the statement is +false+.

```
AboutAsserts#test_assert_truth has expanded your awareness.
AboutAsserts#test_assert_with_message has damaged your karma.

The Master says:
  You have not yet reached enlightenment.
  You are progressing. Excellent. 1 completed.

The answers you seek...
  This should be true -- Please fix this

Please meditate on the following code:
  /Users/fer/Sites/GA/ruby_koans/koans/about_asserts.rb:16:in `test_assert_with_message'

learn the rules so you know how to break them properly
your path thus far [.X________________________________________________] 1/282
```
Now start your advendure.... Happy Hunting!

## Resources

- [Ruby core language reference](http://www.ruby-doc.org/core-2.1.3/)
- [Ruby 2.1.3 Standard Library Documentation](http://www.ruby-doc.org/stdlib-2.1.3/) defines
- [RubySpec](http://rubyspec.org/overview/)
- https://www.ruby-lang.org/en/documentation/
