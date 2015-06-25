# Incog-NEET

> It's the only NEET thing to do.

-- Alice

## Description
Aside from the fact that there is no relationship between NEET and what this
extension does, this extension basically allows you to...

1. search for a term in an existing incognito window.
    * Tab will open to the right of the current active tab in that window.
    * New incognito window will be created if no incognito window is found.
    * You can use the omnibox's `i` keyword. The advantage of this is that you
      get the fancy Google suggestion while not dirtying your search history.
    * These features were inspired by [Search Incognito][1]
        - However, this extension only _creates_ a new window, and doesn't
          open searches in a currently-existing incognito window.
2. reopen a normal-window tab in an incognito window
    * Same opening behavior as item 1.
    * This feature was inspired by [Incognito This Tab][2], but this extension
      had the same problem as Search Incognito.

In short, you can think of it as a mashup of those two plugins, with
modifications to meet my needs. The source code was written from scratch.

## Install
1. Clone the repository
2. Open Chrome/Chomium and go to extensions
3. Check "Developer Mode"
4. Select "Load unpacked extension"
5. Select the directory that you cloned
6. You need to check "Allow in incognito" in order for this extension to work

## Limitations
* The context menu (a.k.a. right click menu) does not update real-time.
    - This is due to the specifications of the API for Chrome extensions. Most
      of the time, the title for the first tab in a window is used in the
      context menu, but it may not always be correct.
* You can _see_ the Google suggestions, but not _select_ them.

## TODO
* Remove context menu in incognito window (since you can use the default
  'Search Google for ...')
* Configurable query URL, tab index
* Simple save/load text files with URLs

## Icon
The "Gardener" icon from https://icons8.com/android-L/ --distributed under
Creative Commons license (Attribution 3.0 Unported)-- is used for this
extension. Thanks!

## License
For the icons, see the link above. MIT License is adopted for the other source
code parts of the extension.

## Author
Naoki Mizuno

[1]: http://searchincognito.blogspot.com/
[2]: http://browsernative.com/extensions/