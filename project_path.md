# The goal of this repo is to install and use the Apache Web Server  [![alt text][1]](https://www.apache.org/) on a Raspberry Pi [![alt text][1]](https://www.raspberrypi.com/) at home
<!-- TODO:1 -->
<!-- important outside the TOC block -->
<!-- markdownlint-disable MD039 -->
- [The goal of this repo is to install and use the Apache Web Server   on a Raspberry Pi  at home](#the-goal-of-this-repo-is-to-install-and-use-the-apache-web-server---on-a-raspberry-pi--at-home)
  - [Connect to the Raspberry Pi via the VS-Code Extensions **Remote - SSH**](#connect-to-the-raspberry-pi-via-the-vs-code-extensions-remote---ssh)
  - [Show desktop from Raspberry Pi over local network - linux based client,  rdesktop and xrdp ](#show-desktop-from-raspberry-pi-over-local-network---linux-based-client--rdesktop-and-xrdp-)
  - [Show desktop from Raspberry Pi over SSH tunnel](#show-desktop-from-raspberry-pi-over-ssh-tunnel)
  - [miscellaneous - off topic](#miscellaneous---off-topic)
<!--- THis empty line is necessary for correct format -->
<!-- TODO:0 -->
<!-- BUG THe both extension **markdownlint** and **Todo Tree** are INCOMPATIBLE as I use them->
>[!NOTE]
> Markdown All in One Documentation - Compatibility - Known issues [![alt text][1]](https://markdown-all-in-one.github.io/docs/guide/compatibility.html)
<!--- THis empty line is necessary for correct format -->
>[!NOTE]
> GitHub repo markdownlint  [![alt text][1]](https://github.com/DavidAnson/markdownlint)
<!--- THis empty line is necessary for correct format -->
> [!TIP]
> Markdown Link as Image instead of text
><!--- THis empty line is necessary for correct format -->
> <!-- - Whats the recommended syntax for an image with a link? [![alt text][1]](https://meta.stackexchange.com/questions/2133/whats-the-recommended-syntax-for-an-image-with-a-link) -->
> - Whats the recommended syntax for an image with a link? [![alt text][1]]([![alt text][2]])
><!--- THis empty line is necessary for correct format -->
> <!-- [![alt text][1]](https://meta.stackexchange.com/questions/2133/whats-the-recommended-syntax-for-an-image-with-a-link) -->
> - HTML Links syntax [![alt text][1]](https://www.w3schools.com/html/html_links.asp)
><!--- THis empty line is necessary for correct format -->
>```html
> [![alt text][1]](URL)
>```
><!--- THis empty line is necessary for correct format -->
> ```markdown
> [![alt text][1]](https://stackoverflow.com/questions/22697688/how-to-cat-eof-a-file-containing-code)
> <!-- Picture of link symbol -->
> [1]: ./img/link_symbol.svg
> ```
> <!--- THis empty line is necessary for correct format -->
> - alternative - even clearer method
> <!--- THis empty line is necessary for correct format -->
> ```markdown
> [alt text][1]][2]
> <!-- Picture of link symbol -->
> [1]: ./img/link_symbol.svg
> <!-- Link Address>
> [2]: https://link_adress
> ```
<!--- THis empty line is necessary for correct format -->
[2]: https://meta.stackexchange.com/questions/2133/whats-the-recommended-syntax-for-an-image-with-a-link
<!--- THis empty line is necessary for correct format -->
> [!Note]
> <!--- THis empty line is necessary for correct format -->
> - NGINX [![alt text][1]](https://nginx.org/) vs. Apache [![alt text][1]](https://www.apache.org/)
>   - The Ultimate Web Server Showdown in 2024 [![alt text][1]](https://www.cloudways.com/blog/nginx-vs-apache/)
>   - This website describes in detail the difference between these programs
<!--- THis empty line is necessary for correct format -->

## Connect to the Raspberry Pi via the VS-Code Extensions **Remote - SSH**

- Follow this Tutorial [![alt text][1]](https://carleton.ca/scs/2024/vscode-remote-access-and-code-editing/)

>[!Tip]
>How to install VSCode extensions from the command line. We using the ssh-remote extension as an example [![alt text][1]](https://stackoverflow.com/questions/34286515/how-to-install-visual-studio-code-extensions-from-command-line)
><!-- -->
>- List already installed extensions
> <!-- -->
> ```bash
> code --list-extensions
>```
><!-- -->
>- Find the name of extension ```<extension_name>``` [![alt text][1]](https://code.visualstudio.com/docs/getstarted/extensions)
>   - One path among many
> <!-- -->  
>1. Open the Extensions view by selecting the Extensions icon in the Activity Bar, or use the Ctrl+Shift+X keyboard shortcut
>2. Click the extension in the main window
>3. Click on the extension's name (first row). A new browser window should open.
>4. In this window you will see the name of the extension
><!-- -->
>- Install extension
><!-- -->
>```bash
>#code --install-extension <extension_name>
>code --install-extension ms-vscode-remote.remote-ssh
>echo $? #return value should be zero
>```
><!-- -->
>- Remove extension
><!-- -->
>```bash
>#code --uninstall-extension <extension_name>
>code --uninstall-extension ms-vscode-remote.remote-ssh
>echo $? #return value should be zero
>```
><!-- -->
>Check via command line it the extension installed
><!-- -->
>```bash
>#code --list-extensions | grep <extension_name>
>code --list-extensions | grep ms-vscode-remote.remote-ssh
>echo $? #return value should be zero
>```
<!--- THis empty line is necessary for correct format -->
>[!TIP]
>Disable the screen blanking [![alt text][1]](https://www.reddit.com/r/debian/comments/7ft10g/new_to_debian_all_i_want_to_do_for_now_is_disable/)
>command
><!--- THis empty line is necessary for correct format -->
>```bash
>```
><!--- THis empty line is necessary for correct format -->

## Show desktop from Raspberry Pi over local network - linux based client,  rdesktop and xrdp [![alt text][1]](https://debianforum.de/forum/viewtopic.php?t=158811#p1071435)
<!-- https://www.google.com/search?client=firefox-b-e&channel=entpr&q=debian+rdesktop -->

- command

```bash
rdesktop -z -P -x l -a 32 -g 1200x800 -k de 192.168.178.40
```

## Show desktop from Raspberry Pi over SSH tunnel

## miscellaneous - off topic

- Capitalization and lowercase in English - Groß- und Kleinschreibung im Englischen [![alt text][1]](https://de.pons.com/p/wissensecke/grammatik-to-go/gross-kleinschreibung-englisch)
<!--
xset s off && xset -dpms && xset s noblank
https://www.reddit.com/r/debian/comments/7ft10g/new_to_debian_all_i_want_to_do_for_now_is_disable/

htop like disk usage
-->
<!-- Link sign - Don't Found a better way :-( - You know a better method? - Please send me a email -->
[1]: ./img/link_symbol.svg
