🎙️ Smart Voice Calculator
A modern, feature-rich calculator built with Flutter that supports voice commands, persistent calculation history, and dynamic theme switching. This app leverages a clean UI and robust state management to provide a seamless user experience.

✨ Features
🎙️ Voice-to-Text Input: Perform calculations hands-free using the integrated speech recognition system.

📜 Persistent History: Automatically saves your last 15 calculations locally using Hive, so you never lose track of your work.

🎨 Dynamic Themes: Choose from 4 distinct built-in themes (Light and Dark variations) with custom accent colors (Blue, Orange, Green, Red).

🔢 Advanced Logic: Handles complex math expressions, percentage calculations, and smart parentheses placement.

📱 Responsive UI: A clean, grid-based layout that adapts to different screen sizes and orientations.

🛠️ Tech Stack
Framework: Flutter (Dart)

State Management: Provider — Handles real-time theme switching and UI updates.

Local Database: Hive — Lightweight and blazing-fast key-value database for history persistence.

Math Engine: Math Expressions — Parses and evaluates complex mathematical strings.

Voice Recognition: Speech to Text — Converts spoken words into mathematical inputs.

🚀 Getting Started
Prerequisites
Flutter SDK installed on your machine.

An IDE (VS Code or Android Studio).

A physical device or emulator (Note: Speech-to-text requires microphone permissions on physical devices).

📁 Project Structure
Plaintext
lib/
├── main.dart              # App entry point & Provider configuration
├── calculator_screen.dart # Main UI logic & Calculation engine
└── theme.dart             # Custom ThemeData definitions
⚙️ How It Works
Calculation Logic: The app uses the math_expressions library to parse strings like (2+5)x3 into executable code.

Data Persistence: On every "=" press, the result is saved to a Hive box named calculation_history. This data is reloaded the next time the app opens.

Theme Provider: The ThemeProvider class listens for index changes and updates the MaterialApp theme instantly without losing the app state.

🤝 Contributing
Contributions are welcome! If you have ideas for new features (like scientific modes or currency conversion), feel free to fork the repo and submit a pull request.
