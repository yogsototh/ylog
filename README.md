> This project has two homes.
> It is ok to work in github, still, for a better decentralized web
> please consider contributing (issues, PR, etc...) throught:
>
> https://gitlab.esy.fun/yogsototh/ylog

---


# `ylog`

`ylog` is a simple command line note taking tool.

Example:

~~~
> cd project
> ylog init # <-- create a log file (.log)
> cd subdir/of/project
> ylog It took me very long to verify the file foo.hs
> ylog todo rename foo.hs to bar.hs
> cd ../../../another/subdir
> ylog There is another foo.hs here
> ylog show
[13-11-2013] (subdir/of/project) It took me very long to verify the file foo.hs
[13-11-2013] (subdir/of/project) [ ] rename foo.hs to bar.hs
[13-11-2013] (another/subdir) There is another foo.hs here
> ylog edit <-- manually edit the file ; use EDITOR environment variable
~~~

Of course you could always add aliases to make it easier to use:

~~~
> alias n=ylog
> alias t="ylog todo"
~~~

## Install

~~~
git clone https://github.com/yogsototh/ylog.git
~~~

Then copy the `ylog` file into one of the directory of your $PATH.
To get the list simply type:

~~~
> echo $PATH | sed 's/:/\n/g'
~~~

It uses zsh which is pretty common in UNIX world.
