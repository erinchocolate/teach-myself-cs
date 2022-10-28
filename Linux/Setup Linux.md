# 🐧Setup Linux

## Study Note ✍️

### Setup Manjaro

Manjaro is an arch-based os. I use Pacman to install packages.

Git

- `sudo pacman -S git`

Yay

- `sudo git clone <https://aur.archlinux.org/yay-git.git$ cd yay-git$ makepkg -si`

Chrome

- `git <https://aur.archlinux.org/google-chrome.gitmakepkg -s`

Vim

- `sudo pacman -S vim`

Neovim

- `sudo pacman -S base-devel cmake unzip ninja tree-sitter curl`
- `git clone <https://github.com/neovim/neovimcd neovim && makesudo make install`

Visual studio code

- `sudo pacman -S code`

fish shell

- `sudo pacman -S fish`

- Install Oh my fish - `curl <https://raw.githubusercontent.com/oh-my-fish/oh-my-fish/master/bin/install> | fish`

- Install neofetch 
  - `git clone <https://github.com/dylanaraps/neofetch>`
  - `cd neofetch`
  - `sudo make install`
  - `need to change fish.config to display automatically`

### Dual Boot

Step 1: Create a new partition for new OS

- How to open Disk Management in Windows 10

  - The easiest way to open Disk Management in Windows 10 is from computer Desktop. Right click on Start Menu (or press Windows+X hotkey) and then select "Disk Management".

  - Use Windows+R hotkey to open Run window. Then type "Diskmgmt.msc" and click "OK" or hit "Enter" key.

Step2: After you open Disk Management, right click the partition you would like to expand and then choose

Step3: use [rufus](https://rufus.ie/en/) to save the Linux OS

Step4: Enter BIOS and choose bootable usb as Boot option

Step5: Install Linux and reboot

### Minecraft Server

How to transfer files from local linux to server?

- In Unix, you can use [SCP (the scp command)](https://www.google.com/search?q=how+to+transfer+file+from+local+to+remote+server+linux&oq=how+to+t&aqs=chrome.0.69i59l2j69i57j0i512l2j69i60l3.2836j0j1&sourceid=chrome&ie=UTF-8)to securely copy files and directories between remote hosts without starting an FTP session or logging into the remote systems explicitly. The scp command uses SSH to transfer data, so it requires a password or passphrase for authentication.

JNI Error when starting a Minecraft Server?

- The problem comes from the fact that your JRE (Java Runtime Enviroment), that is your installed Java version and your JDK (Java Development Kit) do not work together correctly.
- Download the lastest Java JDK version

### VPN

- Choose openvpn in AWS market place
- Generate SSH keys
  - ssh key too open error? `chmod 400 ~/.ssh/id_rsa`