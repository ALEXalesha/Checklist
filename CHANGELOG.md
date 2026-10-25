# Changelog

What changed for the user in each release. The full text of each release, in English and
Russian, is on the [releases page](https://github.com/ALEXalesha/Checklist/releases).

## 2.1.0 - 2026-09-24 - The window opens where and how large it was closed, maximized too

The geometry is saved when the window closes and restored at the next start. If the saved value is damaged, or the window's title bar would not be on any screen (a monitor has been unplugged), the window opens at the default size instead.

## 2.0.0 - 2026-09-22

The window was rewritten from Tkinter to Qt (PySide6).

**Why:** with a long list of expanded notes, Tk re-wrapped every note on each resize step and the window visibly lagged while being dragged. The Qt version holds one 60 Hz frame (16 ms) per resize step with 200 expanded rows, and that budget is now a test.

**What is new in 2.0**

- Notes on items: multi-line, shown under the row in grey italics, expandable with the mouse or `→` / `←`.
- Themes: follow Windows, or force light or dark; the choice is remembered and file dialogs follow it too.
- Windows 11 look: rounded menus, fields and buttons.
- Every menu action has a shortcut, and the `Alt` ones work in the Russian keyboard layout as well.
- Undo and redo in the note panel.
