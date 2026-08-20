# Markade

A miscellaneous collection of arcade `.mra` and `.rbf` files for the **MiSTer FPGA** platform.

The files in this repository have been gathered from various public sources around the MiSTer community and are collected here mainly for convenience and easy installation through the MiSTer Downloader.

## What’s Included

* Arcade `.mra` definition files
* Arcade `.rbf` FPGA cores
* Experimental, beta, uncommon or older arcade cores and definitions

**No ROM files or copyrighted game data are included in this repository.**

## ⚠️ Experimental Content

Some files in Markade may be:

* Beta or work-in-progress
* Buggy or incomplete
* Older builds
* Hardware or configuration dependent
* Currently non-functional

There is no guarantee that every core or MRA in this repository will work correctly.

This collection is intended more as a useful archive of interesting MiSTer arcade content than a curated set of guaranteed-working releases.

## Installation

Markade can be added as a custom database for the MiSTer Downloader.

Add the following to the bottom of your `downloader.ini`:

```ini
[Usquebagh/Markade]
db_url = https://raw.githubusercontent.com/Usquebagh/Markade/db/db.json.zip
```

Then run:

```text
update_all.sh
```

or the standard MiSTer Downloader.

Files will automatically be installed into their corresponding locations under `_Arcade`.

## Updates

When files are added, removed or updated in this repository, the Markade downloader database is rebuilt automatically.

Running `update_all.sh` will then pull the latest available versions onto your MiSTer.

## ROM and LaserDisc Files

Some cores require additional ROM files that are not included in this repository.
Place any required MAME ROMs in:

/games/mame/

LaserDisc game files (.dlv) should be placed in:
/games/laserdiscgames/

Check the relevant core or MRA documentation for any game-specific file requirements.

## Credits

The `.rbf` cores and `.mra` files contained here are the work of their respective developers, maintainers and contributors within the MiSTer community.

Markade does not claim authorship of third-party cores or MRA definitions. This repository exists primarily as a convenient collection and distribution point.

If you are the author of something included here and would like attribution added, a source corrected, or a file removed, please open an issue.
