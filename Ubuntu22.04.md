# Ubuntu 22.04 安装日记

## 软件源

```bash
sudo add-apt-repository universe
sudo add-apt-repository multiverse
sudo apt update
```

## install
```bash
sudo apt install git
sudo apt install imagemagick pdftk
sudo apt install p7zip-full p7zip-rar unar
```

## 驱动问题
```bash
sudo ubuntu-drivers autoinstall
```
## 手机

### [GSConnect](https://www.omgubuntu.co.uk/2018/11/connect-android-ubuntu-gsconnect)
```bash
sudo apt install gnome-shell-extension
```

### [Scrcpy](https://github.com/Genymobile/scrcpy)
```bash
sudo snap install scrcpy
```


## Other 

```bash
# sudo snap install vlc
# sudo snap install code
sudo apt  install vlc
sudo snap install gimp
sudo snap install obs-studio
sudo snap install xournalpp
```
### vscode 
should install deb version from [here](https://code.visualstudio.com/docs/?dv=linux64_deb), 
since the snap version has [bug with input chinese](https://dev.to/dance2die/ubuntu-ibus-not-working-on-visual-studio-code-1m37).

### Some post install
```bash
sudo apt install vlc-plugin-access-extra libbluray-bdj libdvd-pkg
```

## wps
