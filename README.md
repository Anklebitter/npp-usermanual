Notepad++ User Manual
=======

***Documentation is like sex, when it's good, it's very, very good; when it's bad, it's better than nothing.***

Of course, it's not our goal to create bad documentation, but you get what we mean.

[**Notepad++ User Manual**](https://npp-user-manual.org) is built collaboratively, and your contribution is very welcome. Before submitting a pull request (PR), please check our [contribution rules](CONTRIBUTION.md) to prevent your PR from being rejected.



Summary
=======

* [Getting started](content/docs/getting-started.md)
* [Programing Languages](content/docs/programing-languages.md)
* [User Defined Language System](content/docs/user-defined-language-system.md)
* [Searching](content/docs/searching.md)
* [Session](content/docs/session.md)
* [Macros](content/docs/macros.md)
* [Auto-completion](content/docs/auto-completion.md)
* [Function List](content/docs/function-list.md)
* [Plugins](content/docs/plugins.md)
* [Preferences](content/docs/preferences.md)
* [Themes](content/docs/themes.md)
* [Command Line Arguments](content/docs/command-prompt.md)
* [Shell Extension](content/docs/shell-extension.md)
* [Binary Translation](content/docs/binary-translation.md)
* [Upgrading](content/docs/upgrading.md)
* [Other Resources](content/docs/other-resources.md)


How to test site locally
=======

**Notepad++ User Manual** website is generated by [Hugo](https://gohugo.io/) by using [hugo-book theme](https://github.com/alex-shpak/hugo-book).
In order to visualize the site (with your modification) on your computer locally, you have to download [Hugo **extended** version](https://github.com/gohugoio/hugo/releases) firstly.
Go to the root of Notepad++ User Manual repository under your bash shell (use `Git bash` under windows) then type `HUGODIR\hugo.exe server --minify --theme book`

```bash
donh@MYPC MINGW64 /c/husbandIsNotATM/npp-usermanual (adapt_hugo_book_theme)
$ /c/tmp/hugo/hugo_ext/hugo.exe server --minify --theme book
Building sites …
                   | EN
+------------------+----+
  Pages            | 23
  Paginator pages  |  0
  Non-page files   |  0
  Static files     | 14
  Processed images |  0
  Aliases          |  0
  Sitemaps         |  1
  Cleaned          |  0

Total in 69 ms
Watching for changes in C:\husbandIsNotATM\npp-usermanual\{content,themes}
Watching for config changes in C:\husbandIsNotATM\npp-usermanual\config.toml
Environment: "development"
Serving pages from memory
Running in Fast Render Mode. For full rebuilds on change: hugo server --disablastRender
Web Server is available at http://localhost:1313/ (bind address 127.0.0.1)
Press Ctrl+C to stop

```

Type [http://localhost:1313/](http://localhost:1313/) on the adress bar of your browser et voilà!
