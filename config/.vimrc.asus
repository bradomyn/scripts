
set nocompatible    " use vim defaults

" set UTF-8 encoding
set enc=utf-8
set fenc=utf-8
set termencoding=utf-8

" use indentation of previous line
set autoindent
" use intelligent indentation for C
set smartindent

" configure tabwidth and insert spaces instead of tabs
set tabstop=4        " tab width is 4 spaces
set shiftwidth=4     " indent also with 4 spaces
set expandtab        " expand tabs to spaces

" wrap lines at 80
set textwidth=80
set wrap
"set wrapmargin=4
" turn syntax highlighting on
set t_Co=256
syntax on
"colorscheme elflord / pablo

colorscheme desert

" turn line numbers on
set number
" highlight matching braces
set showmatch

"set mouse=a " use mouse everywhere


set ls=2            " allways show status line
set scrolloff=3     " aeep 3 lines when scrolling

set showcmd         " display incomplete commands
set hlsearch        " highlight searches
set incsearch       " do incremental searching
set ruler           " show the cursor position all the time
set novisualbell    " turn off visual bell
set nobackup        " do not keep a backup file
set number          " show line numbers
set ignorecase      " ignore case when searching 
"set noignorecase   " don't ignore case
set title           " show title in console title bar
set ttyfast         " smoother changes
"set ttyscroll=0        " turn off scrolling, didn't work well with PuTTY
set modeline        " last lines in document sets vim mode
set modelines=3     " number lines checked for modelines
set shortmess=atI   " Abbreviate messages
set nostartofline   " don't jump to first character when paging
set whichwrap=b,s,h,l,<,>,[,]   " move freely between files
    "set viminfo='20,<50,s10,h

    set autowrite      " auto saves changes when quitting and swiching buffer
    "set expandtab      " tabs are converted to spaces, use only when required
    "set sm             " show matching braces, somewhat annoying...
    "set nowrap         " don't wrap lines

    " Enhanced keyboard mappings
    "
    " in normal mode F2 will save the file
    nmap <F2> :w<CR>
    nmap <F3> :wq<CR>

    " remove spelling 
    nmap <F4> :set nospell<CR>
    nmap <F5> :set spelllang=de<CR>

nmap <F6> :set spelllang=it<CR>
    nmap <F7> :set spelllang=en<CR>

    " in insert mode F2 will exit insert, save, enters insert again
    imap <F2> <ESC>:w<CR>i
    imap <F3> <ESC>:wq<CR>

    " remove spelling 
    imap <F4> <ESC>:set nospell<CR>
    imap <F5> <ESC>:set spelllang=de<CR>
    imap <F6> <ESC>:set spelllang=it<CR>
    imap <F7> <ESC>:set spelllang=en<CR>

    " spelling checker
    "next spelling error 
    nmap <F9>  ]s 
    "previous spelling error
    nmap <F10>  [s
    "The same but in insert mode
    imap <F9> <ESC>]s
    imap <F10> <ESC>[s
    "pop up spelling menu crtl X s
    imap <F8> <C-X>s
    nmap <F8> ei<C-x>s <ESC>

" spell settings
:setlocal spell spelllang=en

"C pluging
filetype plugin on

" --- OmniCppComplete ---
" -- required --
set nocp " non vi compatible mode
" -- optional --
" auto close options when exiting insert mode
autocmd InsertLeave * if pumvisible() == 0|pclose|endif
set completeopt=menu,menuone
" -- configs --
let OmniCpp_MayCompleteDot = 1 " autocomplete with .
let OmniCpp_MayCompleteArrow = 1 " autocomplete with ->
  let OmniCpp_MayCompleteScope = 1 " autocomplete with ::
  let OmniCpp_SelectFirstItem = 2 " select first item (but don't insert)
  let OmniCpp_NamespaceSearch = 2 " search namespaces in this and include  files
  let OmniCpp_ShowPrototypeInAbbr = 1 " show function prototype (i.e.  parameters) in popup window
  " -- ctags --
  " map <ctrl>+F12 to generate ctags for current folder:
  map <F11> :!ctags -R --c++-kinds=+p --fields=+iaS --extra=+q .<CR><CR>
  " add current directory's generated tags file to available tags
  set tags+=~/.vim/tags
