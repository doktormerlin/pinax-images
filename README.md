# Pinax Images Rethought

This is a fork of [Pinax Images](https://github.com/pinax/pinax-images) with some additions and changes that I thought Pinax Images missed.

## Changes

1. Removed "preview" field in Admin.py. The <img/> Tag did not work and there already is a clickable link to the image in the Image field
2. Added "ID" readonly field to the inline-admin, so that [pinax-blog](https://github.com/pinax/pinax-blog) images are usable again.
3. Added "Alt text" field to make alt-texts in template possible
4. Added image optimization using [django-optimized-image](https://pypi.org/project/django-optimized-image/)

## Installation

So far, the only way to install it, is to install it from source.

**If you want to use it together with pinax-blog, you have to install the [original pinax-images package](https://github.com/pinax/pinax-images) first!**

### Using Pip

1. Open a commandline
2. Install the package with `pip install git+https://github.com/doktormerlin/pinax-images-rethought.git`

### Using setup.py

1. Open a commandline
1. Clone this repository with `git clone https://github.com/doktormerlin/pinax-images-rethought`
2. CD To the cloned directory with `cd pinax-images-rethought`
3. Install the package using `python setup.py install`


## Usage

Add `OPTIMIZED_IMAGE_METHOD = 'pillow'` to your settings.py

For other usage, please take a look at the [original README file](README_original.md)