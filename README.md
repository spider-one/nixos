# nixos

for the initial setup, install with a basic configuration.nix to start

pull the git repo into ~/etc

will likely need to move the /etc/nixos/hardware-configuration.nix

need to set up .gitignore for the hardware-configuration.nix file

my configuration.nix will take over from the default configuration.nix

```
mkdir ~/etc
sudo mv /etc/nixos ~/etc/
sudo chown -R $(id -un):users ~/etc/nixos
sudo ln -s ~/etc/nixos /etc/
```

initialize the git repo and push online

will need the ssh private key in order to push

```
git remote add origin https://github.com/spider-one/nixos.git
git branch -M main
git push -u origin main
```

```
ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIFtLWWzTPW99+YOmSF7p4Nt6odElCtEusYnsqNUasEHi
```
