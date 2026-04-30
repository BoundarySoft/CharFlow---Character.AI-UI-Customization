# CharFlow---Character.AI-UI-Customization
A Tampermonkey extension for Character.AI

![CharFlow preview](https://i.imgur.com/6slCpdM.png)

# CharFlow - Character AI Customization

A Tampermonkey userscript that lets you completely customize the look and feel of Character.AI chat pages.

## Main Purpose

This script transforms the default Character.AI chat interface into a fully customizable experience. It adds a settings panel that lets you change colors, fonts, backgrounds, bubble shapes, and much more—without touching any of the original website's code.

## Key Features

### Visual Customization
- **Backgrounds** – Set an image URL or upload a local file as your chat background. Adjust blur, brightness, and add a color overlay.
- **Chat Bubbles** – Change bubble colors (same for all or separate for AI/User), add glassmorphism effects, borders, and drop shadows.
- **Corner Styles** – Make bubbles uniformly rounded or customize each corner individually.
- **Typography** – Choose from 15+ Google Fonts, use a custom font URL, adjust size, weight, line height, and color text differently for AI vs User.
- **Text Styling** – Enable custom colors for italic and bold text.

### Preset System
- Save your current settings as a named preset
- Load, delete, export, or import presets (share them with others)
- Reset individual categories or everything to default

### Chat Tools
- **Export Chat** – Download your conversation as a clean HTML file with avatars, search functionality, and dark/light mode toggle.
- **Remove Disclaimer** – Hide the "AI chatbot" warning messages (visual only, doesn't affect functionality).

### Interface
- Floating settings button (draggable, saves position)
- Collapsible settings panel (also draggable)
- Search through settings by keyword
- Category-based organization
- Visual previews for corner radius changes
- Toast notifications for actions

## How It Works Together

1. **Load** – Script checks you're on a Character.AI chat page, then injects its own CSS and UI elements.

2. **Storage** – All settings are saved locally in your browser using Tampermonkey's storage. Nothing is sent anywhere.

3. **Real-time Updates** – When you change a setting (like a color or slider), the script instantly updates the chat page CSS and saves the preference.

4. **Dynamic Monitoring** – A MutationObserver watches for new messages being added and reapplies your styles automatically.

5. **Presets** – Saving a preset captures every setting into a JSON object. Loading it applies all those values at once.

![CharFlow preview_2](https://i.imgur.com/Ly8tio0.png)
