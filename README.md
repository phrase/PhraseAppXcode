# PhraseApp Xcode Plugin

This plugin integrates [PhraseApp](https://phraseapp.com/) into Xcode. Currently it supports uploading and downloading of localization files for [Localizable Strings](http://docs.phraseapp.com/guides/formats/ios-localizable-strings/) and [Xliff](http://docs.phraseapp.com/guides/formats/xliff/).

## Installation

1. Download the latest release from the [Releases](https://github.com/phrase/PhraseAppXcode/releases) tab
2. Make sure you have a plugin folder for your Xcode project, if not:

		mkdir -p ~/Library/Application\ Support/Developer/Shared/Xcode/Plug-ins/

3. Unzip the archive into the Xcode plugin folder:

        ~/Library/Application\ Support/Developer/Shared/Xcode/Plug-ins/

4. Restart Xcode

The plugin was successfully tested on OS X 10.10 with Xcode 6.2, 6.3 and 6.4 but might work with other versions of Xcode and Mac OS, too.

## Setup

To use the plugin from within Xcode go to

    Product > PhraseApp > Settings

and configure your project settings:

* Access token managed from your [account settings](https://phraseapp.com/settings/oauth_access_tokens)
* ProjectID from your [projects overview](https://phraseapp.com/projects)
* Localization file format, e.g. `Strings` or `Xliff`
* Application path that must point to your localization files

	* Localizable.string: Location of your locale.lproj/ folders
    * Xliff: Location of your Xliff files

## Usage

You can upload and download your localization files directly from your Xcode menu:

    Product > PhraseApp > Download locales # Shift + Alt + D
    Product > PhraseApp > Upload locales # Shift + Alt + U

## More Information

* [PhraseApp Support](https://phraseapp.com/contact)
* [PhraseApp Documentation](http://docs.phraseapp.com/)
* [Working with iOS](http://docs.phraseapp.com/guides/setup/ios/)
