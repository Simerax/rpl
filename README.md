# Moved to [Gitlab](https://gitlab.com/Simerax/rpl)

# rpl
Bare Bones Perl Repl - No Security, No Fancy Stuff, only REPL
It's basically just a fancy 'eval'

### Why?
I wanted a simple perl repl with minimal dependencies in one script

### Dependencies
* Data::Dump (__not Data::Dumper__)
* Term::ReadLine (a stub is enough but then you won't have a command history)

### What's there?
* Dumping of evaluated expressions
* Ability to require perl files with the §r command (just type §r myfile.pl)
* Strict (can be toggled by §strict and §no-strict - Variables are not strict since every command is in its own eval but things like barewords are caught)
* Code is evaluated in its own package 'REPL' so names don't clash with the main script functions (of course you can still override main functions if you try ;) )


![](https://i.imgur.com/RiZkMZk.gif)
