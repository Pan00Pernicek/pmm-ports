# pmmfs
Ports like wrapper for Bedrock Linux's package manager manager (wip)

# usage:

`pmmfs` script needs to be in $PATH, otherwise Makefile wont work

location of ports directory is defined by $location inside script, change it, defaults are unusable

then cd to directory above $location and run `pmmfs make` to generate Makefile that will be used

then run `pmmfs fetch` and wait, it will take long time because i am lazy to optimize/write it in language thats faster than sh

then if you want get details of package using pmmfs, cd to $location and then cd <package manager that have avaible package> then cd <stratum that have avaible package> then cd <package> and then just `make` or `make show`
  
 if you want install package then do same but instead of `make show` do `make install` (as root)
 
 and if you want uninstall package then same but instead of `make show` do `make uninstall` (as root)
