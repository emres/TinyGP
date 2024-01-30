# TinyGP

This is the Java source code of [TinyGP](https://github.com/emres/TinyGP), the
genetic programming software as described in "[A Field Guide to Genetic
Programming](http://www.gp-field-guide.org.uk/)" (ISBN 978-1-4092-0073-4) by
Riccardo Poli, Bill Langdon, Nic McPhee, published in March, 2008 (See also its
[Amazon.com
page](https://www.amazon.com/Field-Guide-Genetic-Programming/dp/1409200736)). You
can also read [my Goodreads
review](https://www.goodreads.com/review/show/6166473293).

The code is copied from the book, and I kept the formatting preferred by the
authors intact. Any errors and bugs that might arise because of this copying
process is solely my responsibility and should not be attributed to the authors.

There are few differences between the version in this repository and the one in
the published paperback version, because apparently a few bugs had been reported
after the book's publication. The authors described those bugs and their fixes
in the following blog posts:

* [Bug in TinyGP Java Code](http://www.gp-field-guide.org.uk/2008/05/bug-in-tinygp-java-code.html)
* [A (potential) bug in TinyGP](http://www.gp-field-guide.org.uk/2008/11/potential-bug-in-tinygp.html)
* [Another Bug Fixed in TinyGP](http://www.gp-field-guide.org.uk/2009/01/another-bug-fixed-in-tinygp.html)

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
`problem.dat`. It is identical to `sin-data.txt`.

The URLs for source code and data file in the published version are broken at
the time of this writing (25 January, 2024) but they are reachable on Internet
Archive Wayback Machine:

* [TinyGP (also known as Tiny GP) - A Tiny Genetic Programming Implementation (as seen on 6 October 2009)](https://web.archive.org/web/20091006123714/http://cswww.essex.ac.uk/staff/rpoli/TinyGP/)

Nevertheless, I wanted to have a copy of them in my personal GitHub repository,
so that I can refer to them later. I also created a modern Java version of the
source code by refactoring this original: https://github.com/emres/ModernTinyGP

## Other relevant repositories on GitHub

There are also a few other repositories on GitHub that have the source code, as
well as attempts at Java modernisation:

* https://github.com/JesseBuesking/TinyGP-Java
* https://github.com/marcinkalaus/TinyGP-Java
* https://github.com/Pandoors/TinyGP
* https://github.com/Sitaarz/TinyGP-Java
* https://github.com/tlisowicz/TinyGP-Java

