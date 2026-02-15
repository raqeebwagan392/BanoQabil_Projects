# 🎯 QuizMaster - Interactive Knowledge Challenge

A modern, engaging quiz application built with pure HTML, CSS, and JavaScript. Features a vibrant gradient design, real-time timer, animated feedback, and comprehensive answer review system.

![QuizMaster](https://img.shields.io/badge/Status-Complete-success)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)
![No Dependencies](https://img.shields.io/badge/Dependencies-None-brightgreen)

## 🌟 Features

### 📚 Quiz System
- **50+ Question Pool**: Large variety of questions across multiple categories
- **Random Selection**: Every quiz session randomly selects 10 questions for variety
- **Multiple Categories**: General Knowledge, Science, Math, Geography, History, Technology, Arts, Sports
- **30-Second Timer**: Time pressure for each question with visual countdown
- **Real-time Feedback**: Instant visual feedback on correct/incorrect answers
- **Score Tracking**: Comprehensive scoring and statistics

### 🎨 User Experience
- **Vibrant Design**: Eye-catching gradient background with animated patterns
- **Smooth Animations**: Engaging transitions and effects throughout
- **Responsive Layout**: Works perfectly on desktop, tablet, and mobile devices
- **Keyboard Shortcuts**: Use 1-4, A-D keys to select answers, Enter to submit
- **Progress Tracking**: Visual progress bar and question counter

### 📊 Review & Analytics
- **Answer Review**: Complete review of all questions after quiz completion
- **Performance Analysis**: Detailed breakdown of correct/incorrect answers
- **Visual Indicators**: Color-coded feedback for easy understanding
- **Retake Option**: Start a new quiz with different random questions

## 🚀 Quick Start

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge)
- No build tools, libraries, or dependencies required!

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/quizmaster.git
   ```

2. **Navigate to the project folder**
   ```bash
   cd quizmaster
   ```

3. **Open the application**
   - Simply double-click `index.html` to open in your default browser
   - Or right-click → "Open with" → Choose your browser
   - Or use a local development server:
   
   ```bash
   # Using Python 3
   python -m http.server 8000
   
   # Using Python 2
   python -m SimpleHTTPServer 8000
   
   # Using Node.js (http-server)
   npx http-server
   
   # Using PHP
   php -S localhost:8000
   ```

4. **Start playing!**
   - Visit `http://localhost:8000` in your browser (if using local server)
   - Click "Start Quiz" and test your knowledge!

## 📂 Project Structure

```
quizmaster/
│
├── index.html          # Complete application (HTML, CSS, JS all-in-one)
├── README.md          # Project documentation
│
└── Assets (CDN-based)
    └── Google Fonts   # Space Mono & Poppins fonts
```

## 🎮 How to Play

1. **Start**: Click the "Start Quiz" button on the welcome screen
2. **Read**: Each question appears with 4 multiple-choice options
3. **Select**: Click on your answer (or use keyboard shortcuts: 1-4 or A-D)
4. **Submit**: Click "Submit Answer" button (or press Enter)
5. **Continue**: Click "Next Question" to proceed
6. **Review**: After completing all 10 questions, view your results and review answers

### ⚡ Features During Quiz
- **Timer**: 30 seconds per question (turns red at 10 seconds)
- **Progress Bar**: Visual indicator of quiz completion
- **Question Counter**: Shows current question number (e.g., "Question 3 of 10")
- **Immediate Feedback**: See if your answer is correct/incorrect right away
- **Auto-Submit**: Question auto-submits when timer reaches zero

## 🎨 Color Palette

```css
--primary: #FF6B6B       /* Coral Red - Main accent */
--secondary: #4ECDC4     /* Turquoise - Secondary accent */
--accent: #FFE66D        /* Sunny Yellow - Highlights */
--success: #06D6A0       /* Success Green */
--error: #EF476F         /* Error Pink */
--dark: #1A1A2E          /* Deep Navy - Dark elements */
--light: #FFFFFF         /* White - Clean backgrounds */
```

## 💻 Technologies Used

### Frontend
- **HTML5**: Semantic structure and accessibility
- **CSS3**:
  - CSS Variables (Custom Properties) for theming
  - Flexbox & Grid for responsive layouts
  - Keyframe animations for smooth transitions
  - Linear gradients for visual appeal
  - Media queries for responsiveness
- **Vanilla JavaScript**:
  - ES6+ features (arrow functions, template literals, spread operator)
  - Fisher-Yates shuffle algorithm for randomization
  - DOM manipulation
  - Event handling
  - Timer/interval management
  - Page Visibility API for tab management

### External Resources
- **Google Fonts**: Space Mono (display) & Poppins (body text)

## 📱 Responsive Breakpoints

- **Desktop**: > 768px (Full feature set)
- **Tablet**: 481px - 768px (Optimized layout)
- **Mobile**: ≤ 480px (Touch-friendly interface)

## ⌨️ Keyboard Shortcuts

| Key | Action |
|-----|--------|
| `1-4` or `A-D` | Select answer option |
| `Enter` | Submit selected answer |
| Works only during active question (before submission) |

## 🧠 Question Categories

The quiz includes 50 questions across 8 categories:

1. **General Knowledge** (10 questions)
   - World capitals, famous landmarks, cultural facts

2. **Science** (10 questions)
   - Physics, chemistry, biology, astronomy

3. **Mathematics** (5 questions)
   - Basic arithmetic, algebra, geometry

4. **Geography** (8 questions)
   - Countries, capitals, landmarks, continents

5. **History** (5 questions)
   - World events, historical figures, dates

6. **Technology & Computers** (5 questions)
   - Programming, internet, tech companies

7. **Arts & Literature** (3 questions)
   - Famous works, authors, composers

8. **Sports** (4 questions)
   - Rules, facts, Olympic knowledge

## 🎯 Scoring System

- **Each Question**: Equal weight (10% per question for 10-question quiz)
- **Perfect Score**: 100% (10/10 correct)
- **Performance Levels**:
  - 🏆 **100%**: Perfect Score! (Quiz Master)
  - 🌟 **80-99%**: Excellent Work!
  - 👍 **60-79%**: Good Job!
  - 📚 **40-59%**: Keep Learning!
  - 💪 **0-39%**: Don't Give Up!

## 🔧 Customization Guide

### Adding New Questions

Add questions to the `allQuestions` array in the JavaScript section:

```javascript
const allQuestions = [
    // ... existing questions
    {
        question: "Your question here?",
        options: ["Option A", "Option B", "Option C", "Option D"],
        correct: 2  // Index of correct answer (0-3)
    }
];
```

### Changing Quiz Length

Modify the number of questions selected:

```javascript
// In selectRandomQuestions() function
quizData = shuffled.slice(0, 10);  // Change 10 to your desired number
```

Also update display references:
```javascript
totalQuestionsSpan.textContent = 10;  // Update to match
totalQuestionsResult.textContent = 10;  // Update to match
```

### Adjusting Timer Duration

Change the timer duration (currently 30 seconds):

```javascript
// In loadQuestion() function
timeLeft = 30;  // Change to your desired seconds

// In startTimer() function - warning threshold
if (timeLeft <= 10) {  // Change when warning appears
    timerElement.classList.add('warning');
}
```

### Modifying Colors

Update CSS variables in the `:root` selector:

```css
:root {
    --primary: #FF6B6B;      /* Change to your color */
    --secondary: #4ECDC4;    /* Change to your color */
    --accent: #FFE66D;       /* Change to your color */
    /* ... other colors */
}
```

### Customizing Animations

Adjust animation speeds in CSS:

```css
:root {
    --transition-fast: 0.2s ease;    /* Quick transitions */
    --transition-normal: 0.3s ease;  /* Standard transitions */
    --transition-slow: 0.5s ease;    /* Slower transitions */
}
```

## 🌐 Browser Compatibility

| Browser | Version | Status |
|---------|---------|--------|
| Chrome | Latest | ✅ Fully Supported |
| Firefox | Latest | ✅ Fully Supported |
| Safari | Latest | ✅ Fully Supported |
| Edge | Latest | ✅ Fully Supported |
| Opera | Latest | ✅ Fully Supported |
| IE 11 | - | ⚠️ Limited Support |

**Note**: Modern browsers (released after 2020) recommended for best experience.

## ✨ Advanced Features

### Fisher-Yates Shuffle Algorithm
```javascript
function shuffleArray(array) {
    const shuffled = [...array];
    for (let i = shuffled.length - 1; i > 0; i--) {
        const j = Math.floor(Math.random() * (i + 1));
        [shuffled[i], shuffled[j]] = [shuffled[j], shuffled[i]];
    }
    return shuffled;
}
```

### Page Visibility API
Automatically pauses timer when user switches tabs:
```javascript
document.addEventListener('visibilitychange', () => {
    if (document.hidden) {
        clearInterval(timer);
    } else if (quizScreen.classList.contains('active') && !isAnswered) {
        startTimer();
    }
});
```

### Answer State Management
```javascript
let answeredQuestions = [];  // Stores all quiz history

answeredQuestions.push({
    question: "Question text",
    selectedAnswer: 2,        // User's choice (or null)
    correctAnswer: 1,         // Correct answer index
    isCorrect: false          // Boolean result
});
```

## 🎨 Design Philosophy

- **Vibrant & Energetic**: Gradient backgrounds with animated patterns
- **Clear Feedback**: Immediate visual confirmation of actions
- **Smooth Interactions**: Carefully crafted animations and transitions
- **User-Friendly**: Intuitive interface with helpful instructions
- **Accessible**: Keyboard navigation and clear visual hierarchy

## 🙏 Acknowledgments

- Fonts: [Google Fonts](https://fonts.google.com) (Space Mono & Poppins)
- Inspiration: Modern quiz applications and educational platforms
- Icons: Unicode emoji characters

## 🔮 Future Enhancements

Planned features for future versions:

- [ ] Difficulty levels (Easy, Medium, Hard)
- [ ] Category selection (choose specific topics)
- [ ] Multiplayer mode (compete with friends)
- [ ] Leaderboard system (track high scores)
- [ ] User accounts and progress tracking
- [ ] Question submission by users
- [ ] Sound effects and background music toggle
- [ ] Share results on social media
- [ ] Hints system (50/50, skip question)
- [ ] Detailed explanations for each answer
- [ ] Custom quiz creation
- [ ] Dark/Light theme toggle
- [ ] Internationalization (multiple languages)
- [ ] Accessibility improvements (screen reader support)
- [ ] Backend integration for persistent data
- [ ] Mobile app version (React Native/Flutter)

## 🎓 Learning Resources

This project demonstrates:
- Modern JavaScript practices (ES6+)
- CSS animations and transitions
- Responsive web design
- State management in vanilla JS
- Event-driven programming
- Timer and interval management
- Array manipulation algorithms
- DOM manipulation techniques

Perfect for beginners learning web development!

## 📊 Project Stats

- **Total Questions**: 50
- **Question Categories**: 8
- **Lines of Code**: ~1,500
- **File Size**: ~50KB
- **Dependencies**: 0 (Zero!)
- **Load Time**: < 1 second

---

## 📝 Changelog

### Version 1.0.0 (Current)
- ✅ Initial release
- ✅ 50 questions across 8 categories
- ✅ Random question selection
- ✅ Real-time timer with auto-submit
- ✅ Answer review system
- ✅ Responsive design
- ✅ Keyboard shortcuts
- ✅ Animated UI elements
- ✅ Performance statistics

---

**Happy Quizzing! 🎉**
