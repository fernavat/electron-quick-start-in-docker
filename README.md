# electron-app

This is a dockerfile to launch an electron gui within a docker container.

Currently, the sole image is oriented toward a dev environment where the the source code changes a lot (and is therefore in a bound volume), because it's where I'm at.

I'm merely beginning my electron(ic) journey and so far this image only ran an "hello world" example, so I can't really vouch about its correctness yet, except that it can run an hello world example :).

## Usage

The 'dockerfile' and 'entryScript.sh' files that I used to build the image that was pushed in the docker hub are included for completeness, but not necessary to run the image.

You just need to use docker-compose to make use of the prescribed settings to launch the container.

You'll want to tweak the settings (user name and id and corresponding home folder) in the docker-compose.yml file to reflect your environment and change the content of the 'app' directory with your electron app.

## Name Change Notice

Changed the name (including the image) for this project from atom-electron to electron-app as I found the previous name confusing (given the existence of the Atom text editor) when revisiting the project after a prolonged absence. I'll keep the old atom-electron image on my docker hub for compatibility reason in the unlikely event that someone out there is depending on it.
