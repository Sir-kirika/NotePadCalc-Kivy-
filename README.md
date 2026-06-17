# Notepad Calculator

A KivyMD-based notes application that combines note-taking with inline calculator functionality.
To run the app open "dist" folder and run main.exe

## Features

- Create, edit, and delete notes
- Automatic JSON-based note storage
- Auto-save while typing
- Timestamp tracking (`YYYY-MM-DD HH:MM:SS`)
- Sort notes by last updated date
- Light and Dark theme support
- Undo / Redo editing
- Inline arithmetic evaluation
- Variable declarations and reuse
- RecycleView-based note list
- Settings panel and About screen

## Examples

### Basic Arithmetic

```text
3+3
```

Result:

```text
3+3 = 6
```

### Variables

```text
c=5
m=3
x=20
y=m*x+c
```

Result:

```text
c=5
m=3
x=20
y=m*x+c=65
```

### Shopping List

```text
milk=10*100
eggs=30*50
bread=2*100
```

Result:

```text
milk=10*100=1000
eggs=30*50=1500
bread=2*100=200
```

## Storage

Notes are stored in:

```text
notes_store2.json
```

Each note is saved as:

```json
{
  "note_id": {
    "title": "Example",
    "content": "Note content",
    "last_updated": "2025-06-27 14:23:45"
  }
}
```

## Main Components

### MainScreen

- Displays saved notes
- Sorting controls
- Settings panel
- Navigation to editor and about screens

### EditorScreen

- Note editing
- Auto-save
- Inline expression evaluation
- Variable support
- Undo / Redo

### AboutScreen

- Application information
- Usage examples

### NoteRow

Custom RecycleView item displaying:

- Note title
- Last updated timestamp
- Delete action

## Dependencies

```bash
pip install kivy
pip install kivymd
```

## Run

```bash
python main.py
```

## Future Improvements

- License manager
- Search notes
- Export/import notes
- Markdown support
- Syntax highlighting
- Cloud synchronization
