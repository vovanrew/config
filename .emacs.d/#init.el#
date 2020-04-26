;; Initialise the package system first of all.
(package-initialize)

;; Skip the default splash screen.
(setq inhibit-startup-message t)

;; Remove window tool at top
(tool-bar-mode -1)
(scroll-bar-mode -1)

;; Line wrapping
(setq word-wrap          t)
(global-visual-line-mode t)

;; MELPA packages are available
(require 'package)
(add-to-list 'package-archives '("melpa-stable" . "https://stable.melpa.org/packages/") t)
(setq package-enable-at-startup nil)

;; Initializes the package infrastructure
(package-initialize)

;; Tell emacs where is your personal elisp lib dir
(add-to-list 'load-path "~/.emacs.d/modules/")

(autoload 'lua-mode "lua-mode" "Lua editing mode." t)
(add-to-list 'auto-mode-alist '("\\.lua$" . lua-mode))
(add-to-list 'interpreter-mode-alist '("lua" . lua-mode))

;; load ergoemacs mode
(add-to-list 'load-path "~/.emacs.d/modules/ergoemacs-mode")
(require 'ergoemacs-mode)

;; load material theme
(add-to-list 'load-path "~/.emacs.d/modules/emacs-material-theme")
(require 'material-theme)
(load-theme 'material t)
