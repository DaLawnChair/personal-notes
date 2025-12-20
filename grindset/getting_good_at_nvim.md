# Configurations:

Configurations can be found inside of the path:
```bash
/home/johnzhou/.config/nvim
```

Where the file structure is:
```bash
.
├── init.lua                  // configuration set up, and most keybinds for navigation and editing
├── lazy-lock.json
├── LICENSE
├── lua
│   ├── chadrc.lua
│   ├── configs
│   │   ├── conform.lua
│   │   ├── lazy.lua
│   │   └── lspconfig.lua    // lsp movement
│   ├── mappings.lua         // contains debugger info for dap, haven't really used it
│   ├── options.lua
│   └── plugins
│       ├── dap.lua          // dap configs, haven't really used
│       └── init.lua         // loading plugins, like dap, lsp
└── README.md 
```


# Navigations

Classically we have our controls for moving hjkl.

In normal mode, we also have 
* 0 for the start of the line
* $ for the end of the line
* b for previous word
* w for start of the next word
* e for the end of the next word

## More advanced movements (vertical):
* ctrl+d for half a page down
* ctrl+u for half a page up
* \# + gg for global line repositioning
* \# + j/k for relative line positioning
* zz for recentering
* f+{char} for moving to the next instance of char. F+{char} does this for opposite direction
	* ; after doing this moves to the next instance of this
	* , after doing this moves to the prev instance of this

* [ move up across vertical whitespace
* ] move down across vertical whitespace


## More advanced movements (horizontal):
* v+i+<#identifier> lets you match the next instance/move and copy the internal contents
	* ie v+i+" lets you select the contents of the values in the below text
	* this is a good use of my "free time"
* v+a+<#identifier> lets you match the next instance/move and copy the entire thing
	* ie v+a+) lets you copy the entire contents from the expression
	* 4+5+(12321/98999)

## Jump list: all movements will build a list of movements you've made during your session
* ctrl+i walks you forward across the list
* ctrl+o walks you backwards across the list


## marks (`'`)
Using `m<character>`, you can place a mark for where you are within a file. Using marks you can navigate through marks created within the file, or nativate through files:

`'<lower_case_letter>` = go to local mark at `<lower_case_letter>`
`'<upper_case_letter>` = go to global mark at `<upper_case_letter>`
`''` = go to previous mark within the file
`'[0-9]` = move to a file







# Searching:
* if you want to quickly look for intances of phrases you are highlighting
* \* in normal mode will let you find all instances of it in the file and let you use n/N to navigate through them
* / will let you type in the phrase you want to search for and let you use n/N to navigate through them




# Custom Definitions:

Mode: Command Result
All CTLR+4 = end of line
n CTLR+hkjl = move windows in the direction
All CTRL+q/e = move to the previous/next word 
All CTRL+w = delete the previous word

From LSP and telescope (`lua/configs/lspconfig.lua`):
# Credits [Robotic Nation](https://youtu.be/rkLEP2EuvX8?si=tcKYulA_C-e2atUW)

n  K = gets the definition as a small window over the class/function

n gd = Get Definition of a class or function, this will open it on as a new buffer
n gD = Get declaration of a class or function, this will open it on as a new buffer
n gt = Get type definition, this will open it on as a new buffer
n gi = Get implementation, this will open it on as a new buffer
n <leader>df = go to next warning/error in list diagnostics
n <leader>dp = go to prev warning/error in list diagnostics
n <leader>fr = opens a miniwindow where we can view instances of the class/function, and can visit there






# references
https://www.youtube.com/watch?v=ibNvyTD4Icg 
* a lot of content on vertical and horizontal movement tricks
[Robotic Nation](https://youtu.be/rkLEP2EuvX8?si=tcKYulA_C-e2atUW)
* LSP and telescope config
