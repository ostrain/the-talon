# The Talon

The Talon is a macOS [service](http://www.macworld.com/article/1163996/software-utilities/how-to-use-services-in-mac-os-x.html)
which allows you to highlight one or more [JIRA](https://www.atlassian.com/software/jira) issue IDs in almost any macOS
application, press a keyboard shortcut of your choosing, and view all of those JIRA issues in your browser. 

For example, if you're viewing commit messages in your terminal and come across a JIRA issue ID like `FOO-123`, you can highight
it and press your shortcut to view it, no copy-and-pasting required.


## Installation

1. Clone the repository.
2. Double click on the "View JIRA Issues" file, then click Install.
3. Configure your JIRA server's URL by running the following command in a Terminal (replacing the example URL):

    `defaults write com.owenstrain.talon.jira url https://jira.example.com/browse/`

4. Define your global keyboard shortcut:
    1. Go to System Preferences > Keyboard > Shortcuts > Services
    2. Find "View JIRA Issues" in the list (under the "Text" section) and assign it a keyboard shortcut that won't conflict with
	normal keyboard shortcuts (e.g. ⌥⇧⌘X)
5. Select some JIRA issue ID(s) in almost any app and press your keyboard shortcut (you can select a whole block of text that
   happens to contain some issue IDs and the regex should find them correctly).


## Future Work

* Installation script that sets the keyboard shortcut for you
  (https://apple.stackexchange.com/questions/115675/set-services-keyboard-shortcut-via-script-osx/115772)
