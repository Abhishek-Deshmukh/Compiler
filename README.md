# Compiler

This compiler was originally written by LukeSmithxyz in his Larbs Setup([More about it](https://larbs.xyz://larbs.xyz/))

I have done some tweaks to it according to my requirements.

This script runs scripts based on the extension of the file being compiled

Feel free to drop in issues.

### Requirements
 Which ever thing you use for compiling

### Currently Supports
- .tex (Latex)
- .mom, .ms (groff)
- .rmd (RMarkDown)
- .md (MarkDown)(using pandoc)
- .py (Python)
- .c (C)
- .html (HTML)(opens in default browser)
- .ts (typescript)
- .js (javascript - node)
- .cpp (C++)
- .go (go)
- .sent (sent)

### Installation
`cd` into the directory where you wanna keep this.

```
$ curl https://raw.githubusercontent.com/Abhishek-Deshmukh/Compiler/master/compiler > compiler
```

The above command will download the contents of the compiler into the file naems `compiler`

### Usage

##### Command line
You can use the above script in the following way

```
$ compiler file.tex
```

This will compile the .tex file into a .pdf file with the same name(`file.pdf`) in the same directory.

##### Vim
You can also use it directly from vim by adding

```
map <leader>c :w! \| !compiler <c-r>%<CR>
```

into you .vimrc

This will set `<leader> c` as the key which you can use to compile your document from within vim.

If you don't know what your leader key is, it's usually \ . But to be sure check the line

```
let mapleader =" "
```
in your .vimrc

There will be something betweent the quotes which will be your leader key.

If you are using vim [check out](https://github.com/Abhishek-Deshmukh/StudentVim) my vimrc repo it include the compiler file and many more features.

