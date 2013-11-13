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
