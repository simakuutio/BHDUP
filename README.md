[![h1n054ur - BHDUP](https://img.shields.io/static/v1?label=h1n054ur&message=BHDUP&color=blue&logo=github)](https://github.com/h1n054ur/BHDUP)
[![stars - BHDUP](https://img.shields.io/github/stars/h1n054ur/BHDUP?style=social)](https://github.com/h1n054ur/BHDUP)
[![forks - BHDUP](https://img.shields.io/github/forks/h1n054ur/BHDUP?style=social)](https://github.com/h1n054ur/BHDUP)

<h1 align="center">
	<img width="400" src="bhdup-logo.png" alt="BHDUP">
</h1>

# BHDUP


Script to Automate Uploading using BHDAPI written using python 3.9 (mostly)

## Usage:

You will need 3 keys to run this script, google how to register for tmdbv3api its free, the other two ask in the forums if you are unsure.

Rename directories according to BHD naming conventions.

Run it from inside directory where you have all properly named releases make sure bhdup.py and .env are in the same directory.

    python3 bhdup.py  or python3 /path/to/bhdup.py

Make sure there is nothing other than the Directories you want to make torrents of, the .env and the bhdup.py files in your current working directory.

## Install

I'm going to pretend you have no python experience.

0.1 **Install mktorrent:** https://github.com/Rudde/mktorrent

0.2 **Install ffmpeg:** https://github.com/FFmpeg/FFmpeg

0.3 **Install mediainfo:** https://github.com/MediaArea/MediaInfoLib

0.4 **Install imgbox-cli:** https://github.com/plotski/imgbox-cli

1. Check which python you have.
2. Clone this repo.
3. Go into this repo.
4. Install the requirements.
5. Copy .env.example to .env

Steps 1-5:

```
python3 --version
git clone https://github.com/fachizel/BHDUP.git
cd BHDUP
pip install -r requirements.txt
cp .env.example .env
```

6. **Update `.env` file to have YOUR KEYS and change Screenshot times if you need follow the format in .env.example .**

## Notes:

- If you mess up and get stuck with a ton of temp files and want to delete them all from the current directory before re-running the script, use this handy command:

      rm -r *.files tmp *.png mediainfo.txt *.torrent

- Only works with UHD Remux, BD Remux, DVD Remux, 2160p, 1080p and 720p, Might include missing categories later.

- Assumes all directories are named correctly, media files are one directory deep, and no whitespaces in names that will confuse mktorrent.

- Logo made with courtesy of https://www.freelogodesign.org/
