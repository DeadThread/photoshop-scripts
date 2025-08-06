📸 Date-Venue-City-Combined.jsx

This Adobe Photoshop script (.jsx) automates the process of generating Poster.jpg files from a single PSD template using data parsed from folder names.
🛠️ What It Does

    Prompts you to select:
        A .psd template file.
        A root folder containing subfolders for each event or show.
    For each subfolder:
        Parses the folder name to extract Date, Venue, and City.
        Inserts that information into a text layer named Date / Venue / City in the PSD.
        Exports the result as Poster.jpg into the subfolder.

📁 Folder Name Format

Each subfolder should follow this naming format:

Artist - YYYY-MM-DD - Venue - City [or City (State)]

🔍 Example:

Gorillaz - 2025-08-09 - Red Rocks - Morrison (CO)

Parsed into:

    Date: 2025-08-09
    Venue: Red Rocks
    City: Morrison

🧾 Text Layer Format

The script inserts the parsed information into the following text layer:

Date / Venue / City

It will be replaced with:

2025-08-09
Red Rocks
Morrison
💾 Output

Each subfolder will receive a new file:

Poster.jpg

    Format: JPEG
    Quality: 90%
    Optimized for web
    The original template is never modified

🚀 How to Use

    Open Photoshop.
    Go to File > Scripts > Browse...
    Select the script file (batchPosterGenerator.jsx).
    Follow the prompts to:
        Select your PSD template
        Select the root folder with event subfolders
    Let the script process each folder automatically.

⚠️ Requirements

    Adobe Photoshop (tested on modern versions)
    A .psd template containing a text layer named Date / Venue / City
    Properly named subfolders

📂 Example Folder Structure

/Shows
├── Gorillaz - 2025-08-09 - Red Rocks - Morrison (CO)
│ └── Poster.jpg
├── Daft Punk - 2025-12-01 - MSG - New York (NY)
│ └── Poster.jpg
📄 License

MIT License — Free to use and modify