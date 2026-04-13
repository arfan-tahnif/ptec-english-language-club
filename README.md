# PTEC VocabMaster – English Language Club

A single-file English vocabulary learning web app built with **HTML, CSS, and JavaScript**. It is designed to help learners browse vocabulary, search words, hear pronunciation, save useful words, take quizzes, track progress, test English level, and access study resources in one clean interface.

## Overview

This project is a lightweight browser-based English learning tool. It runs directly from a single HTML file, so there is no build step, no framework, and no installation required beyond opening the file in a modern browser.

The app focuses on practical learning features such as:

- vocabulary browsing
- search and pronunciation
- saved words
- quiz practice
- progress tracking
- English level testing
- PDF resource access
- dark mode support
- animated section transitions

## Main Features

### 1. Browse Vocabulary
- Browse a curated vocabulary collection.
- View each word with:
  - word
  - phonetic/pronunciation
  - part of speech
  - definition
  - example sentence
  - category
- Navigate through words with a card-based interface.

### 2. Search & Pronounce
- Search by:
  - word
  - meaning
  - example
  - category
- If a search term is not found, the app keeps the current word view unchanged and shows a helpful no-result message.
- Built-in pronunciation support uses the browser’s **Speech Synthesis API**.
- Includes dedicated **Search**, **Pronounce**, and **Clear** actions.

### 3. Category Filtering
The app includes category-based vocabulary organization, such as:
- All Words
- IELTS Essentials
- Academic Writing
- Common Idioms
- Daily Conversation

### 4. Saved Words
- Users can save useful vocabulary items.
- Saved words are stored locally in the browser.
- Helpful for revision and personal word collection building.

### 5. Quiz Section
- Users can take a multiple-choice vocabulary quiz.
- Tracks:
  - score
  - total answered
  - mistakes
  - quizzes taken
- Built for quick self-practice.

### 6. Progress Section
- Displays learning progress based on local storage.
- Tracks saved and learned activity over time.
- Gives users a simple view of their study journey.

### 7. English Level Test
- Includes a dedicated **Level Test** button.
- Provides a short English assessment with grammar, vocabulary, usage, speaking, and reading/writing style questions.
- Estimates user ability level from the test result.
- Useful as a quick self-check tool.

### 8. Resource Corner
- A dedicated **Resource** section for English-related PDF materials.
- Intended for grammar, vocabulary, pronunciation, and writing support resources.
- Appears only from the **Resource** button.
- Supports animated section reveal.

### 9. About Section
- Includes project or platform introduction content.
- Useful for describing the purpose of the app, club, course, or institution.

### 10. Dark Mode
- Supports light and dark appearance.
- Improved contrast for text visibility in dark mode.
- Theme preference is stored in the browser.

### 11. Smooth UI Animation
- Animated transitions are used for opening major sections.
- Resource, Saved, Quiz, Progress, and About sections use smooth reveal behavior.
- Other existing internal interactions remain unchanged.

## Technology Used

- **HTML5**
- **CSS3**
- **Vanilla JavaScript**
- **LocalStorage** for saving progress and theme
- **Speech Synthesis API** for pronunciation

## File Structure

This project is mainly designed as a **single HTML file**.

### Important script/data areas
Inside the HTML file, the main editable data blocks include:

- `words` → vocabulary dataset
- `categories` → category list
- `resourcePdfs` → PDF resource links and notes
- `englishLevelQuestions` → level test questions

### Local storage keys
The app uses browser local storage for persistence:

- `ptec-progress`
- `ptec-theme`

## How to Use

### Run locally
1. Download or keep the HTML file on your computer.
2. Open it in a modern browser such as Chrome, Edge, or Firefox.
3. Start using the app directly.

No server or installation is required.

## Customization Guide

### Update vocabulary words
Find the `words` array in the script section and add/edit objects like this:

```js
{
  id: 1,
  word: "Example",
  phonetic: "/ɪɡˈzɑːmpəl/",
  partOfSpeech: "noun",
  definition: "Something used to explain an idea.",
  example: "This is an example sentence.",
  category: "Daily Conversation"
}
```

### Update categories
Edit the `categories` array to add or rename categories.

### Add or replace PDF resources
Edit the `resourcePdfs` array:

```js
const resourcePdfs = [
  {
    title: "English Grammar Essentials",
    level: "Starter",
    note: "A useful starter resource for building grammar fundamentals.",
    url: "https://your-link-here.pdf"
  }
];
```

### Edit the English level test
Update the `englishLevelQuestions` array to:
- add more questions
- change skill labels
- adjust answer keys
- make the test easier or harder

### Change branding
You can customize:
- app title
- logo/favicon
- headings
- colors
- fonts
- section descriptions

## Best Browser Support

The app works best in modern browsers.

### Notes
- Pronunciation depends on browser support for speech synthesis.
- Voice quality and available accents may vary by browser and device.
- Local storage data stays in the same browser unless manually cleared.

## Recommended Use Cases

This project is suitable for:
- English clubs
- school language practice
- IELTS vocabulary support
- classroom demo tools
- self-study vocabulary apps
- lightweight GitHub-hosted learning pages

## Deployment

Because the project is a single HTML file, it can be hosted easily on:
- GitHub Pages
- Netlify
- Vercel
- any shared hosting or cPanel hosting

## Author

**Md. Arfan Tahnif**  
GitHub: [arfan-tahnif](https://github.com/arfan-tahnif)

## Future Improvement Ideas

Possible upgrades for future versions:
- CEFR labels such as A1, A2, B1, B2, C1
- score history charts
- export/import saved progress
- admin panel for adding words
- multiple quiz modes
- real PDF previews
- pronunciation voice selection
- mobile-first enhancements

## Credits

Developed as a words English learning interface for vocabulary practice, pronunciation support, progress tracking, and study resources.

## License
