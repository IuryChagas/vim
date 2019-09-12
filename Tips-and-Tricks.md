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

