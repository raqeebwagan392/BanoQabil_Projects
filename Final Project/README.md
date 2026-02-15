# 🏋️ PowerFit Gym - Fitness Website

A modern, responsive gym website built with HTML, CSS, and JavaScript. Features a sleek dark theme with gradient accents, interactive components, and a fully functional user interface.

![PowerFit Gym](https://img.shields.io/badge/Status-Complete-success)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

## 🌟 Features

### 🎨 Modern Design
- **Dark Theme**: Eye-catching dark color scheme with gradient accents
- **Responsive Layout**: Fully responsive design that works on all devices
- **Smooth Animations**: Engaging animations and transitions throughout
- **Custom Styling**: Professional UI with custom buttons, cards, and components

### 📱 Sections

1. **Hero Section**
   - Full-screen landing with compelling tagline
   - Call-to-action buttons
   - Animated scroll indicator

2. **About Section**
   - Company information and mission
   - Dynamic statistics (Years, Members, Trainers)
   - Facilities showcase with icons

3. **Membership Plans**
   - Three tier pricing structure (Basic, Standard, Premium)
   - Feature comparison
   - Interactive plan selection

4. **Trainers Section**
   - Expert trainer profiles with images
   - Specialties and experience
   - Social media links

5. **Class Schedule**
   - Weekly class timetable
   - Color-coded difficulty levels
   - Trainer assignments

6. **BMI Calculator**
   - Real-time BMI calculation
   - Health category classification
   - Personalized recommendations

7. **Contact Form**
   - Membership registration
   - Form validation
   - Success confirmation

### ⚡ Interactive Features

- **Sticky Navigation**: Transparent navbar that becomes solid on scroll
- **Mobile Menu**: Hamburger menu for mobile devices
- **Active Section Highlighting**: Nav links highlight based on scroll position
- **Smooth Scrolling**: All anchor links use smooth scroll behavior
- **Plan Selection**: Auto-populates contact form when selecting a plan
- **BMI Calculator**: Dynamic calculation with health recommendations
- **Form Validation**: Comprehensive client-side validation
- **Scroll to Top**: Floating button appears on scroll

## 🚀 Getting Started

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge)
- No build tools or dependencies required!

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/powerfit-gym.git
   ```

2. **Navigate to the project directory**
   ```bash
   cd powerfit-gym
   ```

3. **Open the website**
   - Simply open `index.html` in your web browser
   - Or use a local development server:
   ```bash
   # Using Python
   python -m http.server 8000
   
   # Using Node.js (http-server)
   npx http-server
   ```

4. **View in browser**
   - Open `http://localhost:8000` in your browser

## 📂 Project Structure

```
powerfit-gym/
│
├── index.html          # Main HTML file (contains all code)
├── README.md           # Project documentation
│
└── Assets (referenced via CDN)
    ├── Font Awesome    # Icons
    ├── Google Fonts    # Poppins font family
    └── Unsplash        # Hero and trainer images
```

## 🎨 Color Palette

```css
--primary-color: #ff4655    /* Energetic Red */
--secondary-color: #00d4ff  /* Cool Cyan */
--dark-bg: #0a0e27          /* Dark Blue Background */
--darker-bg: #060815        /* Darker Blue */
--card-bg: #141b3a          /* Card Background */
--text-primary: #ffffff     /* White Text */
--text-secondary: #b8c1ec   /* Light Blue Text */
--success: #00ff88          /* Success Green */
--warning: #ffb800          /* Warning Orange */
```

## 💻 Technologies Used

- **HTML5**: Semantic markup and structure
- **CSS3**: 
  - CSS Variables for theming
  - Flexbox and Grid for layouts
  - Custom animations and transitions
  - Media queries for responsiveness
- **JavaScript (Vanilla)**:
  - DOM manipulation
  - Event handling
  - Form validation
  - BMI calculation logic
  - Intersection Observer API
- **External Libraries**:
  - Font Awesome 6.4.0 (icons)
  - Google Fonts (Poppins)

## 📱 Responsive Breakpoints

- **Desktop**: > 1024px
- **Tablet**: 768px - 1024px
- **Mobile**: < 768px
- **Small Mobile**: < 480px

## 🔧 Customization

### Changing Colors
Edit the CSS variables in the `:root` selector:
```css
:root {
    --primary-color: #your-color;
    --secondary-color: #your-color;
    /* ... other variables */
}
```

### Modifying Content
All content is within the HTML file. Key sections to edit:
- Hero title and subtitle
- About section text
- Membership plan details and pricing
- Trainer information
- Contact information

### Adding New Sections
Follow the existing section structure:
```html
<section class="your-section" id="your-id">
    <div class="container">
        <h2 class="section-title">Your Title</h2>
        <p class="section-subtitle">Your subtitle</p>
        <!-- Your content -->
    </div>
</section>
```

## ✨ Key Features Explained

### BMI Calculator
```javascript
// Formula: weight (kg) / height (m)²
const bmi = weight / (heightInMeters * heightInMeters);

// Categories:
// < 18.5: Underweight
// 18.5 - 24.9: Normal
// 25 - 29.9: Overweight
// ≥ 30: Obese
```

### Form Validation
- Name: Minimum 3 characters
- Email: Valid email format (regex)
- Phone: Valid phone format, minimum 10 digits
- Plan: Required selection
- Success message display after submission

### Scroll Effects
- Navbar background changes on scroll
- Active section highlighting in navigation
- Scroll-to-top button appears after scrolling
- Intersection Observer for element animations

## 🌐 Browser Support

- ✅ Chrome (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)
- ⚠️ IE11 (partial support, may require polyfills)

## 🙏 Acknowledgments

- Hero image from [Unsplash](https://unsplash.com)
- Icons from [Font Awesome](https://fontawesome.com)
- Fonts from [Google Fonts](https://fonts.google.com)

## 🔮 Future Enhancements

- [ ] Add backend integration for form submissions
- [ ] Implement user dashboard
- [ ] Add online class booking system
- [ ] Integrate payment gateway
- [ ] Add member testimonials section
- [ ] Create blog section for fitness tips
- [ ] Add multi-language support
- [ ] Implement dark/light theme toggle

---
