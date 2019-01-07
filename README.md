My Vim Customizations
===

## About
These files contain my personal Vim customizations. So far I have implemented the following:

* [Vundle](https://github.com/VundleVim/Vundle.vim), a Vim package manager
* [One Dark theme](https://github.com/joshdick/onedark.vim), a theme for Vim based on Atom's One Dark theme

## Notes
The following list describes how I have the files configured on my computer, which is set up according to 
the [set-up tutorial](https://eecs280staff.github.io/p1-stats/setup.html#command-line-tools) of my university's introductory CS course.
I use [Windows 10 Subsystem for Linux (WSL)](https://eecs280staff.github.io/p1-stats/setup_wsl.html) with an Ubuntu Bash Shell.

1. The files in this repository are located in a folder named `.vim`, which is itself located in my home directory (`~` a.k.a. `/home/Username`).

2. The `vimrc` found in this repository is hard-linked to the `.vimrc` file found in my home directory (one directory up). This was accomplished by
running the following line in the shell:

	`ln ~/.vimrc ~/.vim/vimrc`  

	Of course, this was performed when I had everything in the `.vimrc` and the `vimrc` file was non-existent. You may have to adjust this for your own use.
	Basically, the only reason for the `vimrc` file is to make it easier to upload the `.vim` folder to github and make it easier to edit and find the rc file.

3. To use Vundle, it may be neceesary to install the plugins which are listed in the `vimrc` file. To accomplish this, run the following line in shell, or 
better yet, just take a look at the [Vundle set-up instructions](https://github.com/VundleVim/Vundle.vim).

	`vim +PluginInstall +qall`
