# SP-12 MIDI Disk

SP-12 MIDI Disk is a disk drive for the E-mu SP-12 drum machine that runs in your web browser. The SP-12 saves its sounds
and sequences to the page over MIDI, with its own Cassette/Disk 3 functions, and loads them back the same way. The page
keeps two disks, like a sound floppy and a sequence floppy, and saves each one to a file on your computer or phone. It
also lists what a disk holds, plays the pads, segments and songs, edits segments and songs, and turns WAV and other
sound files into SP-12 sounds. Everything is in one web page; it sends nothing anywhere.

**Open it here: <https://sirkrisbo.github.io/SP12-MIDI-Disk/>**

## What you need

- An SP-12 with stock v2.6 firmware, or SP-12 Rambo 3.1 or later.
- Chrome or Edge on Windows, Mac, Linux or Android. Safari, and every browser on iPhone or iPad, have no Web MIDI.
- A USB MIDI interface.
- Two MIDI cables, one each way.

## Your first save, in 5 steps

1. **Cables:** the SP-12's MIDI OUT to your interface's IN, and the interface's OUT to the SP-12's MIDI IN.
2. **Connect:** open the page and press **CONNECT**. When the browser asks, allow MIDI devices, including *control and
   reprogram* (that is SysEx; the SP-12 needs it).
3. **Ports:** choose **MIDI In** (the port the SP-12's MIDI OUT goes to) and **MIDI Out**. The screen says
   **Waiting for SP12**.
4. **On the SP-12:** press **CASSETTE/DISK**, then **3**, then **2** (Save Sounds; **1** is Save Sequences). At
   "Insert Disk / and Press Enter" press **ENTER**. A full 20 seconds of sounds takes about 5 minutes.
5. **Keep it:** when the screen says **Saved Sounds**, press **SAVE** to save the disk as a `.sp12` file.

To send it back, LOAD the file and use Load Sounds (Cassette/Disk 3 5) or Load Sequences (3 3) on the SP-12. **HELP** on the
page explains everything else.

On Windows only one program can use a MIDI port at a time, so close DAWs and other MIDI programs first. On Android, open
the page from its https address above, not from a file.

## What it can do

- Answers every Cassette/Disk 3 function: Save, Load and Verify Sounds and Sequences, Load Sound #, Load Segment #,
  Catalog and Format.
- Keeps a SOUND disk and a SEQ disk in the browser, and saves each one to a file.
- Repairs the block numbers that some MIDI interfaces damage.
- **CATALOG:** plays the pads (also from the computer keyboard), and plays segments and songs as the SP-12 plays them,
  with TEMPO and TAP.
- **EDIT:** notes (add, move, delete, level, tuning or decay, several at once), a segment's time signature, swing and
  length, song steps of every kind, new, copied and deleted segments and songs, and UNDO / REDO.
- **Sound tools:** REC (sound files become SP-12 sounds: mono, 12 bits, 26,042 Hz), DOWNLOAD (WAV, or several as a ZIP),
  DELETE, DECAY, CH, dragging pads to move or swap them, and V2.6 LOCK (keeps a sound disk that stock v2.6 can load).
- **LOG:** every MIDI message both ways, ready to copy or download.

## Files

- **Opens:** `.sp12` (this page's own disk files), `.sp12disk`, the SP12 app's `.SPLB12` (sounds) and `.SPLQ12`
  (sequences), and the SP12 tool's `.SP12`. The page tells them apart by their content.
- **Saves:** disks as `.sp12`; sounds as `.wav` (several at once as one `.zip`).

## Credits and licence

The SP-12, its sounds' tables and its file formats are E-mu Systems' work; SP-12 and E-mu are trademarks of their
respective owners. Not affiliated with E-mu Systems.

© 2026 Kris O'Sullivan. SP-12 MIDI Disk is free software under the GNU General Public License, version 3 or (at your
option) any later version, with no warranty: see [LICENSE](LICENSE). The small tables and the sequence-file tail that
the page copies from the SP-12's ROMs and its IC88 PROM are the work of E-mu Systems, their copyright holder; they are
included only for compatibility and are not covered by this licence.
