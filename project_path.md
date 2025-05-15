# The goal of this repo is to install and use the Apache Web Server  [![alt text][1]](https://www.apache.org/) on a Raspberry Pi to use it at home

- [The goal of this repo is to install and use the Apache Web Server   on a Raspberry Pi to use it at home](#the-goal-of-this-repo-is-to-install-and-use-the-apache-web-server---on-a-raspberry-pi-to-use-it-at-home)
  - [Connect to the Raspberry Pi via the VS-Code Extensions **Remote - SSH**](#connect-to-the-raspberry-pi-via-the-vs-code-extensions-remote---ssh)
  - [miscellaneous - off topic](#miscellaneous---off-topic)

> [!TIP]
><!--- THis empty line is necessary for correct format -->
> - Image as text for a markdown link [![alt text][1]](https://meta.stackexchange.com/questions/2133/whats-the-recommended-syntax-for-an-image-with-a-link)
>   - Whats the recommended syntax for an image with a link? [![alt text][1]][2]
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

## miscellaneous - off topic

- Capitalization and lowercase in English - Groß- und Kleinschreibung im Englischen [![alt text][1]](https://de.pons.com/p/wissensecke/grammatik-to-go/gross-kleinschreibung-englisch)

<!-- Link sign - Don't Found a better way :-( - You know a better method? - Please send me a email -->
[1]: ./img/link_symbol.svg
