# RDF_Project

## Overview

RDF_Project is a multi-language code editor and project manager built with PyQt6 and QScintilla, designed for rapid development and validation of RDF-based web projects. It features syntax highlighting, auto-completion, project navigation, live mobile preview, terminal output, and rule-based validation for files and projects. The editor is tailored for HTML, CSS, JavaScript, PHP, Python, and JSON, and integrates with XAMPP for local server previews.

---

## Features

- **Multi-language Syntax Highlighting**: Supports HTML, CSS, JavaScript, PHP, Python, and JSON.
- **Auto-completion**: Context-aware suggestions for code completion.
- **Project Explorer**: Browse, open, and create files within your workspace.
- **Tabbed Editing**: Edit multiple files in tabs.
- **Integrated Terminal**: Output and feedback directly in the editor.
- **Mobile View Preview**: Live preview of web files in a simulated mobile device frame.
- **Rule-based Validation**: Validate files and projects against custom rules.
- **Dark Theme Support**: Toggle dark mode for comfortable coding.
- **Search & Navigation**: Find words, go to line, and highlight text.
- **XAMPP Integration**: Automatically starts XAMPP Control Panel for local server previews.

---

## Installation

### Prerequisites

- **Python 3.8+**
- **PyQt6**
- **QScintilla**
- **psutil**
- **chardet**
- **PyQtWebEngine** (for mobile preview)
- **XAMPP** (for local server preview)

### Setup

1. **Clone the repository:**
    ```sh
    git clone https://github.com/yourusername/RDF_Project.git
    cd RDF_Project
    ```

2. **Install dependencies:**
    ```sh
    pip install PyQt6 QScintilla psutil chardet PyQt6-WebEngine
    ```

3. **Ensure XAMPP is installed at `C:\xampp` (or update the path in `main.py`).**

---

## Usage

1. **Run the application:**
    ```sh
    python main.py
    ```

2. **Features:**
    - **Open/Create Projects:** Use the Project menu to open or create new projects.
    - **Edit Files:** Double-click files in the project explorer to open in tabs.
    - **Live Preview:** Mobile view shows a live preview of your web files.
    - **Terminal:** View output and feedback in the integrated terminal.
    - **Validation:** Use the Validation menu to validate files or the entire project.
    - **Search:** Press `Ctrl+F` to search within the current file.
    - **Go to Line:** Press `Ctrl+G` to jump to a specific line.

---

## Project Structure

```
RDF_Project/
│
├── main.py                # Application entry point
├── code_editor.py         # Main code editor window and logic
├── Qscintilla.py          # QScintilla-based editor UI
├── syntax_highlighter.py  # Syntax highlighting rules
├── autocompleter.py       # Auto-completion logic
├── terminal_widget.py     # Integrated terminal widget
├── mobile_view.py         # Mobile device preview widget
├── theme.py               # Dark theme palette
├── images/                # Icons and images for UI
├── rules/                 # Rule files for validation
│   ├── rules_ui.json
│   ├── rules_json.json
│   ├── rules_bw.json
│   ├── rules_bvo.json
│   └── rules_action.json
└── ...
```

---

## Configuration

- **XAMPP Path:** Update the path in `main.py` if your XAMPP installation is not at `C:\xampp`.
- **Rules:** Place your validation rule files in the `rules/` directory.
- **Images:** UI icons and preview images should be placed in the `images/` directory.

---

## Testing

Unit tests can be added in a `tests/` directory.  
To run tests (if available):

```sh
pytest tests/
```

---

## Contributing

1. Fork the repository.
2. Create your feature branch (`git checkout -b feature/your-feature`).
3. Commit your changes (`git commit -am 'Add new feature'`).
4. Push to the branch (`git push origin feature/your-feature`).
5. Create a Pull Request.

---

## License

This project is licensed under the MIT License. See `LICENSE` for details.

---

## Contact

For questions or feedback, please contact [rahulrdhamdhere@gmail.com].
