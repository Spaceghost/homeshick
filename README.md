homeshick [![Build Status](https://travis-ci.org/Spaceghost/homeshick.png?branch=development)](https://travis-ci.org/Spaceghost/homeshick)
=========
In Unix, configuration files are king.  
Tailoring tools to suit your needs through configuration can be empowering.  
An immense number of hours is spent on getting these adjustments just right,
but once you leave the confines of your own computer, these local optimizations are left behind.

By the power of git, homeshick enables you to bring the symphony of settings
you have poured your heart into with you to remote computers.
With it you can begin to focus even more energy on bettering your work environment
since the benefits are reaped on whichever machine you are using.

However bare bones these machines are, provided that at least bash 3 and git 1.5 are available you can use homeshick.
homeshick can handle multiple dotfile repositories. This means that you can install
larger frameworks like [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh)
or a multitude of emacs or vim plugins alongside your own customizations without clutter.

For detailed [installation instructions](https://github.com/Spaceghost/homeshick/wiki/Installation), [tutorials](https://github.com/Spaceghost/homeshick/wiki/Tutorials) and [tips](https://github.com/Spaceghost/homeshick/wiki/Automatic-deployment) & [tricks](https://github.com/Spaceghost/homeshick/wiki/Symlinking) have a look at the [wiki](https://github.com/Spaceghost/homeshick/wiki).

Quick install
-------------

homeshick is installed to your own home directory and does not require root privileges to be installed.
```sh
git clone git://github.com/Spaceghost/homeshick.git $HOMESICK_DIR/repos/homeshick
```
*Note: If you'd like to help testing new features before they are released use `git clone --branch testing git://...`*

To invoke homeshick, source the `homeshick.sh` script from your rc-script:
```sh
# from sh and its derivates (bash, zsh etc.) 
printf '\nsource "$HOMESICK_DIR/repos/homeshick/homeshick.sh"' >> $HOME/.bashrc
# fish shell
echo \n'source "$HOMESICK_DIR/repos/homeshick/homeshick.fish"' >> "$HOME/.config/fish/config.fish"
```

Contributing
------------

Before submitting pull requests or reporting bugs, please make sure to read
the [contribution guidelines](CONTRIBUTING.md).
