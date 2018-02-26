VimPaneNavigation
=====================

"VimPaneNavigation" is a plugin for the Sublime Text 3 editor that provides
vim-esque keyboard navigation between tabs and split panes (when using multiple
split panes in a window.)

0. **Split Pane Navigation:** Adds key bindings for `ctrl+l` and `ctrl+h` to cycle through the multiple split panes open in a window (if there are multiple split panes).
0. **Sending Tabs To Other Panes:** Adds key bindings for `ctrl+shift+h` and
`ctrl+shift+l` to send tabs from their current pane to the next/previous panes (if there are multiple split panes in a window).

Installation
------------
VimPaneNavigation is available for installed through [Package Control](http://wbond.net/sublime_packages/package_control/installation) for Sublime Text 2. The advantage of using this method is that Package Control will automatically keep VimPaneNavigation up to date with the latest version. To install it with Package Control:

* Make sure you have Package Control installed, instructions available at http://wbond.net/sublime_packages/package_control/installation
* Once you install Package Control, restart Sublime Text 2 and bring up the Command Palette with `cmd+shift+P` (on Mac OS X) or `ctrl+shift+P` (on Windows or Linux).
* Select "Package Control: Install Package" and  wait while Package Control fetches the latest package list.
* Then, start typing "Pane Navigation" and select it from the list when it appears (restarting Sublime Text 2 is not necessary).

Otherwise, you can install VimPaneNavigation with or without git. **With git**:
Clone the repository in your Sublime Text "Packages" directory (`git clone
https://github.com/jetpks/VimPaneNavigation.git`). **Without git**: Download
the latest source from [GitHub](https://github.com/jetpks/VimPaneNavigation) and copy the folder folder to your Sublime Text "Packages" directory.

The "Packages" directory is located at:

* OS X:

        ~/Library/Application Support/Sublime Text 3/Packages/

* Linux:

        ~/.config/sublime-text-3/Packages/

* Windows:

        %APPDATA%/Sublime Text 3/Packages/

Usage
-----
There are four key bindings associated with this plugin (note that in the descriptions, "next" and "previous" refer to the order in which the tabs/panes appear in the window, not based on recency as is the default in Sublime Text 2):

* `ctrl+l`: cycle to the next pane in the active window
* `ctrl+h`: cycle to the previous pane in the active window
* `ctrl+shift+l`: send the current tab to the next pane in the active window
* `ctrl+shift+h`: send the current tab to the previous pane in the active window

Configuring
-----------
If you would like part of the available functionality (for example, if you only want the split pane navigation), simply comment out the key bindings for the unwanted functionality. Additionally, if you would like to change the key bindings, simply edit the "Key Bindings" file available in the preferences menu: `Preferences->Package Settings->Pane Navigation->Key Bindings - Default`.

Credits
-------
This is a lightly edited fork of
[borist's SublimePaneNavigation
plugin](https://github.com/borist/SublimePaneNavigation). The changes from the
original are to use H and L to navigate panes. And to remove the override of
ctrl+tab, and ctrl+shift+tab as it's handled by sublime.

For Full VIM-like editing
-------------------------
For full vim emulation, I use [guillermooo's Six](https://packagecontrol.io/packages/Six).
