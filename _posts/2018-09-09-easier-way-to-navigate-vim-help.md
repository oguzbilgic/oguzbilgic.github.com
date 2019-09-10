---
layout: post 
title: Easier Way to Navigate Vim Help
---

# Easier Way to Navigate Vim Help

_September 2019_

Paste the code below to your `vimrc`.

```vim
" Easier way to navigate vim help
augroup vim_help_autocmds
  autocmd!

  " Use <CR> to move to tag
  autocmd FileType help nnoremap <buffer> <cr> <c-]>
  " Use <BS> to go back
  autocmd FileType help nnoremap <buffer> <bs> <c-t>

  " Use <tab> to jump to the next tag within the helpfile
  autocmd FileType help nnoremap <buffer> <tab> /\|\zs\S\{-}\|/<cr>:noh<cr>

  " Center the cursor vertically
  autocmd FileType help setlocal scrolloff=999

  " Scroll half page using J and K
  autocmd FileType help nmap <buffer> J <c-d>
  autocmd FileType help nmap <buffer> K <c-u>
augroup END
```
