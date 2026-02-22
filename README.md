# React Visual Text Editor

A browser-based text editor featuring an interactive virtual keyboard, bidirectional language support (Hebrew/English), and comprehensive text styling capabilities — all built with React and powered by localStorage for document persistence.

> ⚠️ This is a demonstration project. The authentication system uses localStorage and is not suitable for production use with sensitive data.

## Features

* **Virtual Keyboard** — On-screen keyboard with multiple layouts (letters, uppercase, numbers, symbols, emojis)
* **Bilingual Support** — Seamless Hebrew and English input with automatic RTL/LTR text direction
* **Text Styling** — Real-time color, font family, and font size customization
* **Document Management** — Create, save, load, and manage multiple documents simultaneously
* **Search & Replace** — Find and replace characters across documents with visual highlighting
* **Undo Functionality** — Revert recent changes with action history tracking
* **User Authentication** — Basic login/signup system with localStorage-based session management
* **Multi-Document Workspace** — Work on several documents at once with active document switching

## Tech Stack

**Frontend:**
* React 19.2.0
* Vite (Build tool)
* CSS3
* ESLint

**Storage:**
* localStorage for user data and document persistence

## Project Structure
```
react-visual-text-editor/
├── src/
│   ├── components/
│   │   ├── DocumentEditor/    # Document management and display
│   │   │   ├── Files/          # Save/load functionality
│   │   │   ├── Screen/         # Text rendering area
│   │   │   ├── Document.jsx
│   │   │   └── DocumentEditor.jsx
│   │   ├── Keyboard/           # Virtual keyboard system
│   │   │   ├── ActionKeys.jsx  # Delete, search, replace, undo
│   │   │   ├── DesignKeys.jsx  # Styling controls
│   │   │   ├── LanguageKeys.jsx # Character input
│   │   │   └── Keyboard.jsx
│   │   ├── User/               # Authentication
│   │   │   ├── LogInAndSignUp.jsx
│   │   │   └── User.jsx
│   │   └── Button.jsx
│   ├── App.jsx
│   └── main.jsx
├── index.html
├── package.json
└── vite.config.js
```

## Getting Started

### Prerequisites
* Node.js (v16 or higher)
* npm

### Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd react-visual-text-editor
```

2. Install dependencies:
```bash
npm install
```

### Running the Application

1. Start the development server:
```bash
npm run dev
```

2. Open `http://localhost:5173` in your browser

### Build for Production

```bash
# Build the application
npm run build

# Preview production build
npm run preview

# Run ESLint
npm run lint
```

## Usage

1. **Authentication** — Register a new account or login with existing credentials
2. **Create Document** — Click "Open a new editing screen" to start a new document
3. **Input Text** — Use the virtual keyboard to type in Hebrew, English, numbers, symbols, or emojis
4. **Style Text** — Customize color, font, and size for new text or apply changes to all existing text
5. **Search & Replace** — Find specific characters and replace them throughout the document
6. **Save Document** — Save your work with a custom filename
7. **Load Document** — Access previously saved documents from the file menu
8. **Multi-Document** — Switch between multiple open documents by clicking on them

## Key Features Breakdown

### Virtual Keyboard
- 6 input modes: English lowercase, uppercase, Hebrew, digits, symbols, emojis
- Real-time language switching with automatic text direction adjustment
- Space, Enter, and Delete functionality

### Text Styling
- **Colors:** Black, Green, Red, Pink, Blue
- **Fonts:** Arial, Helvetica, Verdana, Tahoma
- **Sizes:** 12px, 16px, 20px, 24px
- Apply styles to new text or retroactively to all text

### Document Operations
- Delete last character, delete last word, or clear all content
- Undo last action with history tracking
- Save documents with custom names
- Load and switch between saved documents

## Author

Developed as part of a full-stack development course.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
