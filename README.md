#Configuring the command line w/ zsh

###1. Install oh-my-zsh 
```
$ sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

###2. Configure Theme
2. Open `~/.zshrc` file in your text editor
  
Pick a [ZSH_theme](https://github.com/robbyrussell/oh-my-zsh/wiki/Themes)
  

In `.zshrc` file:
```
ZSH_THEME="«your-theme-here»"

```

###3. Zsh features
1. **Supercharged `ls`**
  `ls -«x»` gives a lot of sort-display options for the directory

2.  **Advanced History**
  enter the terminal command and zsh will have a history of that command that you can cycle through with the ↑ key.

3. **Enable plugins** 
  Edit your `~/.zshrc` file 
  ```
  plugins=(git node «plugin-name»)
  ```

  Add some [ZSH plugins](https://github.com/robbyrussell/oh-my-zsh/wiki/Plugins)
  - extract
  - osx (tons of cl utilities)


*PROTIP* `source ~/.zshrc` will update configurations without having to close & reopen the termminal 

###4. Include & Setup *z.sh*
* Note: must have *homebrew* to install z (homebrew requires Xcode)*

  1. `$ brew install z.sh`  

  2. `$ curl https://raw.githubusercontent.com/rupa/z/master/z.sh >> z.sh`  

  3.  In `~/.zshrc` file:
    ```
    #include Z
    . ~/z.sh
    ```
  4. now you can `z «directory-or-file_name»` to navigate to 'frecent' directories
