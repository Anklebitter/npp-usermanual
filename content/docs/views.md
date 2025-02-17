---
title: Views
weight: 105
---

The View menu controls the look of the Notepad++, including how Notepad++ and the Windows operating system interact, what features and panels are active inside Notepad++, and whether there are one or two Views (visible files) active at the same time.

Many of the entries in the View menu act as settings or toggles, to enable or disable showing some feature.  Some of these are remembered every time you run Notepad++, and others are just active for the single session and not remembered -- those that are remembered will be marked as [↗](#remembered-settings "Remembered Setting").

## Application Views

Choosing **Always On Top** will make the Windows OS always keep Notepad++ on top of of other windows, even when you give other windows focus.  If this is blocking another window you need access to, you can drag one of the windows, or you can disable **Always on Top** mode and then switch to the blocked window.

Choosing **Toggle Full-Screen Mode** will cause Notepad++ to take up the full screen, and the title bar and menu bar and tool bar will _not_ be visible.  The menu bar will no longer be accessible through Alt-key accelerators, so the Notepad++ menu system cannot be used to get out of this mode; however, there is a little + sign in a box  (`⊞`) in the upper right which can be used to exit the full-screen mode; alternatively, use the current keyboard shortcut for this toggle action (the default shortcut is `F11`), or close Notepad++ with `Alt+F4` or other Windows OS methods of closing applications and then restart Notepad++ (which will come up in normal view again). (To clarify: though Alt-accelerators will not show the menu bar or access the menu bar menus, action shortcuts defined through Shortcut Mapper will still work, even if they use the Alt key.)

Choosing **Post-It** will get rid of the title bar, menu bar, and tool bar (similar to full-screen mode), but it will maintain the same window size as Notepad++ previously took up, rather than enlarging to take up the whole screen.  This mode will also hide the tab bar, so you can focus on working on the single visible tab, though you can still use the tab-switching shortcuts to choose another tab. Like full-screen mode, Post-It mode has the `⊞` in the upper right of the window for leaving this mode, or you can use the shortcut (the default shortcut is `F12`) or exit Notepad++ and restart.

Choosing **Distraction Free Mode** (new to v8.0.0) will combine full-screen mode with Post-It mode, so it will go full screen, and will hide the title bar, menu bar, tool bar, and tab bar; it will also add wide margins within the edit menu, so the text doesn't go so wide across the full-screen window.

## View Current File In...

The **View Current File In...** sub-menu will launch the current file in a standard web browser (Firefox, Chrome, Edge, or IE).  This works best for HTML or other web documents, but text, XML, and other file types can also be viewed in the browser.

## Show Symbol

The **Show Symbol**[↗](#remembered-settings "Remembered Setting") sub-menu will affect whether certain characters are rendered with special glyphs so that they can easily be seen or identified in the editor view, and whether certain tab and wrap guides will be visible.

There are three entries that are grouped together, which can affect the rendering of certain characters with alternate glyphs. Please note that while the characters may be displayed differently in Notepad++, the underlying file has the normal characters encoded per the current **Language** menu settings.  Only one of these three options can be selected (indicated with a check mark `✓`) at a given time, and selecting a new option will un-select the old.  If you want none of these symbol options, click on the option that is currently selected and it will be turned off (and none of the options will have the check mark `✓`).

* **Show Whitespace and TAB**: When selected, the space character will show as a [colored](../preferences/#global-styles "Style Configurator > Global Styles > White Space Symbol") dot `·`, and the tab as a colored arrow `→` that expands to fill the width of the tab.
* **Show End of Line**: When selected, the carriage return character will be rendered as `CR` in a small box, the line feed character as `LF`, and a Windows two-character line ending as `CRLF`.  (The boxed characters are colored as "reverse text", so the active [Global Styles > Default > Foreground colour](../preferences/#global-styles "see Style Configurator > Global Styles") will fill in the box and the active [Global Styles > Default > Background colour](../preferences/#global-styles "see Style Configurator > Global Styles") will define the boxed-letter's foreground color.)
* **Show All Characters**: When selected, this is effectively both **Show Whitespace and TAB** and **Show End of Line** at the same time.

When the **Show Indent Guide** entry is selected, a [colored](../preferences/#global-styles "Style Configurator > Global Styles > Indent Guideline Style") dotted vertical line `⸽` will show where each of the tab stops are located if there are enough tabs or spaces at the start of a given line to go beyond a tab stop (as defined by the [per-language Tab settings](../preferences/#language)).

When the **Show Wrap Symbol** entry is selected and **Word Wrap** is also enabled, there will be a little [colored](../preferences/#global-styles "Style Configurator > Global Styles > White Space Symbol") arrow `↲` on the far edge of the current line if that line has been wrapped.

## Zoom

The **Zoom** sub-menu will allow you to **Zoom In** (enlarge the text), **Zoom Out** (shrink the text), or **Restore Default Zoom** (which will change the text size back to default settings).  These actions all act only on the current View, so if you have two Views visible, only one will be affected.  Zooming can also be accomplished by holding down the `Ctrl` key and using the mouse wheel to go up (enlarge) or down (shrink).

## Move / Clone

The **Move/Clone Current Document** submenu will allow you to affect where the current document is viewed.

If you **Move to Other View**, the current file will be moved from one View to the other.  If there is currently only one View visible, this command will make the second View visible -- it may be to the right, below, to the left, or above the original View, depending on where the second view was last placed.  To change the arrangement of the Views, right-click on the dotted bar between the two Views, and **Rotate Right** or **Rotate Left**, which will change the orientation from side-to-side to above-and-below.  You can also accomplish this **Move to Other View** by dragging the tab from one View's tab-bar to the other, or right clicking on the tab and selecting the **Move to Other View** from that menu.

If you **Clone to Other View**, the current file will be visible in both Views at the same time.

If the current file is currently not modified (so no unsaved changes), you can also either **Move to New Instance** or **Clone to New Instance**, which will move the active file from this instance to a new instance of Notepad++, or make this file open in both the current Notepad++ and a new instance of Notepad++.  This will work to create a new instance of Notepad++ even if the [**Settings > Preferences > Multi-Instance**](../preferences/#multi-instance) is set to "mono-instance".

## Tab

The **Tab** sub-menu will allow you to navigate through the various open tabs of the active View.

The numbered entries will activate the _Nth_ tab. The **Next tab** and **Previous tab** actions will activate the next or previous tab in the list of tabs (wrapping).

The **Move Tab Forward** and **Move Tab Backward** will change the current file's position in the tab list one slot at a time, forward or backward.  The tab order can also be changed by dragging the tabs to the new position in the tab-bar.

## Wrapping

The **Word wrap**[↗](#remembered-settings "Remembered Setting") entry will toggle whether or not long lines will be wrapped in the display, and affects all tabs in both Views.

When this toggle is not set, you will have to use the horizontal scroll bar to the see the whole current line; when the toggle is set, the line will _appear_ to wrap at the end of your current editor view width, but there will be no newline (so if you open the same text file in a different editor, or a different computer's Notepad++ with different settings, it won't wrap at that character).  **Note**: The line wraps on whole-word increments when possible, but if the current word is longer than the entire line-length, it _will_ wrap in the middle of the word.

## Focus View

The **Focus on Another View** action will swap your active focus between the two Views (if both Views are visible).

## Hiding Lines

The **Hide Lines** action will hide the active line or selected lines, and place symbols in the margin to allow you to unhide those lines.  The text is still there when you save, it will just temporarily not be visible while you are editing (until you unhide the text, or re-start Notepad++).

## Folding

There are a group of folding-related commands, which will allow the folding or unfolding of blocks of text based on the current syntax highlighter lexer for a [programming language](../programing-languages/) or [User Defined Langauge](../user-defined-language-system/), and the folding rules defined in that lexer or UDL.  (To "fold" the text means to temporarily hide a block of text; to "unfold" the text means to reveal that block of text again.)  If folding blocks are nested (contained inside other folding blocks), the outermost block is level 1, the block immediately inside that is level 2, and so on.  (Folding is _not_ remembered from one run to the next, nor is it saved in the automatic or manually-saved session file.)

* **Fold All** and **Unfold All** will collapse or reveal all fold blocks in the current file.
* **Collapse Current Level** and **Uncollapse Current Level** will collapse or reveal the block based on the caret position
* The entries in the **Collapse Level** and **Uncollapse Level** sub-menus will collapse or reveal every level _N_ block in the active file.

## File Summary

The **Summary...** action opens a small dialog that lists information about the current file, including the full path, the various file timestamps, and the length in bytes, characters (excluding line endings), number of words, and number of lines.

## Panels

There are a variety of builtin "panels" (sub-windows) that can be used in Notepad++.  These panels can be "docked" (so they appear as part of the main Notepad++ application window) on either the right, left, top, or bottom edges; or they can be made to "float", so they appear as a separate independent window.  Docked panels can be moved easily to another edge, or to floating, by clicking on the panel's title and dragging it to the new location.

The **Project Panels**[↗](#remembered-settings "Remembered Setting") sub-menu entries will toggle the display of each of the three [Project Panels](../session/#project-panels)

The **Folder as Workspace**[↗](#remembered-settings "Remembered Setting") entry will toggle the display of the [Folder as Workspace](../session/#folder-as-workspace) panel

The **Document Map**[↗](#remembered-settings "Remembered Setting") item will toggle the display of the Document Map panel, which shows a copy of the file in a tiny font, with a highlighted range to indicate which section of the current file is visible in the editor.

The **Document List**[↗](#remembered-settings "Remembered Setting") toggle will display the Document List panel, which lists all the open documents and allows easily switching between them.  (Prior to v8.1.3, the panel was known as the **Doc Switcher** panel and controlled through the [General preferences](../preferences/#general), but that name was confused with the Document Switcher `Ctrl+TAB` settings in [MISC preferences](../preferences/#misc).)

The **Function List**[↗](#remembered-settings "Remembered Setting") toggle will display the [Function List](../function-list/) panel, which lists the functions, methods, and classes in the current file, and allows easy navigation to those sections of the file by double-clicking in the Function List panel.  (The "functions, methods, and classes" are programming terms, but the feature can also be used for listing headings or sections of other structured files, or through [config files](config-files/#function-list), can be made to match anything else that you choose to match for indicating "sections" of your text, whatever that happens to mean to you.)

## Synchronized Scrolling

The **Synchronize Vertical Scrolling** and **Synchronize Horizontal Scrolling** will allow the two Views to be locked together, so that if you scroll in one view, the other view will also scroll in the same direction.  This is useful for comparing two files or comparing two parts of the same file at the same time.  By cloning the same file in both views, and locking them at different locations, you can also use Notepad++ like a "newspaper reader", showing two columns of text simultaneously.

## Text Direction

The **Text Direction RTL** and **Text Direction LTR** are useful for text that needs to be written Right to Left (RTL), or to switch a file back to Left to Right (LTR) viewing after it had previously been set to RTL.  This is especially beneficial for editing Hebrew and Arabic scripts, and any other writing systems that are read Right to Left.

## Live File Monitoring

The **Monitoring (tail -f)** toggle will have Notepad++ watch the current file for live changes in the background, and will update the display as it notices the underlying file change.  This puts the file in a de-facto read-only mode, so that the file cannot be edited in Notepad++ as it's being changed by whatever task is changing the file in the background.  This is useful for watching a log file as new lines are added to the end, and is inspired by the Linux command `tail -f` which performs a similar function, hence the entry's name.

The Monitoring feature is also similar to the File Status Auto-Detection settings in the [MISC preferences](../preferences/#misc), which influences whether Notepad++ will detect external changes in the open file(s) even without Monitoring enabled.

## Remembered Settings

[↗](#remembered-settings "Remembered Setting"): These indicated settings are remembered from one run of Notepad++ to the next.
