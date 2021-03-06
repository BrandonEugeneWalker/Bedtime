# Bedtime 

Support healthy sleeping habits by reminding yourself to step away from your screens an hour before bed.


## Get it from the elementary OS AppCenter!

[![Get it on AppCenter](https://appcenter.elementary.io/badge.svg)](https://appcenter.elementary.io/Bedtime)

This app is available on the elementary OS AppCenter.

# Install it from source

You can of course download and install this app from source.

## Dependencies

Ensure you have these dependencies installed

* granite
* gtk+-3.0
* switchboard-2.0

## Install, build and run

```bash
# install elementary-sdk, meson and ninja 
sudo apt install elementary-sdk meson ninja
# clone repository
git clone {{repository_url}} Bedtime
# cd to dir
cd Bedtime
# run meson
meson build --prefix=/usr
# cd to build, build and test
cd build
sudo ninja install && Bedtime
```

## Generating pot file

```bash
# after setting up meson build
cd build

# generates pot file
sudo ninja Bedtime-pot

# to regenerate and propagate changes to every po file
sudo ninja Bedtime-update-po
```
