# CLI Quiz App

A small Node.js command-line quiz application that runs multiple-choice questions from a JSON file. This project is a simple, modular CLI useful as a learning example or as a foundation for a more advanced quiz tool.

## Features

- Run quizzes from a structured JSON file
- Colorized terminal output for clear feedback
- Modular code (entry point, quiz logic, input handling, color helpers)
- Easy to customize and extend

## Prerequisites

- Node.js (v12+ recommended)
- npm (for dependency management)

## Installation

1. Clone the repository:

   git clone <repo-url>
   cd <repo-directory>

2. Install dependencies (if package.json is present):

   npm install

## Running the App

Start the quiz using Node.js:

   node index.js

Or run via npm if a start script exists:

   npm start

Follow the on-screen prompts to answer questions. The app will display a final score at the end.

## File Structure (overview)

- index.js        — Application entry point (starts the quiz)
- quiz.js         — Quiz flow, question selection, and scoring
- input.js        — Utilities for reading user input and prompts
- colors.js       — Terminal color/styling helpers
- questions.json  — Question bank (JSON array of question objects)
- package.json    — Metadata and npm scripts (may or may not exist)

There may be alternate copies (e.g., files prefixed with `_` or download artifacts). Keep the canonical files (without `_`) as the active source.

## Question Format

Each question in questions.json should follow a simple structure. Example:

{
  "id": 1,
  "question": "What is the capital of France?",
  "options": ["Paris", "Rome", "Berlin", "Madrid"],
  "answer": 0
}

- `answer` is typically the index of the correct option (0-based).

## Customization

- Edit questions.json to change or add questions.
- Modify colors.js to change styling.
- Update input.js for different prompt behavior or validation.
- Extend quiz.js to add categories, timed questions, or scoring rules.

## Troubleshooting

- If you see module errors, run `npm install` and ensure package.json lists required packages.
- If the app loads a different questions file, check index.js for the filename used and consolidate duplicates.

## Contributing

1. Fork the repo
2. Create a feature branch
3. Make changes and open a pull request

Please include clear commit messages and small focused changes.

## License

Choose and add an appropriate license (e.g., MIT). If a LICENSE file already exists, follow that.

---

If you want, I can now:

- Inspect the repository files and update this README with exact scripts/dependencies and examples
- Clean up duplicate or binary artifacts (I can recommend which files to remove)

Tell me how you'd like to proceed.