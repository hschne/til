---
title: Disable Specific Lsp Servers in Neovim 
date: 2025-05-28
tags: neovim
---

# Disable Specific Lsp Servers in Neovim 

I have a bunch of language servers set up using nvim-lspconfig and Mason. Sometimes I get to a new project where a particular LS and it's annotations are in the way. 

Then I can use `LspStop server-name` (e.g. `LspStop rubocop`) to stop that language server.
