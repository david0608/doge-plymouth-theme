## Install plymouth-themes-script

```
$ sudo apt install -y plymouth-themes-script
```

## Place theme files

```
$ sudo cp -r doge /usr/share/plymouth/themes/doge
```

## Install theme

```
$ sudo update-alternatives --install /usr/share/plymouth/themes/default.plymouth default.plymouth /usr/share/plymouth/themes/doge/doge.plymouth 100
```

## Change theme

```
$ sudo update-alternatives --config default.plymouth
...
# select doge theme
...
$ sudo update-initramfs -u
...
```
