<html>
    <h1 align='center'>
        dirsplit
    </h1>
    <p align='center'>
        splits directory into multiple with equal size 
        <br>
        <pre align='center'>sudo curl https://raw.githubusercontent.com/yumiris/dirsplit/master/dirsplit > /usr/local/bin/dirsplit</pre>
    </p>
</html>

# Introduction

`displit` is designed to for a simple purpose: convert a directory with many multiple files (which are all smaller than a certain medium, eg. DVD) and "splits" it into "volumes", looking for the optimal order to get the best space/medium-number efficiency.

The actual action is either adding the files to `mkisofs` catalogs or real moving of files into new directories (or creating links/symlinks). The method is not limited to files, whole directories can also be handled this way (see various filesystem exploration modes).

# Authors

- **Eduard Bloch (blade)**: principal creator and developer of `dirsplit` 
- **Christian Fromme (kaner-guest)**: contributions on the historical SVN repository

# Install

Most distributions will offer `dirsplit` using their dependency manager:

| Distribution | Command                       |
|--------------|-------------------------------|
| Debian       | `apt-get install genisoimage` |
| Ubuntu       | `apt-get install genisoimage` |
| Kali Linux   | `apt-get install genisoimage` |
| CentOS       | `yum install dirsplit`        |
| Fedora       | `dnf install dirsplit`        |
| Raspbian     | `apt-get install genisoimage` |

On other distributions, you may have to manually install `dirsplit`. Arch Linux is an example where manual installation is required. To manually install `dirsplit`, please install Perl and then download the `dirsplit` script as follows:

```sh
sudo curl https://raw.githubusercontent.com/yumiris/dirsplit/master/dirsplit > /usr/local/bin/dirsplit
```

# Notes

This repository preserves the source code and history for `dirsplit`, which has been copied from the now-gone `cdrkit` SVN repository. Distributions such as Arch Linux don't provide `dirsplit`, and thus this repository was created to make the obtaining of `dirsplit` a breeze.