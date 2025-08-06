🎨 Date-Venue-City-Seperate.jsx

This Adobe Photoshop script (.jsx) automates the creation of event-specific posters by dynamically updating text layers in a PSD template based on subfolder names. It saves both .jpg and .psd files into each subfolder.
💡 What It Does

    Prompts the user to:
        Select a PSD template
        Choose a root folder containing multiple subfolders (each representing an event)
    For each subfolder:
        Parses the folder name to extract Date, Venue, and City
        Updates individual text layers in the template:
            Date
            Venue
            City
        Exports:
            A flattened Poster.jpg
            A layered Poster.psd

📁 Folder Name Format

Each subfolder should follow this naming convention:

Artist - YYYY-MM-DD - Venue - City [or City (State)]

🔍 Example:

Daft Punk - 2025-12-01 - MSG - New York (NY)

Extracted as:

    Date: 2025-12-01
    Venue: MSG
    City: New York

Text within brackets or parentheses is stripped from the city name.
🖋️ Required PSD Layers

Your PSD template must contain separate text layers named exactly:

    Date
    Venue
    City

The script will automatically search through nested groups to find and update them. Text position and justification are preserved.
💾 Output Files

Each subfolder will receive two new files:

Poster.jpg ✅ High-quality JPEG for use
Poster.psd ✅ Layered PSD for editing

    JPEG:
        Format: Save for Web
        Quality: 90%
        Optimized: Yes
    PSD:
        Includes all layers
        Saved as a copy

📂 Example Structure

/Shows
├── Daft Punk - 2025-12-01 - MSG - New York (NY)
│ ├── Poster.jpg
│ └── Poster.psd
├── Radiohead - 2025-10-18 - Red Rocks - Morrison (CO)
│ ├── Poster.jpg
│ └── Poster.psd
🚀 How to Use

    Open Adobe Photoshop.
    Go to File > Scripts > Browse...
    Select the .jsx script file.
    When prompted:
        Choose your PSD template
        Select the root folder that contains your event subfolders
    Let the script process all subfolders automatically.

🧰 Features

    🔎 Auto-recognition of text layers, even inside groups
    🛡️ Robust error handling for missing layers or bad folder names
    📝 Logs all updated text layer names to the Photoshop console
    🧽 Whitespace-safe parsing and decoding of folder names

✅ Requirements

    Adobe Photoshop (any modern version)
    A properly structured PSD template with named text layers
    Subfolders with valid, parseable names

📄 License

MIT License — Use and modify freely.