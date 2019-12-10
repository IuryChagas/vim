<h1 align="center"> Tips and Tricks </h1>

## Basic Vim Commands You Should Know

| N° | DESCRIPTION | COMMAND |
|--- |--- | --- |
| . | Open file | __vim__ _fileName_|
| . |Move left |__h__|
| . |Move down |__j__|
| . |Move up   |__k__|
| . |Move right|__l__|
| . | Command mode begins with the symbol | __:__ |
| . | Close file | __:q__ |
| . | Close and don't save | __:q!__|
| . | Save changes | __:w__ |
| . | Zalva e Zai | __ZZ__ |
| . | copy | __y__ |
| . | copy a line | __yy__ |
| . | paste | __p__ |
| . | cut | __d__ |
| . | cut a line | __dd__ |
| . | cut two lines | __2dd__ |
| . | Split screen to see both files vertically | **:vsplit** _file_|
|_ex:_| Use **tab** after typed **_:vsplit_** to see files or directory options |**:vsplit OtherFile**|
| . | Open file at last line **+** _or_ **$**| **vim _fileName_ +**|
|_ex:_| Open file at last line **$** _or_ **+**| **vim _fileName_ $**|
| . | Open file and go to specific line **+n°**| **vim _fileName_ +8**|
| . | Open two files splitted in horizontal columns **-o**| **vim -o _file1 file2_**|
| . | Switch between files _Ctrl + ww_|**Ctrl ww**|
| . | Open two files splitted in vertical columns **-O**| **vim -O _file1 file2_**|
| . | Save and close all files |**wqa**|
| . | Don't save and close all files |**wqa!**|

## Moving inside file

| N° | DESCRIPTION | COMMAND |
|--- |--- | --- |
| . | Jump to the end of the file | __G__ |
| . | Go to last line of file _same effect of **G**_|**:$**|
| . | Jump to the beginning of it | __gg__ |
| . | Move to a specific line | __123G__ _or_ __123gg__ or __122j__ or __122k__ |
| . | Launch file on Vim already on specific line. | __$vim _**filename**_ +n°__ |
| . | Move cursor to the beginning of the current line | __0__ |
| . | Move cursor to the end of the current line | __$__ |
| . | Move cursor to beginning of text on current line | __^__ |
| . | Move cursor to the top of the current window | __H__ |
| . | Move cursor to the  middle of the current window. | __M__ |
| . | Jump to the matching brace "_when you’re editing code_" |  __%__ |
| . | Delete char at cursor | __x__ |
| . | Replace word | __r__ |
| . | Insert at cursos | __i__ |
| . | Insert beginning of line | __I__ |
| . | Append at cursor | __a__ |
| . | Append at end of line | __A__ |
| . | Exit insert mode | __ESC__ |
| . | Delete word | __dw__ |
| . | Delete entire line and keep in normal mode | __D__ |
| . | Next word | __w__ |
| . | Go to '_x_' word forward | __n°w__ |
|_ex:_| Go to two word forward | __2w__ |
| . | Go to end of third word ahead | __3e__ |
| . | Salve **all** files and close files | __:wqa__ |
| . | navigate on file to up | __Ctrl__+__u__|
| . | navigate on file to down | __Ctrl__+__d__|
| . | navigate between paragraphs block, to up |__{__|
| . | navigate between paragraphs block, to down |__}__|
| . | Jump to next paragraph, to Up **shift + (** |**shift (**|
| . | Jump to next paragraph, to Down **shitft + )** |**shift )**|
| . | Navigate using context with |__%__|
| . | Set lines with position numbers _**nu!**_ or _**number**_ |**:set nu!**|
| . | Go to especific line **n°** |**:5**|
|_ex:_| **:55** _Jump to 55 line_ |_line 55_|
| . | Save a specific excerpt from inside the file |**:5,10w newFileToSave.md**|
|_ds_| inside the file type _initial n°_, _final n°_**w** **NewFileName.extension** |**:5,10w newFileName.md**|
|_ds_| the content at line 5 to line 10 will be saved in newFileName.md |
| . | To subwrite an existing file _:n°w! nameExistingFile.extension_|**:1,5w! nameExistingFile.md**|

## Moving and editing inside line

| N° | DESCRIPTION | COMMAND |
|--- |--- | --- |
| . | Moving word to word with Control and arrow -> | __Ctrl + -> __ |
| . | Moving by  lines, stop on first letter of line n°+_ ex: | **4**_ |
| . | Next word, stop at end letter of word | __e__ |
|_ex._| ex: Go to end of fifth word | __5e__ |
| . | Go to High of the window |__H__|
| . | Go to Middle of the window |__M__|
| . | Go to Low of the window |__L__|
| . | Go to especify charactere/word |__fCharactereHere__|
|_ex:_| _Go to ()_ | __f(__|
|_ex._| Go to third parenthesis ex: |__3f(__|
|_ex._| Go to next occurrence of search used by f |__;__|
|_ex:_| search 'a'. Use __fa__, now find next occurrence of 'a'. Use __;__
| . | Find this next word | * |
| . | Go to next word like this |__n__|
| . | Back to word like this |__N__|
| . | Altern by uppercase/lowercase |__~__|
| . | Change a word |__cw__|
| . | Change whole word |__caw__|
| . | Repeat the previous action |__.__|
| . | Sellect all with |**ggVG**|
| . | Delete x first lines |**:d19**|
|_ds_| _note!_ depends on the current cursor position. |**:d19**|
|_ds_| _If at the beginning of the file. 19 first lines will be deleted_ |**:d19**|
|_ds_| _If at end of file_. 10 last lines will be deleted_ |**:d10**|
 
## On mode Visual

| N° | DESCRIPTION | COMMAND _init v_|
|--- |--- | --- |
| . | To select word or paragraphs, just use |__h, j, k , l__|
| . | Transform to lowercase |__u__|
| . | Transform to Uppercase |__U__|
|_ex:_| Select word or paragraphs and use |__u__ or __U__|
| . | reverse selected lines order |__!tac__|
| . | commnet multiple lines `ctrl`+`v` + `n°`+`j`, `shift`+`i` + `symbol` + `Esc` + `Esc`|**V** + **20j** + **shift i** + **#** + **Esc** + **Esc**|
| .| comment multiple lines with Regex `:InitLine,LastLine s/^/symbol/g` ex:|**:9,23 s/^/#/g**|
|_ds_| `s` = substitute. `^` = beginning of line. `#` = symbol to comment in vi. `g` = globally | |
| . | Compare modifications between files |**vimdiff file-vs1 file2-vs2**|

## Recovering information

| N° | DESCRIPTION | COMMAND |
|--- |--- | --- |
| . | Undo last change | __u__ |
| . | Undo changes on entire line | __U__ |
| . | Redo change | __Ctrl__ _+_ __r__ |
| . | Open last edited file with the cursor on the last known position | __CTRL + o + o__ |

## Shell commands

| N° | DESCRIPTION | COMMAND |
|--- |--- | --- |
| . | Run shell commands inside of it | __:r !__ |
|_ex:_| To output the current month calendar | __:r !cal__ |
|_ex:_| For the current date and time | __:r !date__ |

## History

| N° | DESCRIPTION | COMMAND |
|--- |--- | --- |
| . | History of the last commands ran "_consultation only_" | __:history__ |
|_ex:_| interactive command history window. | __q:__ |
|_ex:_| Then is a matter of choosing the command to run and executing it with | `<CR>` |

## Compressed files

| N° | DESCRIPTION | COMMAND |
|--- |--- | --- |
| . | Open compressed file | __$vim archive.tar.gz__ |
|_ds:_| _We can then open, edit and save those files without having to extract them._ | |

##  Don’t know what a command does?

| N° | DESCRIPTION | COMMAND |
|--- |--- | :---: |
| 76. | launch the manpage for the keyword | __K__ |

## searching... and editing...

| N° | DESCRIPTION | COMMAND |
|--- |--- | --- |
| . | Search and Replace |__:s/1°/2°/g__|
| ex. | Search and Replace |__:s/old/new/g__|
|_ds:_| /Replacethisto/new |__/__|
|_ds:_| /new change |__/__|
|_ds:_| To global change |__/g__|
|_ex:_| You can specify by lines >> |__:1,10%s/old/new/g__|
|_ds:_| You will change all occurrences of **old** to **new** from line 1 up to line 10. |__:1,10%s/old/new/g__|
|_ds:_| To search the entire file change the line numbers to a percent symbol: |__:%s/old/new__|
| . | Search specific word. _ex_ **lorem** |**/lorem**|
|_ds_| _The vim search mechanics is case sensitive_|
|_ds_|_To next occurrence of word, press **Enter** after typed /lorem_ and press **n** to occurrences down |**n**|
|_ds_|_To next occurrence of word, press **Enter** after typed /lorem_ and press **shift + n** to occurrences Up |**N**|
| . | Editing file with vim without leaving the command line. _Ex:_ | **vi -c ":% s/word/NewWord/g" -c ":x" file.txt** |
| . | To see more information about vim map |**:map**|

## Mapping

| N° | DESCRIPTION | COMMAND |
|--- |--- | --- |
| . | Commands mapping, ex ggVG to select all text |**:map `<F12>` ggVG**|
|_ds_| The command key **F12** is set to run like ggVG. _"select all text file"_ now |**F12** _is the same_ **ggVG**|
|_ds_| Other example _to select all text_ now with `Ctrl` + `a` |**:map `C-a` ggVG**|

## Indentation

| N° | DESCRIPTION | COMMAND |
|--- |--- | --- |
| . |indent all the file. sellect all with __ggVG__ and use __=__|__ggVG__ _+_ __=__|
| . |indent our entire file according to the definition of tabs we’re using|__gg=G__|
| . | To take it a step further, <br>we can setup marks to indent an entire file and keep the cursor where it is |__mmgg=G’m__|
| . | search for all occurrences of ‘error’ in all .txt files |__:vimgrep error *.txt__|
| . | For more information on __*Vimgrep*__ |__:h vimgrep__|

## Checking git branch  using Vim

| N° | DESCRIPTION | COMMAND |
|--- |--- | --- |
| . | see the contents of a given file in a different branch<br> without having to change into it | __git show__ branch_name:/path/to/file.txt | __vim -__|

__git show__ branch_name:/path/to/file.txt __| vim -__
 
