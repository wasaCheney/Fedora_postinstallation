# Fedora post-installation
- Update, `sudo dnf update -y`
- Ghleper
- [Enable rpmfusion free and nonfree](https://rpmfusion.org/Configuration)
  - `sudo dnf install https://mirrors.rpmfusion.org/free/fedora/rpmfusion-free-release-$(rpm -E %fedora).noarch.rpm https://mirrors.rpmfusion.org/nonfree/fedora/rpmfusion-nonfree-release-$(rpm -E %fedora).noarch.rpm`

# Apps via GetApps
- gnome tweak tools/extentions
- Chrome, Edge
- GIMP, Blender, 2D/3D image processing
- LibreOffice suite (TexMath extention. and WPS office - online version - tex supported, MicroSoft Office - online version)
- Draw.io (Of course it can works online, flowchart, mindmap, etc.)
- Flameshot (works properly under X11 rather than Wayland, screenshot)
- Zathura, pdf
- Anydesk, remote desk
- Jabref, reference management, [browser extension](https://docs.jabref.org/collect/jabref-browser-extension)
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
- [NVim](https://github.com/neovim/neovim/blob/master/INSTALL.md)
  - `sudo dnf install -y neovim python3-neovim`
- [Spacevim](https://spacevim.org/)
  - python, latex, markdown...
