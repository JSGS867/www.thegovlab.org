[![Build Status](https://travis-ci.org/GovLab/www.thegovlab.org.svg?branch=master)](https://travis-ci.org/GovLab/www.thegovlab.org)

The GovLab website.

## Quick Start

### NOTE:
If you are updating from any commit prior to [1.0.0](https://github.com/GovLab/www.thegovlab.org/releases/tag/1.0.0)/[e425c0](https://github.com/GovLab/www.thegovlab.org/commit/e425c0ae65ad6fe046bdf29895df1a27ec1d7875), run `npm i` before developing

### Installation

Make sure the following are installed on your machine:

* npm
* Python 2.7
* [pip and virtualenv](http://stackoverflow.com/q/4324558)
* [SASS](http://sass-lang.com/install) (Optional, however, if `sass` isn't on your command-line,
your SASS files won't be rebuilt.)

Run the following commands in the base of your cloned repo:

```
npm i

virtualenv venv

source venv/bin/activate

pip install -r requirements.txt
```

(Note) On Windows, use `venv\Scripts\activate` instead of `source`

### Development

From within local repo, run:

```
source venv/bin/activate
```
if `virtualenv` is not already running in your shell session, and then:

```
python build.py runserver
```
to start the server.

Site will be served at http://localhost:7000 by default.

### Deployment

From within local repo, run:

```
python build.py deploy
```
