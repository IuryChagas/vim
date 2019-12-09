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
| 17. | Split the screen to see both files | **:vsplit/**_path-to-file_**/**_file_|
| 18. | Open file at last line **+**| **vim _fileName_ +**|
| 19. | Open file and go to specific line **+n°**| **vim _fileName_ +8**|
| 20. | Open two files splitted in vertical columns **-o**| **vim -o _file1 file2_**|
| 21. | Open two files splitted in vertical columns **-O**| **vim -O _file1 file2_**|

## Moving inside file

| N° | DESCRIPTION | COMMAND |
|--- |--- | --- |
| 22. |Jump to the end of the file | __G__ |
| 23. |Jump to the beginning of it | __gg__ |
| 24. |Move to a specific line | __123G__ _or_ __123gg__ or __122j__ or __122k__ |
| 25. |Launch file on Vim already on specific line. | __$vim _**filename**_ +n°__ |
| 26. |Move cursor to the beginning of the current line | __0__ |
| 27. |Move cursor to the end of the current line | __$__ |
| 28. | Move cursor to beginning of text on current line | __^__ |
| 29. |Move cursor to the top of the current window | __H__ |
| 30. |Move cursor to the  middle of the current window. | __M__ |
| 31. |Jump to the matching brace "_when you’re editing code_" |  __%__ |
| 32. | Delete char at cursor | __x__ |
| 33. | Replace word | __r__ |
| 34. | Insert at cursos | __i__ |
| 35. | Insert beginning of line | __I__ |
| 36. | Append at cursor | __a__ |
| 37. | Append at end of line | __A__ |
| 38. | Exit insert mode | __ESC__ |
| 39. | Delete word | __dw__ |
| 40. | Delete entire line and keep in normal mode | __D__ |
| 41. | Next word | __w__ |
| 42. | Go to '_x_' word forward | __n°w__ |
|_ex._| Go to two word forward | __2w__ |
| 43. | Go to end of third word ahead | __3e__ |
| 44. | Salve **all** files and close files | __:wqa__ |
| 45. | navigate on file to up | __Ctrl__+__u__|
| 46. | navigate on file to down | __Ctrl__+__d__|
| 47. | navigate between paragraphs, to up |__{__|
| 48. | navigate between paragraphs, to down |__}__|
| 49. | Navigate using context with |__%__|

## Moving and editing inside line

| N° | DESCRIPTION | COMMAND |
|--- |--- | --- |
| 50. | Moving word to word with Control and arrow -> | __Ctrl + -> __ |
| 51. | Moving by  lines, stop on first letter of line n°+_ ex: | **4**_ |
| 52. | Next word, stop at end letter of word | __e__ |
|_ex._| ex: Go to end of fifth word | __5e__ |
| 53. | Go to High of the window |__H__|
| 50. | Go to Middle of the window |__M__|
| 54. | Go to Low of the window |__L__|
| 55. | Go to especify charactere/word |__fCharactereHere__|
|_ex:_| _Go to ()_ | __f(__|
|_ex._| Go to third parenthesis ex: |__3f(__|
|_ex._| Go to next occurrence of search used by f |__;__|
|ex:| search 'a'. Use __fa__, now find next occurrence of 'a'. Use __;__
| 56. | Find this next word | * |
| 57. | Go to next word like this |__n__|
| 58. | Back to word like this |__N__|
| 59. | Altern by uppercase/lowercase |__~__|
| 60. | Change a word |__cw__|
| 61. | Change whole word |__caw__|
| 62. | Repeat the previous action |__.__|

## On mode Visual

| N° | DESCRIPTION | COMMAND _init v_|
|--- |--- | --- |
| 63. | To select word or paragraphs, just use |__h, j, k , l__|
| 64. | Transform to lowercase |__u__|
| 65. | Transform to Uppercase |__U__|
|_ex:_| Select word or paragraphs and use |__u__ or __U__|
| 66. | reverse selected lines order |__!tac__|

## Recovering information

| N° | DESCRIPTION | COMMAND |
|--- |--- | --- |
| 67. | Undo last change | __u__ |
| 68. | Undo changes on entire line | __U__ |
| 69. | Redo change | __Ctrl__ _+_ __r__ |
| 70. | Open last edited file with the cursor on the last known position | __CTRL + o + o__ |

## Shell commands

| N° | DESCRIPTION | COMMAND |
|--- |--- | --- |
| 71. | Run shell commands inside of it | __:r !__ |
|_ex:_| To output the current month calendar | __:r !cal__ |
|_ex:_| For the current date and time | __:r !date__ |

## History

| N° | DESCRIPTION | COMMAND |
|--- |--- | --- |
| 72. | History of the last commands ran "_consultation only_" | __:history__ |
|_ex:_| interactive command history window. | __q:__ |
|_ex:_| Then is a matter of choosing the command to run and executing it with | < CR > |

## Compressed files

| N° | DESCRIPTION | COMMAND |
|--- |--- | --- |
| 73. | Open compressed file | __$vim archive.tar.gz__ |
|_ds:_| _We can then open, edit and save those files without having to extract them._ | |

##  Don’t know what a command does?

| N° | DESCRIPTION | COMMAND |
|--- |--- | :---: |
| 74. | launch the manpage for the keyword | __K__ |

## searching... and editing...

| N° | DESCRIPTION | COMMAND |
|--- |--- | --- |
| 75. | Search and Replace |__:s/1°/2°/g__|
| ex. | Search and Replace |__:s/old/new/g__|
|_ds:_| /Replacethisto/new |__/__|
|_ds:_| /new change |__/__|
|_ds:_| To global change |__/g__|
|_ex:_| You can specify by lines >> |__:1,10%s/old/new/g__|
|_ds:_| You will change all occurrences of **old** to **new** from line 1 up to line 10. |__:1,10%s/old/new/g__|
|_ds:_| To search the entire file change the line numbers to a percent symbol: |__:%s/old/new__|

## Indentation

| N° | DESCRIPTION | COMMAND |
|--- |--- | --- |
| 76. |indent all the file. sellect all with __ggVG__ and use __=__|__ggVG__ _+_ __=__|
| 77. |indent our entire file according to the definition of tabs we’re using|__gg=G__|
| 78. | To take it a step further, <br>we can setup marks to indent an entire file and keep the cursor where it is |__mmgg=G’m__|
| 79. | search for all occurrences of ‘error’ in all .txt files |__:vimgrep error *.txt__|
| 80. | For more information on __*Vimgrep*__ |__:h vimgrep__|

## Checking git branch  using Vim

| N° | DESCRIPTION | COMMAND |
|--- |--- | --- |
| 81. | see the contents of a given file in a different branch<br> without having to change into it | __git show__ branch_name:/path/to/file.txt | __vim -__|

__git show__ branch_name:/path/to/file.txt __| vim -__
 
