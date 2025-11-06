# Firefox CSS
A small collection of various Firefox CSS customisations.


## Vertical Tabs with 2-line Labels

Vertical tabs' height has been increased, wrapping the tab labels to two lines.

Includes:
* Full-width tab group labels
* Chevron arrows added to the tab group labels

CSS code: [VerticalTabs-2LineLabels.css](/chrome/VerticalTabs-2LineLabels.css)

![](/screenshots/VerticalTabs-2LineLabels.png)


## Other Styles

Some styles that I'm currently using. These links lead to the original sources for reference.

CSS code: [OtherStyles.css](/chrome/OtherStyles.css)

* Hide the Close button from each tab `*`
* [Move the "leave page" dialog to the top center](https://www.reddit.com/r/FirefoxCSS/comments/1lvn3pe/comment/n27ll9u/)
* [Expand the "Add bookmark" tree-view area](https://www.reddit.com/r/FirefoxCSS/comments/1jj31rw/comment/mjk6pcx/)
* [Lock the side bar width](https://www.reddit.com/r/FirefoxCSS/comments/1jtmptd/comment/mlvl5z6/)
* [Remove the side bar shadow](https://www.reddit.com/r/FirefoxCSS/comments/1j3mx5s/comment/mg256hp/) `*`
* [Make the collapsed Tab Groups' outline not look ugly with dark theme](https://www.reddit.com/r/FirefoxCSS/comments/1k1itvc/comment/mnnxnks/) `*`
* Alternative Back & Forward buttons glyphs
* [Centered URL box text](https://github.com/MrOtherGuy/firefox-csshacks/blob/master/chrome/urlbar_centered_text.css) - Also centered when the URL box is focused
* Outlined URL box
* Transparent BG of Search Mode Switcher Button & URL Bar Label Box
* Remove the green dot from a tab

`*` Also part of "Vertical Tabs with 2-line Labels", so you can use only `VerticalTabs-2LineLabels.css` if you prefer.


## Setup

1. Go to `about:config`.
2. Set the `toolkit.legacyUserProfileCustomizations.stylesheets` flag to `true`.
3. Go to `about:support`.
4. In the "Profile Folder" row, click "Open Folder".
5. In the profile folder, create a folder named `chrome`.
6. Place those CSS files from this GitHub repo into the `chrome` folder.
7. Restart Firefox.
8. Enjoy!

If you have an existing CSS setup, place those CSS files (except `userChrome.css`) into the `chrome` folder,
and add the following path(s) to your `userChrome.css` file:
```
@import "VerticalTabs-2LineLabels.css";
@import "OtherStyles.css";
```
