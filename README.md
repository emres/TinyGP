# TinyGP
This is the Java source code of TinyGP, the genetic programming
software as described in "[A Field Guide to Genetic
Programming]([url](http://www.gp-field-guide.org.uk/)http://www.gp-field-guide.org.uk/)"
(ISBN 978-1-4092-0073-4) by Riccardo Poli, Bill Langdon, Nic McPhee, published
in March, 2008 (See also its [Amazon.com
page]([url](https://www.amazon.com/Field-Guide-Genetic-Programming/dp/1409200736))).

There are few differences from the published paperback version, because a few
bugs had been reported. The authors of the book described those bugs and their
fixes in the following blog posts:

* [Bug in TinyGP Java Code]([url](http://www.gp-field-guide.org.uk/2008/05/bug-in-tinygp-java-code.html))
* [A (potential) bug in TinyGP]([url](http://www.gp-field-guide.org.uk/2008/11/potential-bug-in-tinygp.html))
* [Another Bug Fixed in TinyGP]([url](http://www.gp-field-guide.org.uk/2009/01/another-bug-fixed-in-tinygp.html))

As described in the book, you can compile TinyGP from the operating system's
shell, using the following Java compiler command:

```
javac -O tiny_gp.java
```

As described in the book, if the dataset is stored in a file `problem.dat`, the
program can be launched with the following command:

```
java tiny_gp
```

Otherwise, the user can specify a different datafile on the command line, by
giving the command

```
java tiny_gp FILE
```

where FILE is the dataset file name (which can include the full path to the
file). Finally, the user can specify both the datafile and a seed for the random
number generator on the command line, by giving the command:

```
java tiny_gp SEED FILE
```

where SEED is an integer.

For convenience, the example data file is incuded in this repository as
`problem.dat`. This file's contents are identical to `sin-data.txt`.

The source code and data file URLs as given in the published version are broken
at the time of this writing (25 January, 2024) but they are reachable on
Internet Archive Wayback Machine:

* [TinyGP (also known as Tiny GP) - A Tiny Genetic Programming Implementation (as seen on 6 October 2009)]([url](https://web.archive.org/web/20091006123714/http://cswww.essex.ac.uk/staff/rpoli/TinyGP/)https://web.archive.org/web/20091006123714/http://cswww.essex.ac.uk/staff/rpoli/TinyGP/)

Nevertheless, I wanted to have a copy of them in my personal GitHub repository,
so that I can refer to them later, and maybe even create a modern Java version
of the source code by refactoring this original.
