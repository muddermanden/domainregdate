# Purpose

This script takes a list of domain names and returns them sorted by their date of registration. It works for most TLDs, but i.e. WHOIS for `.eu` domains does not provide the registration date on port `43`.

## Install

Just clone this repo to a local folder:

```
git clone https://github.com/muddermanden/domainregdate.git
```

Make sure that `domainregdate` is executable with

```
chmod +x domainregdate
```

For ease of use, you can make a symbolic link to your `~/bin` folder

```
ln -s ~/Documents/GitHub/domainregdate/domainregdate ~/bin/domainregdate
```

## Uninstall 

Just delete the files and symbolic links, if you have created any.

## Usage

If executed without any arguments this is shown

```
$ domainregdate
Usage: domainregdate DOMAIN...
```

Proper usage is

```
$ domainregdate symbolics.com lego.dk diku.dk itu.dk it.edu mhex.dk jubii.dk google.com facebook.com netflix.com twitter.com
1985-03-15: symbolics.com
1987-10-29: diku.dk
1987-10-29: lego.dk
1995-08-03: jubii.dk
1997-03-29: facebook.com
1997-09-15: google.com
1997-11-11: netflix.com
1999-04-12: itu.dk
1999-05-27: it.edu
2000-01-21: twitter.com
2009-05-30: mhex.dk
```
