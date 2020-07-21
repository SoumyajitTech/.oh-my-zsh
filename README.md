# Oh-My-ZSH
This is my configaration file for zsh....
## Install zsh through your Package Manager
```
sudo pacman -S zsh
```
## make Zsh Your Default shell                                                                                                                                 
```   
chsh 
```
## Then change it to /bin/zsh
```
/bin/bash >> /bin/zsh
```
**Type** `echo $SHELL` **to verify your current shell**
``` 
echo $SHELL >> /usr/bin/zsh
```
## Installing Oh My Zsh
```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```
## Installing PowerLeve10K Theme
```
git clone https://github.com/romkatv/powerlevel10k.git $ZSH_CUSTOM/themes/powerlevel10k
```
## Install FuraMono Nerd Font
**For Arch-** `yay -S otf-fura-mono-powerline-git`    

## Download Plugins for auto-suggestion
```
git clone https://github.com/zsh-users/zsh-autosuggestions.git $ZSH_CUSTOM/plugins/zsh-autosuggestions
```
## Download Plugins for Syntax Highlighting
```
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git $ZSH_CUSTOM/plugins/zsh-syntax-highlighting
```
## Change ypur .zshrc file in your home folder
```
sudo nano ~/.zshrc
```
**Find the** `ZSH_THEME` **and replace it with**
```
ZSH_THEME="powerlevel10k/powerlevel10k"
```
## Also add this line below to use Nerd-Fonts
```
POWERLEVEL9K_MODE="nerdfont-complete"
```
## To enable auto-currection uncomment this line
```
#ENABLE_CORRECTION="true"
//To This
ENABLE_CORRECTION="true"
```
## Now add the plungins which you have downloaded
```
Plugins=(git)
//To This
plugins=(git zsh-autosuggestions zsh-syntax-highlighting)
```
## Now save your `.zshrc` file and exit
## Change Font
You will also have to go to **preferences** of your terminal and change to the custom **font** which you installed.
`FiraMono Nerd Font Regular 12`

## Now the last Step
You will need to run **p10k configure** command to setup your terminal looks as per your choice. Just follow the steps. In the last select **option 3** which is **verbose** and then hit **Y** to save changes to your `.zshrc` file

