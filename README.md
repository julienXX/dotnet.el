# dotnet.el

[![MELPA](http://melpa.org/packages/dotnet-badge.svg)](http://melpa.org/#/dotnet)

[dotnet CLI](https://docs.microsoft.com/en-us/dotnet/core/tools/index) mode for Emacs. This package gives you a set of key combinations to perform dotnet CLI tasks within your .NET Core projects.

## Installation

This package can be installed through [melpa](https://melpa.org/):

```
M-x package-install dotnet
```

## Usage

Add dotnet-minor-mode to your csharp-mode-hook or fsharp-mode-hook

```el
(add-hook 'csharp-mode-hook 'dotnet-mode)
;; and/or
(add-hook 'fsharp-mode-hook 'dotnet-mode)
```

Default prefix is `C-c C-n`, you will now have the following key combinations at your disposal:

 Keybinding            | Command
-----------------------|----------------------
 <kbd>prefix a p</kbd> | dotnet-add-package
 <kbd>prefix a r</kbd> | dotnet-add-reference
 <kbd>prefix b</kbd>   | dotnet-build
 <kbd>prefix c</kbd>   | dotnet-clean
 <kbd>prefix g c</kbd> | dotnet-goto-csproj
 <kbd>prefix g f</kbd> | dotnet-goto-fsproj
 <kbd>prefix g s</kbd> | dotnet-goto-sln
 <kbd>prefix n</kbd>   | dotnet-new
 <kbd>prefix p</kbd>   | dotnet-publish
 <kbd>prefix r</kbd>   | dotnet-restore
 <kbd>prefix e</kbd>   | dotnet-run
 <kbd>prefix C-e</kbd> | dotnet-run-with-args
 <kbd>prefix s a</kbd> | dotnet-sln-add
 <kbd>prefix s l</kbd> | dotnet-sln-list
 <kbd>prefix s n</kbd> | dotnet-sln-new
 <kbd>prefix s r</kbd> | dotnet-sln-remove
 <kbd>prefix t</kbd>   | dotnet-test
 <kbd>prefix T</kbd>   | dotnet-test-rerun

You can customize the prefix by adding:
```el
(setq dotnet-mode-keymap-prefix (kbd "<ADD YOUR PREFIX HERE>"))
```

### TODO

- [x] Handle solutions
- [x] Re-run last test(s)
- [ ] Fancier test options (specific file/test)
- [ ] Handle nuget advanced commands
- [ ] Handle paket
