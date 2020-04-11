###### 1.) Install ZSH
`sudo apt install zsh`

###### 2.) Install oh-my-zsh
`sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`

###### 3.) Install fonts
https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Regular.ttf
https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Bold.ttf
https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Italic.ttf
https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Bold%20Italic.ttf

###### 4.) Install powerlevel10k
`git clone --depth=1 https://github.com/romkatv/powerlevel10k.git $ZSH_CUSTOM/themes/powerlevel10k`

###### 5.) Go to settings in Windows Terminal, edit Ubuntu profile:
 ```
{
    "guid": "{2c4de342-38b7-51cf-b940-2309a097f518}",
    "hidden": false,
    "fontFace" : "MesloLGS NF", 
    "fontSize" : 13, 
    "padding": "8, 8, 8, 20",
    "colorScheme": "One Half Dark",
    "startingDirectory":"//wsl$/Ubuntu/home/[username here]",
    "name": "Ubuntu",
    "source": "Windows.Terminal.Wsl" 
}
 ```

    
###### 6.) Set ZSH_THEME="powerlevel10k/powerlevel10k" in ~/.zshrc.
`code ~/.zshrc`
Replace line 11 with: `ZSH_THEME="powerlevel10k/powerlevel10k"`

###### 7.) Install ZSH autosuggestions
`git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions`

###### 8.) Add the plugin to the list of plugins for Oh My Zsh to load (inside ~/.zshrc):

`plugins=(zsh-autosuggestions)`
