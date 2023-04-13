# BASNomadModsDownloader

A simple PowerShell script to automatically download all the Blade and Sorcery: Nomad mods you subscribed to on mod.io.

## Usage

1. Log in to https://mod.io
2. Go to "My account"
3. On the left side of the screen, click on `🔑 ACCESS`
4. Generate API access and OAuth access keys if you don't have them yet (you'll also have to first accept the terms and conditions)
5. Generate an OAuth access *token*. The token should have read access. You can choose what you want to name it.
6. Download the `Download_mods.ps1` file and place it in a folder where you want downloaded zips of mods to appear
7. Right-click the `Download_mods.ps1` file and select "Run with PowerShell". It should ask you some things install location.
8. It'll eventually ask for your OAuth token. Copy the token you generated on mod.io's Access page and paste it there.

If you have done the setup once then it'll just read the settings from the configuration file it generated and everything should happen automatically. If you want to redo the setup, delete or rename `config.json` and it should show the prompts again.

When you run it a window should pop up where it'll tell you how many subscriptions it found, and it should start downloading and unpacking all the zip files.

If you re-run the script at a later date, it will check your subscriptions for updates and it'll only download mods from new subscriptions or mods which have been updated.

After downloading your mods, and if you let the script extract to the questmods folder, then you can copy all the folders inside the questmods folder into your BAS: Nomad mod folder on your Quest.
