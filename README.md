# Kirby Lingonberry
[![Release](https://img.shields.io/github/release/S1SYPHOS/kirby-lingonberry.svg)](https://github.com/S1SYPHOS/kirby-lingonberry/releases) [![License](https://img.shields.io/github/license/S1SYPHOS/kirby-lingonberry.svg)](https://github.com/S1SYPHOS/kirby-lingonberry/blob/master/LICENSE) [![Issues](https://img.shields.io/github/issues/S1SYPHOS/kirby-lingonberry.svg)](https://github.com/S1SYPHOS/kirby-lingonberry/issues)

A Kirby port of the [Wordpress](https://wordpress.org) theme '[Lingonberry](https://wordpress.org/themes/lingonberry)'.

> Lingonberry is a clean theme for bloggers, with responsive design and beautiful typography.

**Table of contents**
- [1. Getting started](#getting-started)
- [2. Troubleshooting](#troubleshooting)
  - [Configuration](#configuration)
- [3. Credits / License](#credits--license)

![screenshot of the kirby-lingonberry theme](screenshot.png)

## Getting started
Use one of the following methods to start blogging with `kirby-lingonberry`:

1. [Clone](https://github.com/S1SYPHOS/kirby-lingonberry.git) or [download](https://github.com/S1SYPHOS/kirby-lingonberry/archive/master.zip) this repository.
2. Unzip / Upload the folder to your site's `root`.

### Configuration
Detailed instructions coming soon!

## Troubleshooting
The comment function is still **considered beta**, so beware of the following caveats:
- `markdown.extra` and KirbyComments' [Smartypants](https://daringfireball.net/projects/smartypants/) option being active at the same time throws a `Too few arguments to function Kirby\Component\Smartypants::parse()` error, caused by a [known bug](https://forum.getkirby.com/t/kirby-2-5-8-update-breaks-markdown-smartypants/9259) which will be fixed in the next release - until then, be sure to disable it via `c::set('comments.form.message.smartypants', false)`.
- For the [time being](https://github.com/Addpixel/KirbyComments/issues/34), KirbyComments doesn't work with the 'home' directory [being omitted](https://getkirby.com/docs/developer-guide/advanced/routing#omitting-the-blog-folder-in-urls), therefore activating the comment function disables custom routing of the 'home' directory (so you'll get `http://example.com/home/example-post` instead of `http://example.com/example-post`).

## Credits / License
This is a [port](https://en.wikipedia.org/wiki/Porting) of the Wordpress theme 'Lingonberry', which was originally developed by [Anders Norén](http://www.andersnoren.se/teman/lingonberry-wordpress-theme). `kirby-lingonberry` is licensed under the [GPL v2](LICENSE), but **using Kirby in production** requires you to [buy a license](https://getkirby.com/buy). Are you ready for the [next step](https://getkirby.com/next)?

**Used Kirby extensions:**
- [Comments](https://github.com/Addpixel/KirbyComments)
- [RSS Feed](https://github.com/getkirby-plugins/feed-plugin)
- [Images](https://github.com/medienbaecker/kirby-images)
- [Quickselect](https://github.com/medienbaecker/kirby-quickselect)
- [Multiselect](https://github.com/distantnative/field-multiselect)
- [Color picker](https://github.com/ian-cox/Kirby-Color-Picker)

## Special Thanks
I'd like to thank everybody that's making great software - you people are awesome. Also I'm always thankful for feedback and bug reports :)
