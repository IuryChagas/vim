<h1 align="center"> Tips and Tricks </h1>

## Basic Vim Commands You Should Know

| N° | DESCRIPTION | COMMAND |
|--- |--- | --- |
| 01. | Open file | __vim__ _fileName_|
| 02. |Move left |__h__|
| 03. |Move down |__j__|
| 04. |Move up   |__k__|
| 05. |Move right|__l__|
| 06. | Command mode begins with the symbol | __:__ |
| 07. | Close file | __:q__ |
| 08. | Close and don't save | __:q!__|
| 09. | Save changes | __:w__ |
| 10. | Zalva e Zai | __ZZ__ |
| 11. | copy | __y__ |
| 12. | copy a line | __yy__ |
| 13. | paste | __p__ |
| 14. | cut | __d__ |
| 15. | cut a line | __dd__ |
| 16. | cut two lines | __2dd__ |
| 17. | Split the screen to see both files | __:vsplit/path-to-file/file__ |

## Moving inside file

| N° | DESCRIPTION | COMMAND |
|--- |--- | --- |
| 18. |Jump to the end of the file | __G__ |
| 19. |Jump to the beginning of it | __gg__ |
| 20. |Move to a specific line | __123G__ _or_ __123gg__ |
| 21. |Launch file on Vim already on specific line. | __$vim _**filename**_ +n°__ |
| 22. |Move cursor to the beginning of the current line | __0__ |
| 23. |Move cursor to the end of the current line | __$__ |
| 24. | Move cursor to beginning of text on current line | __^__ |
| 25. |Move cursor to the top of the current window | __H__ |
| 26. |Move cursor to the  middle of the current window. | __M__ |
| 27. |Jump to the matching brace "_when you’re editing code_" |  __%__ |
| 28. | Delete char at cursor | __x__ |
| 29. | Insert at cursos | __i__ |
| 30. | Insert beginning of line | __I__ |
| 31. | Append at cursor | __a__ |
| 32. | Append at end of line | __A__ |
| 33. | Exit insert mode | __ESC__ |
| 34. | Delete word | __dw__ |
| 35. | Delete entire line and keep in normal mode | __D__ |
| 36. | Next word | __w__ |
| 37. | Go to '_x_' word forward | __n°w__ |
|_ex._| Go to two word forward | __2w__ |
| 38. | Go to end of third word ahead | __3e__ |

## Recovering information

| N° | DESCRIPTION | COMMAND |
|--- |--- | --- |
| 39. | Undo last change | __u__ |
| 40. | Undo changes on entire line | __U__ |
| 41. | Redo change | __Ctrl__ _+_ __r__ |
| 42. | Open last edited file with the cursor on the last known position | __CTRL + o + o__ |

## Shell commands

| N° | DESCRIPTION | COMMAND |
|--- |--- | --- |
| 43. | Run shell commands inside of it | __:r !__ |
|_ex:_| To output the current month calendar | __:r !cal__ |
|_ex:_| For the current date and time | __:r !date__ |

## History

| N° | DESCRIPTION | COMMAND |
|--- |--- | --- |
| 44. | History of the last commands ran "_consultation only_" | __:history__ |
|_ex:_| interactive command history window. | __q:__ |
|_ex:_| Then is a matter of choosing the command to run and executing it with | < CR > |

## Compressed files

| N° | DESCRIPTION | COMMAND |
|--- |--- | --- |
| 45. | Open compressed file | __$vim archive.tar.gz__ |
|_ds:_| _We can then open, edit and save those files without having to extract them._ | |

##  Don’t know what a command does?

| N° | DESCRIPTION | COMMAND |
|--- |--- | :---: |
| 46. | launch the manpage for the keyword | __K__ |

## searching...

| N° | DESCRIPTION | COMMAND |
|--- |--- | --- |
| 47. | search for all occurrences of the word under the cursor | __*__ |

## Indentation

| N° | DESCRIPTION | COMMAND |
|--- |--- | --- |
| 48. |indent our entire file according to the definition of tabs we’re using|__gg=G__|
| 49. | To take it a step further, <br>we can setup marks to indent an entire file and keep the cursor where it is |__mmgg=G’m__|
| 50. | search for all occurrences of ‘error’ in all .txt files |__:vimgrep error *.txt__|
| 51. | For more information on __*Vimgrep*__ |__:h vimgrep__|

## Checking git branch  using Vim

| N° | DESCRIPTION | COMMAND |
|--- |--- | --- |
|52. | see the contents of a given file in a different branch<br> without having to change into it | __git show__ branch_name:/path/to/file.txt | __vim -__|

__git show__ branch_name:/path/to/file.txt __| vim -__
 
