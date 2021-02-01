# 🧟 tlz's [Scoop](https://scoop.sh/) bucket 🪣

Originally created so that I could finish my Windows 10 setup script, I now try to add any applications I come across that meet the [requirements](#requirements), just to make everyone's lives a little bit easier.

![](screenshot.png)

[Installation](#installation) · [Uninstallation](#uninstallation) · [Applications](#applications) · [Disclaimer](#disclaimer) · [Requirements](#requirements) · [Contributing](#contributing)

## Installation

To add this bucket to your Scoop installation, run the following command:

```
scoop bucket add tlz https://github.com/TheLastZombie/scoop-bucket
```

**tlz** is the recommended title, though you can replace it with any name you'd like.

## Uninstallation

If you decide you no longer need this bucket, run the following command to uninstall it:

```
scoop bucket rm tlz
```

This will not remove any applications installed from this bucket, though it will prevent you from getting any new updates for them.

If you chose a different title during the installation above, you'll have to replace **tlz** with the one you chose.

## Applications

To view a list of all included applications, head over to the [Scoop directory](https://rasa.github.io/scoop-directory/by-bucket#TheLastZombie_scoop-bucket) or, if you prefer, take a look inside the [bucket folder](https://github.com/TheLastZombie/scoop-bucket/tree/master/bucket).

## Disclaimer

Please note that some applications might not be portable, i. e. they may:

- create and use directories outside of their own (e. g. [ZOC Terminal](https://www.emtec.com/zoc/))
- create and modify registry keys and values (e. g. [sshpm](https://thelastzombie.github.io/sshpm/))
- access your system in other ways (e. g. [Xreveal](https://yubsoft.com/xreveal/))

It should also be noted that currently, some applications (e. g. [Bandcamp Downloader](https://github.com/Otiel/BandcampDownloader)) don't persist their files correctly.

## Requirements

For an application to be added, it needs to meet the following criteria:

- It must not be available via any other bucket listed in the [Scoop directory](https://rasa.github.io/scoop-directory/by-bucket).
- If written in Node.js or Python, it must not be available via [npm](https://www.npmjs.com/) or [pip](https://pip.pypa.io/).
- It must not require administrative or elevated privileges for the installation.
- It needs to provide a way to check for updates, so that it can be [auto-updated](https://github.com/marketplace/actions/bucket-minion).

Currently, the only exceptions to these rules are my own applications and [youtube-dlc](https://blackjack4494.github.io/yt-dlc/).

## Contributing

If you find anything that needs improvement (such as an application not working correctly if installed via this bucket), don't hesitate to [open an issue](https://github.com/TheLastZombie/scoop-bucket/issues/new)!

If you want to contribute application manifests, please consider the following alternatives first:

- If we're talking about one or two applications only, submit them to a fitting [well-known bucket](https://github.com/lukesampson/scoop/blob/master/buckets.json) instead.
- If we're talking about multiple applications, consider [creating your own bucket](https://github.com/lukesampson/scoop/wiki/Buckets#creating-your-own-bucket)! It's a lot of fun.

If you still want to add a manifest to this bucket, I highly recommend you use [Visual Studio Code](https://code.visualstudio.com/) – it will automatically load the [settings file](https://github.com/TheLastZombie/scoop-bucket/blob/master/.vscode/settings.json) included in this repository which, in turn, will make the process easier for you.
