# nvim_config
Directory : ~/.config/nvim/

Prerequisites : 
  - For OCaml linter : OPAM(OCaml package manager), Merlin(Download by OPAM), conf-vim(Download by OPAM)
  - For Python linter : Pylint(Download by apt-get)
  - For Python autocompletor : jedi-vim(Package download by Vundle)

Pylint options :
  - disabled = (C) : Conventions, (R) : Refactors, (W) : Warnings
  - abled = (E) : Errors, (F) : Fatals
  - only showing abled options

Troubleshooting :
  - merlin error - 'Syntastic' not recognizing ocamlmerlin  
  - check path settings on the shell by  
  <code># echo $PATH</code>  
  - if there is no ocamlmerlin path on the shell, then add the path by  
  <code># export PATH=$PATH:/home/jmyang/.opam/4.04.2/bin</code>  
  - merlin uses ocamlmerlin binary files for running
  - read and try [this](https://github.com/ocaml/merlin/wiki/vim-from-scratch)(at the bottom) for troubleshooting
  - **must read [this](https://github.com/neovim/python-client).** must set vim python compile settings for Neovim

Merlin Key Bindings :
  - Ctrl + x + o : Auto-complete
  - Ctrl + c + t : MerlinTypeOf
  - Ctrl + c + l : MerlinLocate(Locate the definition)
  - Ctrl + c + r : Clear enclosing

Python autocompletion :
  - Ctrl + space : jedi-vim autocompletion(Requires jevi-vim & pylint)
