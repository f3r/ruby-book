# RVM

## RVM structure

RVM is a command-line tool which allows you to easily install, manage, and work with multiple ruby environments from interpreters to sets of gems.

RVM can be installed system-wide _-for all users-_ or for a single-user by default. We recommend to install it for your current user. It will be installed in your $HOME directory, by default under the ~/.rvm/ directory.

## Installing RVM

```
$ \curl -sSL https://get.rvm.io | bash -s stable
```

You will be prompted for your regular user's password as part of the installation procedure and then source the rvm scripts by typing:

```
$ source ~/.rvm/scripts/rvm
```


#### How does the RVM install script work?

For those of you who want to understand what's going on here one level deeper, we can briefly go over exactly what's happening here:

  ```
  $ \Curl -sSL URL
  ```

  - The \curl portion uses the [curl](http://curl.haxx.se/docs/manpage.html) web grabbing utility to grab a script file from the rvm website. Basically, a program that is going to run in our computer to install rvm for us.
  - The backslash that leads the command ensures that we are using the regular curl command and not any altered, aliased version.
  - The -s flag indicates that the utility should operate in silent mode.
  - The -S flag overrides some of this to allow curl to output errors if it fails.
  - The -L flag tells the utility to follow redirects.

[Note] you can also curl any website to see the html code -sort of like a browser will do in the real world. For example, we can get the code of the GA public website by running:

  ```
  $ \curl -i https://generalAssemb.ly
  ```

We have actually 2 commands (curl, and bash), connected with a [UNIX pipe](http://en.wikipedia.org/wiki/Pipeline_(Unix)  The pipe symbol: "|". Pipes allows us to connect the output _(like console.log)_ of a program, with the input of another program.

In this case, the result of "curl" (the installation script) is then piped directly to bash for processing.
  - The -s flag indicates that the input is coming from standard in.
  - We then specify that we want the latest stable version of rvm

And we should be now ready to install ruby...


