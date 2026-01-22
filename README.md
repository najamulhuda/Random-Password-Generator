# Random Password Generator

A lightweight, secure browser-based password generator that creates strong random passwords with customizable character sets. Built with vanilla JavaScript, HTML, and CSS - no dependencies required.

## Table of Contents
- [Features](#features)
- [Demo](#demo)
- [Screenshots](#screenshots)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [How It Works](#how-it-works)
- [Future Enhancements](#future-enhancements)
- [Contributing](#contributing)
- [License](#license)
- [Author](#author)

## Features

- Random password generation with 12 characters
- Includes uppercase letters, lowercase letters, numbers, and special symbols
- One-click copy to clipboard functionality
- Clean and responsive user interface
- No external dependencies
- Client-side generation for maximum security

## Demo

[Live Demo](https://github.com/najamulhuda/Random-Password-Generator/settings/pages) <!-- Add your GitHub Pages or deployment link here -->

## Screenshots

![Password Generator Screenshot](./screenshot.png)
<!-- Add your screenshot in the repository and update the path -->

## Technologies Used

- HTML5
- CSS3
- JavaScript (Vanilla)
- Google Fonts (Poppins)

## Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/random-password-generator.git
```

Navigate to the project directory:

```bash
cd random-password-generator
```

Open the `index.html` file in your browser:

```bash
# On macOS
open index.html

# On Linux
xdg-open index.html

# On Windows
start index.html
```

Or simply double-click the `index.html` file.

## Usage

1. Open the application in your web browser
2. Click the "Generate Password" button to create a random password
3. The password will appear in the input field
4. Click the copy icon to copy the password to your clipboard
5. Paste and use your secure password wherever needed

## Project Structure

```
random-password-generator/
│
├── index.html              # Main HTML file
├── style.css               # CSS stylesheet
├── images/                 # Directory for images
│   ├── copy.png           # Copy icon
│   └── generate.png       # Generate button icon
└── README.md              # Project documentation
```

## How It Works

### Password Generation Algorithm

The password generator ensures security by:

1. **Character Set Definition**: Uses four character sets:
   - Uppercase: `ABCDEFGHIJKLMNOPQRSTUVWXYZ`
   - Lowercase: `abcdefghijklmnopqrstuvwxyz`
   - Numbers: `123456789`
   - Symbols: `@#$%^&*()_+~|}{[]></-=`

2. **Guaranteed Diversity**: The algorithm ensures at least one character from each set:
   ```javascript
   password += upperCase[Math.floor(Math.random() * upperCase.length)];
   password += lowerCase[Math.floor(Math.random() * lowerCase.length)];
   password += number[Math.floor(Math.random() * number.length)];
   password += symbol[Math.floor(Math.random() * symbol.length)];
   ```

3. **Random Fill**: Remaining characters are randomly selected from all character sets

4. **Output**: Generates a 12-character password with mixed character types

### Copy to Clipboard

Uses the `document.execCommand("copy")` method to copy the generated password to the clipboard.

## Future Enhancements

- [ ] Add password length customization slider
- [ ] Add character type toggle options (enable/disable uppercase, lowercase, numbers, symbols)
- [ ] Implement password strength indicator
- [ ] Add password history with local storage
- [ ] Create dark/light theme toggle
- [ ] Add multiple password generation
- [ ] Include password entropy calculator
- [ ] Add export functionality (download passwords as text file)

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository

```bash
git fork https://github.com/yourusername/random-password-generator.git
```

2. Create a new branch

```bash
git checkout -b feature/your-feature-name
```

3. Make your changes and commit

```bash
git add .
git commit -m "Add: your feature description"
```

4. Push to your branch

```bash
git push origin feature/your-feature-name
```

5. Open a Pull Request

## License

This project is open source and available under the [MIT License](LICENSE).

## Author

**Your Name**

- GitHub: [@najamulhuda](https://github.com/najamulhuda)
- Email: najamulhuda791@gmail.com

---

### Show Your Support

Give a ⭐️ if you like this project!

---

**Made with ❤️ and JavaScript**
