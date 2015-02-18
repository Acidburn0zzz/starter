setshell
=====
set the shell for a user in terminal.app and if present, copy dotfiles/iterm2.plist to ~/Library/Preferences/com.googlecode.iterm2.plist
-----
**requires:**
\- ansible\-playbook \-K for sudo only if your shell_path is outside of /bin<br />

playbook use:<br />
&nbsp;&nbsp;\- role: setshell<br />
&nbsp;&nbsp;&nbsp;&nbsp;shell\_path: "/bin/zsh"<br />
