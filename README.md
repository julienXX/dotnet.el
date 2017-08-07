# dotnet.el

[dotnet CLI](https://docs.microsoft.com/en-us/dotnet/core/tools/index) mode for Emacs. This package gives you a set of key combinations to perform dotnet CLI tasks within your .NET Core projects.

## Installation

This package can be installed through [melpa](https://melpa.org/):

```
M-x package-install dotnet
```

## Usage

Add dotnet-minor-mode to your csharp-mode-hook or fsharp-mode-hook

```el
(add-hook 'csharp-mode-hook 'dotnet-minor-mode)
;; and/or
(add-hook 'fsharp-mode-hook 'dotnet-minor-mode)
```

You will now have the following key combinations at your disposal:

 Keybinding             | Command
------------------------|----------------------
 <kbd>C-c C-c a p</kbd> | dotnet-add-package
 <kbd>C-c C-c a r</kbd> | dotnet-add-reference
 <kbd>C-c C-c b</kbd>   | dotnet-build
 <kbd>C-c C-c c</kbd>   | dotnet-clean
 <kbd>C-c C-c n</kbd>   | dotnet-new
 <kbd>C-c C-c p</kbd>   | dotnet-publish
 <kbd>C-c C-c r</kbd>   | dotnet-restore
 <kbd>C-c C-c e</kbd>   | dotnet-run
 <kbd>C-c C-c C-e</kbd> | dotnet-run-with-args
 <kbd>C-c C-c t</kbd>   | dotnet-test

### TODO

- [ ] Handle solutions
- [ ] Fancier test options (specific file/test)
- [ ] Handle nuget advances commands
- [ ] Handle paket
