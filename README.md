# The `envdefx` package

This small package enhances the possibilities of users and developers
to deal with definitions of environments by closing a gap
in \LaTeX's repertoire of definition macros, i.e.
this package provides `\provideenvironment` that acts exactly like
`\providecommand`, just for environments instead of control sequences.
The argument parsing (analougusly) is the same as for `\newenvironment`.

Second and last, there is `\letenv` which is an environment version
of the `\let` primitive. Its syntax is
`\letenv{<arg1=arg2>}`
where `<arg2>` is the name of the environment that will be stored
into an environment with the name `<arg1>`,
and the equal sign in contrast to the one in `\let` is _not_ optional.
(Example: `\letenv{oldcenter=center}`)

The package with its two macros can be used by calling

    \usepackage{envdefx}

after installing it properly, of course.

This is version 1.0 of the package

Copyright (C) 2015 by Ruben Giannotti 

---

This work may be distributed and/or modified under the
conditions of the LaTeX Project Public License, either
version 1.3c of this license or (at your option) any
later version. The latest version of this license is in
  http://www.latex-project.org/lppl.txt
and version 1.3 or later is part of all distributions
of LaTeX version 2005/12/01 or later.

This work has the LPPL maintenance status `maintained'.

The Current Maintainer of this work is Ruben Giannotti.

his work consists of the files
  envdefx.dtx 
  envdefx.ins
and the derived file envdefx.sty.

To install the package:

 1. run `latex blocktable.ins`
 2. move 'envdefx.sty' to locations where LaTeX will find it
