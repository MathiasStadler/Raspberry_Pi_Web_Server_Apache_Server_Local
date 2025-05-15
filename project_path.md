# The goal of this repo is to install and use on Raspberry Pi the web server Apache Server [![alt text][1]](https://www.apache.org/)

- in its current stable version
- connected via ssh for remote used

> [!TIP]
><!--- THis empty line is necessary for correct format -->
> - Image as text for a markdown link [![alt text][1]](https://meta.stackexchange.com/questions/2133/whats-the-recommended-syntax-for-an-image-with-a-link)
>   - Whats the recommended syntax for an image with a link? [![alt text][1]][2]
><!--- THis empty line is necessary for correct format -->
> ```markdown
> [![alt text][1]](https://stackoverflow.com/questions/22697688/how-to-cat-eof-a-file-containing-code)
> ```
> <!--- THis empty line is necessary for correct format -->
> - alternative - even clearer method
> <!--- THis empty line is necessary for correct format -->
> ```markdown
> [alt text][1]][2]
> <!-- Link Symbol -->
> [1]: ./img/link_symbol.svg
> <!-- Link Address>
> [2]: https://link_adress
> ```
<!--- THis empty line is necessary for correct format -->
[2]: https://meta.stackexchange.com/questions/2133/whats-the-recommended-syntax-for-an-image-with-a-link
<!--- THis empty line is necessary for correct format -->
> [!Note]
> <!--- THis empty line is necessary for correct format -->
> - **NGINX vs. Apache**
>   - The Ultimate Web Server Showdown in 2024 [![alt text][1]](https://www.cloudways.com/blog/nginx-vs-apache/)
>   - This website describes in detail the difference between these programs
<!--- THis empty line is necessary for correct format -->

## Connect to the Raspberry Pi via the VS-Code Extensions **Remote - SSH**

- Tutorial Link [![alt text][1]](https://carleton.ca/scs/2024/vscode-remote-access-and-code-editing/)

>[!Tip]
>How to install Visual Studio Code extensions from command line [![alt text][1]](https://stackoverflow.com/questions/34286515/how-to-install-visual-studio-code-extensions-from-command-line)
><!-- -->
>List already installed extensions
> <!-- -->
> ```bash
> code --list-extensions
>```
><!-- -->>
>Install extension
><!-- -->
>```bash
> code --install-extension ms-vscode-remote.remote-ssh
>```
><!-- -->
>Remove extension
><!-- -->
>```bash
> code --uninstall-extension ms-vscode-remote.remote-ssh
>```
><!-- -->
>Check via command line it the extension installed
><!-- -->
>```bash
> # code --list-extensions | grep <extension name>
> code --list-extensions | grep ms-vscode-remote.remote-ssh
> echo $? # return value should be zero
>```

<!-- Link sign - Don't Found a better way :-( - You know a better method? - Please send me a email -->
[1]: ./img/link_symbol.svg
