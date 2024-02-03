This fork fixes compatibility with the latest Chrome/Edge browsers and improves performance.

---

Due to lack of time this repo has not gotten new updates in a while. While I have not abandoned the project and may update it in the future, for the time being if there are bugs or lack of features that makes this unusable to you, you can instead use one of these alternatives:
- [Hurl](https://github.com/U-C-S/Hurl)
- [Browser Tamer](https://www.aloneguid.uk/projects/bt/)
- [Browser Choose 2](https://browserchooser2.com/)
- [Browser Picker](https://github.com/mortenn/BrowserPicker)
- [Browser Selector](https://github.com/DanTup/BrowserSelector)

---

# Browser Select
Browser Select is a utility to dynamically select the browser you want instead of just having one default for all links. Similar to the prompt in android to choose a browser when a link in a non-browser app is clicked/touched. It may not be useful for everyone but it helps when you use multiple browsers for different things (e.g. one with proxy and one without) and open many links from other applications (e.g. Messengers).

![screenshot1](https://raw.githubusercontent.com/zumoshi/BrowserSelect/master/screenshots/photo_2016-07-11_13-44-19.png)

Instead of having to copy the link, open the desired (non-default) browser then pasting the link, all you need to do is to click on the link and this prompt will open allowing you to choose the browser you want. It automatically detects installed browsers. It does not require administrative rights and can be installed as a restricted user.

![screenshot 2](https://raw.githubusercontent.com/zumoshi/BrowserSelect/master/screenshots/photo_2015-10-12_16-46-14.jpg)

You may click on the desired browser or press one of the shortcuts (its index or the first letter of its name), for example for chrome you can press 2, g or c.
you may also press Esc (or click the X) to not open the URL.

To install Download this file then set it as the default browser.

![select default browser](https://raw.githubusercontent.com/zumoshi/BrowserSelect/master/screenshots/photo_2015-10-12_16-43-08.jpg)

BrowserSelect has been tested on windows 7, windows 8.1 and windows 10. requires **.net framework 4**.

# Download

You can download browser select here : [Browser select v1.4.1 (412KB)](https://github.com/zumoshi/BrowserSelect/releases/download/1.4.1/BrowserSelect.exe)

[![100% safe Award from softpedia](http://s1.softpedia-static.com/_img/sp100free.png?1)](http://www.softpedia.com/get/Internet/Browsers/Browser-Select.shtml#status)


# Related links

[AlternativeTo](http://alternativeto.net/software/browser-select/)

Reviews: [DSTech](http://dipendrashekhawat.com/choose-specific-browser-every-time-you-open-a-link/)
[TrishTech](http://www.trishtech.com/2016/07/use-different-browsers-for-different-links-with-browserselect/)
[DonationCoder](http://www.donationcoder.com/forum/index.php?topic=42860.msg401447)

Download Mirrors: 
[GitHub](https://github.com/zumoshi/BrowserSelect/releases/latest)
[SoftPedia](http://www.softpedia.com/get/Internet/Browsers/Browser-Select.shtml)
[SnapFiles](http://www.snapfiles.com/get/browserselect.html)
[FindmySoft](http://browserselect.findmysoft.com/)
[browserss](http://browserss.ru/m.browser-select.php)
[ComputerBild](http://www.computerbild.de/download/BrowserSelect-15967517.html)

Note: Mirrors may have outdated versions of BrowserSelect. You can always download the latest version [here](https://github.com/zumoshi/BrowserSelect/releases).


# ToDo

Just a list of some ideas that can be integrated into BrowserSelect.
- [x] Make Settings persist across updates
- [x] Shift-Click to open link in incognito/private mode
- [ ] Option to display running browsers only
- [ ] More Auto-Select rule options
    - [ ] based on the source application
    - [ ] based on file extension
    - [ ] based on URL path
    - [ ] based on keywords
    - [ ] ignoring the URL as an option
    - [ ] custom flags to browsers as an option (e.g. incognito mode or disable CSRF)
- [ ] export/import for rules/settings
- [ ] Sorting browsers on the list
- [ ] Custom Shortcuts
- [ ] Ignoring the rules if Alt key is held down when clicking a link
- [ ] an API to invoke BrowserSelect
- [ ] Bugfix for when Browser was launched with Maximize window state (browser select will launch maximized)
- [ ] A browser extension to launch the correct browser based on the rules even if a link is clicked inside a browser
- [ ] support for portable browsers (adding browsers using a browse button rather than registry)
- [ ] support for non-browser apps as an option (e.g. download managers)
- [ ] themes ? or at least an optional transparent Aero glass mode
- [ ] Ability to choose custom icons for browsers
- [ ] display the unshortened version of adf.ly or goo.gl links when selecting the browser
- [ ] Localization
- [ ] handling of other link types (e.g. `mail:` in case you have both outlook and thunderbird installed [or maybe as a sister app])
- [x] update checker (not as a popup or messagebox, a tiny icon somewhere on the main form that appears when you don't have the last version)
- [ ] add file associations (e.g. .url files, or .html files)

# Changelog

v1.4.1 [24/08/19]
- Fixed couldn't hide chrome profiles separately (#52)
- Improved startup speed by caching browsers (#40)
(special thanks to [kthejoker](https://github.com/kthejoker) for his pull request)

v1.4.0 [12/06/18]
- Fixed Opera (post-blink) private mode (#35)
- Chrome profiles are now listed as separate options (#29)
(special thanks to [kueswol](https://github.com/kueswol) for his pull request)

v1.3.9 [06/04/18]
- Fixed Edge private mode (#34)
- Added Alt as an alternative to shift for open in private/incognito mode (#33)

v1.3.8 [20/10/17]
- Fixed pattern generator for single part domains (e.g. localhost) (issue #27)
- Fixed unintended unescaping of URL's (issue #28)

v1.3.7 [16/08/17]
- Fixed issues with clipping on high dpi screens (#24)

v1.3.6 [11/06/17]
- BrowserSelect's window now shows up in the monitor with the mouse cursor instead of the default one (#22)

v1.3.5 [16/12/16]
- fixed crash on startup caused by incompatible/incomplete registry keys (issues #17,#20,#21)

v1.3.4 [02/09/16]
- fixed Always button adding rules with the wrong pattern for second-level domains (e.g. *.com.au for news.com.au)
- Shift Clicking on browsers now opens the URL in incognito/private browsing
- added an update checker (adds a yellow "New" icon to the main window to indicate a new version is available)[disabled by default]

v1.3.3 [03/08/16]
- fixed a crash on malformed (without protocol) URL's
- added donate button in about page

v1.3.2 [28/07/16]
- bugfix to bring IE to the foreground if it is already open

v1.3.1 [14/07/16]
- bugfix for Auto rule creation of domains with subdomains

v1.3 [11/07/16]
- Added an "Always" button under browser icons that adds a rule for *.domain.tld
- Added a help button in the main form
- made about form closable by Esc key
- added a help form for the settings page
- changed how filters are executed to allow simpler use of a match-all pattern
- added browser select to the list of options when adding rules
- added an apply button to the settings page for Rules
- polished the rule adding interface
- some code Formating/Indenting/Restructuring

v1.2.1 [14/06/16]
- bugfix for InternetExplorer to open links in a new tab instead of a new window

v1.2 [08/06/16]
- you can now add URL patterns to select the Browser based on URL automatically.

v1.1 [18/05/16]
- added option to select browsers that are displayed on the list (and remove/hide some)

v1.0.2 [15/01/16]
- added option to set browser select as the default browser in settings

v1.0.1 [27/10/15]
- added edge browser for windows 10 (it wouldn't show up due edge being a Universal App)
