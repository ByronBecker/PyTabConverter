To execute a python 2.7 file after upgrading to python3, one 

commonly runs into problems with the error 

TabError: inconsistent use of tabs and spaces in indentation

To fix this, one can use the following command

:set tabstop=4 shiftwidth=4 expandtab
:retab

:set is a necessary predecessor for tabstop, shiftwidth, and expandtab
tabstop=4 sets the amount indented by tab equal to 4 spaces

shiftwidth=4 changes the number of space characters inserted for
			 indentation

expandtab turns all tabs into spaces

However, this setting change will only work for future tabs, so
:retab is to apply the new tab settings to all tabs in the file 

...
