# Nullboard

Nullboard is a minimalist take on a kanban board / a task list manager, designed to be compact, readable and quick in use.

https://nullboard.io/preview

![Nullboard](images/nullboard-example-alt.png)

The name also happens to abbreviate to [NB](https://en.wikipedia.org/wiki/Nota_bene), which is a nice touch.

---

## Beschreibung (Deutsch)

Nullboard ist ein minimalistisches Kanban-Board und Aufgabenverwaltungs-Tool, das auf Kompaktheit, Lesbarkeit und schnelle Bedienung ausgelegt ist.

Das Projekt besteht aus einer einzigen HTML-Datei und läuft vollständig im Browser – ohne Server, ohne Cloud, ohne Registrierung. Alle Daten werden lokal im Browser gespeichert.

### Schnellstart

1. `nullboard.html` im Browser öffnen (Doppelklick auf die Datei genügt)
2. Über das Menü oben links ein neues Board anlegen
3. Listen und Notizen per Klick hinzufügen und bearbeiten

---

## Dead simple

* Single-page web app – just one HTML file, jQuery and a set of web fonts.
* Can be used completely offline. In fact, it's designed exactly with this use in mind.

## Locally stored

* All data is stored locally using [localStorage](https://developer.mozilla.org/en/docs/Web/API/Window/localStorage).
* The data can be exported to or imported from a plain text file in a simple JSON format.
* The data can also be automatically backed up to a local disk with the help of:
  * [Nullboard Agent](https://nullboard.io/backups) – a native Windows app
  * [Nullboard Agent Express Port](https://github.com/justinpchang/nullboard-agent-express) – an express.js-based portable app
  * [nbagent](https://github.com/luismedel/nbagent) – a version for Unix systems, in Python

## UI & UX

Everything is editable in place, all changes are saved automatically and the last 50 revisions are kept for undo/redo:

![In-place editing](images/nullboard-inplace-editing.gif)

New notes can be quickly added directly where they are needed, e.g. before or after existing notes:

![Ctrl-add note](images/nullboard-ctrl-add-note.gif)

Notes can also be dragged around, including to and from other lists:

![Drag-n-drop](images/nullboard-drag-n-drop.gif)

Nearly all controls are hidden by default to reduce visual clutter to its minimum:

![Hidden controls](images/nullboard-hidden-controls.gif)

Longer notes can be collapsed to show just the first line, for an even more compact view:

![Collapsed notes](images/nullboard-collapsed-notes.gif)

The default font is [Barlow](https://tribby.com/fonts/barlow/) – it's both narrow *and* still very legible.

![Barlow specimen](images/barlow-specimen.png)

Notes can also be set to look a bit different. This is useful for partitioning lists into sections:

![Raw notes](images/nullboard-raw-notes.gif)

Links starting with `https://` and `http://` are recognized. They will "pulse" on mouse hover and can be opened via the right-click menu.

![Links on hover](images/nullboard-links-on-hover.gif)

Pressing CapsLock will highlight all links and make them left-clickable.

![Links reveal](images/nullboard-links-reveal.gif)

Lists can be moved around as well:

![List swapping](images/nullboard-list-swap.gif)

The font can be changed; its size and line height can be adjusted:

![Theme and zoom](images/nullboard-ui-preferences.gif)

The color theme can be inverted:

![Dark theme](images/nullboard-dark-theme.gif)

Also:

* Support for multiple boards with near-instant switching
* Undo/redo for 50 revisions per board (configurable in the code)
* Keyboard shortcuts, including Tab'ing through notes

## Caveats

* Written for desktop and keyboard/mouse use
* Essentially untested on mobile devices and against tap/touch input
* Works in Firefox, Chrome, Safari and Edge

## Dependencies

* [jQuery 3.6.0](https://jquery.com/) – bundled locally in `extras/`
* Web fonts (Barlow, IBM Plex Sans, Open Sans, Maven Pro) – bundled locally in `extras/`

No build step, no package manager, no server required.

## Dockerized version

See [this fork](https://github.com/rsoper/nullboard).

## Background

Nullboard is something that handles ToDo lists in the way that works really well. For *me* that is.

Tried a lot of options, some were almost *it*, but none was 100%.

**Trello** wasn't bad, but never was comfortable with the idea of storing my data in cloud without any actual need.

**Wekan** looked promising, but ultimately too heavy and had no offline usage support or a local storage option.

**Things** was beautiful, but not the right tool for the job.

**Inkscape** – I kid you not – with a laundry list of text items was actually OK, but didn't scale well.

Ditto for plain **text files**.

Pieces of **paper** were almost there, but rearranging items can be quite a hassle.

So finally got annoyed enough to sit down and write exactly what I wanted.

And, voilà, Nullboard came out  =>  https://nullboard.io/preview

## License

The [2-clause BSD license](https://opensource.org/licenses/BSD-2-Clause/) with the [Commons Clause](https://commonsclause.com/).

That is, you can use, change and re-distribute it for as long as you don't try and sell it.

## Updates

Primary feed is through [@nullboard](https://x.com/nullboard) on X (formerly Twitter).

The changelog is here => https://nullboard.io/changes
