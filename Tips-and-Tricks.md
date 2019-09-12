<h1 align="center"> Tips and Tricks </h1>

## Moving inside file _in Normal mode_

| N° | DESCRIPTION | COMMAND |
|--- |--- | --- |
| 01. |Jump to the end of the file | __G__ |
| 02. |Jump to the beginning of it | __gg__ |
| 03. |Move to a specific line | __123G__ _or_ __123gg__ |
| 04. |Launch file on Vim already on specific line. | __$vim _**filename**_ +n°__ |
| 05. |Move cursor to the beginning of the current line | __0__ |
| 06. |Move cursor to the end of the current line | __$__ |
| 07. |Move cursor to the top of the current window | __H__ |
| 08. |Move cursor to the  middle of the current window. | __M__ |
| 09. |Jump to the matching brace "_when you’re editing code_" |  __%__ |

## Recovering information

| N° | DESCRIPTION | COMMAND |
|--- |--- | --- |
|10. | Open last edited file with the cursor on the last known position | __CTRL + o + o__ |

## Shell commands

| N° | DESCRIPTION | COMMAND |
|--- |--- | --- |
|11. | Run shell commands inside of it | __:r !__ |
|ex: | To output the current month calendar | __:r !cal__ |
|ex: | For the current date and time | __:r !date__ |

## History

| N° | DESCRIPTION | COMMAND |
|--- |--- | --- |
|12. | History of the last commands ran "_consultation only_" | __:history__ |
|ex: | interactive command history window. | __q:__ |
|ex: | Then is a matter of choosing the command to run and executing it with | < CR > |

## Compressed files

| N° | DESCRIPTION | COMMAND |
|--- |--- | --- |
|13. | Open compressed file | __$vim archive.tar.gz__ |
|ds: | _We can then open, edit and save those files without having to extract them._ | |

##  Don’t know what a command does?

| N° | DESCRIPTION | COMMAND |
|--- |--- | :---: |
|14. | launch the manpage for the keyword | __K__ |

## searching...

| N° | DESCRIPTION | COMMAND |
|--- |--- | --- |
|15. | search for all occurrences of the word under the cursor | __*__ |

## Indentation

| N° | DESCRIPTION | COMMAND |
|--- |--- | --- |
|16. |indent our entire file according to the definition of tabs we’re using|__gg=G__|
|17. | To take it a step further, <br>we can setup marks to indent an entire file and keep the cursor where it is |__mmgg=G’m__|
|18. | search for all occurrences of ‘error’ in all .txt files |__:vimgrep error *.txt__|
|19. | For more information on __*Vimgrep*__ |__:h vimgrep__|

## Checking git branch  using Vim

| N° | DESCRIPTION | COMMAND |
|--- |--- | --- |
|20. | see the contents of a given file in a different branch<br> without having to change into it | __git show__ branch_name:/path/to/file.txt | __vim -__|

__git show__ branch_name:/path/to/file.txt __| vim -__
 
