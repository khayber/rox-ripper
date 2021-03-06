#Features#

  * CDDB access
  * Editable track, title, genre, etc., even after CDDB fetching.
  * Simultaneous Rip and Encode
  * Uses cdda2wav and lame/oggenc to do the dirty work.

![http://rox-ripper.googlecode.com/files/ripper.png](http://rox-ripper.googlecode.com/files/ripper.png)

#Releases#
007 (24-Oct-2006)

  * Rewrite options and processors to allow other rip/encoders to be used (other than cdda2wav, lame and oggenc)
  * Add options to keep WAV files and not Encode (suggested by Jonatan Liljedahl)
  * Add Album Cover art support (based on idea and code from Stephen Watson)
  * Change UI to use Progress bars in status area (requires gtk 2.6+)
  * Configurable Directory and Filename patterns (e.g. Track Number, Artist, etc.)
  * Bunches of general fixes and stuff :)

006 (13-Sep-2006)

  * Remove Threads usage (using ROX-Lib's tasks module)
  * Modularize the UI code

005 (Skipped)
004 (15-May-2004)

  * Add a Menu
  * Italian translation from Yuri Bongiorno
  * New Icon (SVG, I did it myself from some Gorilla icons)

09-Apr-2004 (003)

  * Add OGG support
  * Add Extended Attribute support for tag info (in addition to normal mp3/ogg tags)

22-Feb-2004 (002)

  * Croak with a specific message if thread support not present.
  * Added Eject After Ripping option.
  * Improve Option tooltips
  * Moved socket timeout code to PyCDDB and don't fail if python < 2.3.
  * Changed Genre entry to a !ComboBox and pulled in genre list from ID3.py/!MusicBox.
  * Removed borders to look better with openbox and other WMs that do not have borders on all sides of windows.
  * Auto resize columns after getting/editing track names.
  * Fix CD change and update track info logic. Should be really solid now.
  * Fix off by one error on track times. (first two songs always had the same time)
  * Don't return empty track list if cddb query fails. Use Track# instead.
  * Fix race condition between ripping and encoding threads when aborting (Stop).
  * Prepared for translations.
