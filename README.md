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
 <kbd>prefix n</kbd>   | dotnet-new
 <kbd>prefix p</kbd>   | dotnet-publish
 <kbd>prefix r</kbd>   | dotnet-restore
 <kbd>prefix e</kbd>   | dotnet-run
 <kbd>prefix C-e</kbd> | dotnet-run-with-args
 <kbd>prefix t</kbd>   | dotnet-test

You can customize the prefix by adding:
```el
(setq dotnet-mode-keymap-prefix (kbd "<ADD YOUR PREFIX HERE>"))
```

### TODO

- [ ] Handle solutions
- [ ] Fancier test options (specific file/test)
- [ ] Handle nuget advanced commands
- [ ] Handle paket
