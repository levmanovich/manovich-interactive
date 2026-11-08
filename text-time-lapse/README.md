# Text Time-lapse

# Guide

Nov 7, 2026 · @Lev Manovich

**Everything runs in your browser. Your files are read on your own computer and are never uploaded anywhere.**

## What it does

Text Time-lapse shows how a text changed across its saved versions. Load versions of your text you were saving while working, and the tool creates a visualization of your writing process. You can step through versions and see which text parts were added, edited and removed in each. You can see the result on one page, as one small page per version or as a 3D stack of pages, and you can animate it to watch the text being written and revised.

<p>
  <img src="screenshots/cover.webp" alt="Text Time-lapse: visualize your writing process" width="290">
  <img src="screenshots/changes.webp" alt="What was added, edited and removed in each version" width="290">
  <img src="screenshots/final-text.webp" alt="The final text, colored by the version each word was written in" width="290">
</p>

## Preparing your files

Put the versions of one text in a folder, then choose the folder, choose the files, or drag them onto the page. You need at least two versions.

**Formats:** plain text (.txt), Markdown (.md) and Word (.docx). Other files in the folder are skipped, as are hidden files and Word's temporary `~$` files. To use Apple Pages or Google Docs files, export them to .docx or .txt first.

**Order:** the versions are sorted by file name. For example, text\_01.txt is taken as the first version, text\_02.txt as the second, and so on. Numbers are sorted as numbers, so 2 comes before 10. Name your files so that sorting A–Z gives the right order.

| Works | Does not sort correctly |
| --- | --- |
| essay v1.docx, essay v2.docx … essay v10.docx | final.docx, final 2.docx, final REALLY.docx |
| draft 1.txt, draft 2.txt … draft 12.txt | draft one.txt, draft two.txt |
| 2024-07-28 chapter.md, 2024-08-08 chapter.md | 28-07-2024 chapter.md (day first) |

**Dates:** the date shown for each version is the file's last-modified date. If the files were copied or downloaded together, they may all show the same date; the order still follows the names.

**Paragraphs:** each line of text counts as a paragraph. A short first line without a period is treated as the title, and short lines without a period as headings.

## Controls

The panel shows five rows: Files, Text view, Modes, Zoom and Animate. **Advanced ⌄** opens all the other settings: Color, Page and Coloring, and, when Revisions is chosen, the Revisions settings. **Help:** click **?** (top right) to turn on help mode. Then point at any control, or tap it on an iPad or phone, and a short explanation appears next to it; nothing changes while help mode is on. Click **?** again or press Esc to leave. On a laptop, resting the pointer on a control also shows its explanation.

**Screen size:** the page is sized so that all of it fits on your screen. On a laptop, or an iPad held sideways, the controls sit in a column on the left and the page on the right. **Hide controls** (top right) folds the controls into one thin bar with Play / Pause, Start and the three animations, so the page gets almost the whole screen; **Show controls** brings them back. On a phone the controls start hidden.

### Main controls

| Row | Controls | What they do |
| --- | --- | --- |
| Files | Choose a folder… / Choose files… | Load your versions. You can also drop files or a folder on the page. |
| Text view | Final text / All written / Deleted / Edited | Choose which words the page shows: the final text; everything ever written, with cut words crossed out; only what was removed; or only the rewrites. Each button shows its word count. |
| Modes | Text / Blocks / Pages / 3D view | Show the words as text, as colored bars (words that were later removed are pale bars), as one small page per version, or as a 3D stack of pages. The Pages button shows the number of versions, for example 10 pages. Click a small page to open it. In the 3D view, each page has its version number on the left. |
| Zoom | Slider / Large type / Whole page | Works in Text and Blocks, and in the Revisions player. Whole page shows the entire text in columns, so you see the overall pattern of colors; the page opens this way (1.0×). Large type shows about 10 readable lines on screen, in one long column that you scroll down. The slider sets any size in between, or smaller. |
| Color (Advanced) | Colors menu | Choose the colors of the versions: a color set that blends from the oldest version to the newest (Navy–magenta–orange, Sky–violet–vermilion), Soft hues (a calm color for each version), Bright hues (a clearly different color for each), Grays, or Custom… (your own three colors, and Mid to move the middle color). |
| Shape, Text, Paragraphs, Spacing (Advanced) | A4 / 4:5 / Square / 9:16 / 16:9; Left aligned (on/off); Indent / Line between; Line spacing | The shape of the page, left-aligned text (otherwise justified), paragraphs marked by an indent or by an empty line between them, and the space between lines. They apply to every view, including Pages, the 3D view and the player. |
| Coloring (Advanced) | Rewrites bold; Earlier versions in gray (on/off buttons) | Rewrites bold shows rewritten words in bold, in a darker shade of their version's color, and new words a little lighter. It works for every version at once, each in its own color. Earlier versions in gray turns earlier versions gray while an animation runs, so the version being added stands out. It also works when you click a version button: that version shows in color and the earlier ones in gray. |
| Blocks, Bars (Advanced) | Lightness / Saturation; Bar height / Word gap | Shown whenever Blocks is chosen in Modes. They shape the colored bars on the page and in the Revisions player. |
| Animate | Play / Pause, ⏮ Start; Revisions / Versions / Write | Revisions is chosen when the page opens, so you only need to press Play. Choose another animation and it starts at once; a Player row with its controls appears below (see Animations below). Play / Pause and ⏮ Start (back to the beginning) come first in the row and work for all three animations. In 3D view, this row also has Spacing and Transparency: the distance between pages and how see-through they are. |

**Below the controls** (above the page on an iPad held upright or a phone), a line names the text and gives its numbers: versions, dates, words written, words in the final version and words removed. The **Example** button at the start of this line brings back the example the page opens with: 16 saved versions of *Seven Worlds of Digital Art* by Lev Manovich (August–September 2026). Below the line, a strip of small buttons shows each version's color (v1, v2 …); point at one, or use help mode, to see its date and word count. Click one or more to show only their words. In 3D view, clicking a version builds the stack up to it.

### Animations

- **Revisions** shows each version's changes in turn: new words are written in, cut words are crossed out and disappear, and rewrites replace the old words. It opens the player, described below.
- **Versions** shows the chosen text view (for example Final text) one whole version at a time: v1, then v2, and so on. Its Player row has ◀ ▶ (previous or next version), Close-up (a magnifier you move with the mouse) and Time per version.
- **Write** shows all text ever written, word by word, version after version, with cut words crossed out. Its Player row has ◀ ▶ (jump to the start of the previous or next version), Close-up (a magnifier that follows the word being written while the animation plays; pause, then move the mouse to read other parts) and Words/s.

### Player

Pressing **Play** with Revisions chosen (or clicking Revisions) opens the player and plays it from an empty page; **Close player** takes you back. The Text view row is faded in the player. The Zoom row and Text / Blocks in Modes work in the player too: zoom in and scroll inside the page to read a passage. Play / Pause and ⏮ Start (back to the empty page) are in the Animate row. The **Player** row holds ◀ ▶ (previous or next version), Close-up (a magnifier you move with the mouse; it updates as the text changes), a position slider and Time per version (shared with Versions). Click a version button to play just that version; the space bar also plays and pauses. Its other settings are in **Advanced** (they appear there only when Revisions is chosen):

- **Timing:** Crossed out sets how long removed words stay visible, Pause how long the player stops after each version. **Pacing:** Big versions longer gives versions with more changes more time.
- **Order:** All at once, Reading order or Scattered. **Changes:** Text grows (the real length of each version; otherwise the final text stays in place, in gray); Keep cuts (cut words stay, crossed out; otherwise they disappear).
