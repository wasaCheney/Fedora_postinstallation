# Fedora post-installation
- Update, `sudo dnf update -y`
- Vi keybinding for terminal, `set -o vi` to your .bashrc
- Git config to show Chinese characters, `git config --global core.quotePath false`
- Ghleper
- [Enable rpmfusion free and nonfree](https://rpmfusion.org/Configuration)
  - `sudo dnf install https://mirrors.rpmfusion.org/free/fedora/rpmfusion-free-release-$(rpm -E %fedora).noarch.rpm https://mirrors.rpmfusion.org/nonfree/fedora/rpmfusion-nonfree-release-$(rpm -E %fedora).noarch.rpm`
- Mount drive on startup:
  - Find UUID, `sudo blkid`
  - Add to `/etc/fstab`,
  - `UUID=   MountPoint  defaults 0 0`

# Apps via GetApps
- gnome tweak tools/extentions
- Chrome, Edge
- GIMP, Blender, 2D/3D image processing
- LibreOffice suite (TexMath extention. and WPS office - online version - tex supported, MicroSoft Office - online version)
- Draw.io (Of course it can works online, flowchart, mindmap, etc.)
- Flameshot (works properly under X11 rather than Wayland, screenshot)
- Zathura, pdf
  - [Config](https://gist.github.com/michaelmrose/9595075b43f24aa903fa)
    - mkdir and create file, `~/.config/zathura/zathurarc`
  - Make backward search working:
    - Set zathura as the default app for pdf files: choose a pdf file, and right click open with, set as default
    - Modify the spacevim latex.vim, comment out `let g:tex_flavor = "latex"`, and add `let g:vimtex_view_method = "zathra"`
    - Then modify your tex file, compile, `CTRL + Click` will take you back from zathura pdf to the tex file
- Anydesk, remote desk
- Jabref, reference management, [browser extension](https://docs.jabref.org/collect/jabref-browser-extension), [for flatpak browser](https://github.com/JabRef/JabRef-Browser-Extension/issues/611#event-13223959021)
- PeaZip, file archiver

## Texlive

- [Fedora Rec.](https://docs.fedoraproject.org/en-US/neurofedora/latex/)
  - `sudo dnf install texlive-scheme-full`
- Overleaf may be the best oneline version for tex

## Nvidia CUDA
- Follow the [rpmsufion Nvidia](https://rpmfusion.org/Howto/NVIDIA), and [rpmfusion CUDA](https://rpmfusion.org/Howto/CUDA)

## Anaconda Pytorch
- Anaconda, [download and install](https://www.anaconda.com/download/success)
- Pytorch, [CLI install](https://pytorch.org/get-started/locally/)

## Matlab
- ???

## Vim NVim SpaceVim
- Vim keybind for gnome-terminal
  - Add `set -o vi` to `.bashrc`
- [NVim](https://github.com/neovim/neovim/blob/master/INSTALL.md)
  - `sudo dnf install -y neovim python3-neovim`
- [Spacevim](https://spacevim.org/)
  - python, latex, markdown...
