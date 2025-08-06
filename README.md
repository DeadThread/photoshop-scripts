🖼️ Photoshop Scripts – Automated Poster Generators

A collection of Adobe Photoshop automation scripts to generate event posters from a PSD template using folder names as data sources. Ideal for artists, promoters, and designers managing multiple shows or events.
📂 Scripts Included
1. basicPosterGenerator.jsx

🔹 Date-Venue-City-Combined
Generates a single Poster.jpg for each subfolder by updating one text layer:

Date
Venue
City

All content is placed into a single text layer named:
Date / Venue / City

📤 Output:

    Poster.jpg only (flattened)
    Useful for rapid deployment with minimal PSD setup

2. Date-Venue-City-Seperate.jsx

🔹 Full-featured version
Searches for three separate text layers (Date, Venue, City) and updates them independently.

✨ Features:

    Preserves original position and text justification
    Logs all text layers to console for debugging
    Exports both flattened and layered files

📤 Output:

    Poster.jpg (optimized for web)
    Poster.psd (fully layered for editing)

🧠 Folder Structure Requirements

All scripts require a root folder containing subfolders, each representing an event.
Subfolder names must follow this format:

Artist - YYYY-MM-DD - Venue - City [optional state/notes]

Example:

Gorillaz - 2025-08-09 - Red Rocks - Morrison (CO)

From this, the scripts will extract:

    Date: 2025-08-09
    Venue: Red Rocks
    City: Morrison

📝 PSD Template Setup
Script 	Required Text Layers
basicPosterGenerator 	Date / Venue / City
advancedPosterGenerator 	Date, Venue, and City (separate)

Make sure these text layers exist and are properly named in your PSD template.
🚀 How to Run

    Open Adobe Photoshop
    Navigate to:
    File → Scripts → Browse...
    Select the script you want to run (.jsx file)
    Follow prompts to select:
        A .psd template file
        A root folder containing event subfolders

Each subfolder will receive the appropriate poster output.
💼 Use Cases

    Touring artists and bands
    Music or event promoters
    Batch poster creation for social media
    Quick PSD-to-JPG conversions with metadata injection

✅ Requirements

    Adobe Photoshop (tested with modern versions)
    A .psd template with correct layer naming
    Properly structured event folders

📄 License

MIT License — Free to use and modify.
📁 Example Directory

photoshop-scripts/
├── basicPosterGenerator.jsx
├── advancedPosterGenerator.jsx
└── README.md

/Shows
├── Gorillaz - 2025-08-09 - Red Rocks - Morrison (CO)
│ ├── Poster.jpg
│ └── Poster.psd ← (only with advanced script)
