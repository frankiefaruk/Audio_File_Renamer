# Audio File Renamer / Text File Generator

A Python GUI application for managing audio file names in a musical context. This tool helps musicians and audio engineers to:
1. Generate text files containing standardized audio file names based on MIDI note ranges
2. Batch rename audio files according to MIDI note numbers and names
   
![Screenshot 2024-11-16 at 4 08 09 pm](https://github.com/user-attachments/assets/5dcc3024-d374-4765-9593-b19d4a5c5a37)


## Features

- User-friendly GUI interface
- Live preview of file names
- Support for various audio file formats (.wav, .aif, .aiff, .mp3)
- Automatic backup creation before renaming files
- MIDI note range validation
- Standardized naming convention: `{MIDI_number}_{Note_name}_{Instrument_name}.wav`

## Dependencies

- Python 3.8 or higher
- tkinter (usually comes with Python)
- watchdog==3.0.0

## Installation

1. Clone this repository:

bash
git clone https://github.com/frankiefaruk/Audio_File_Rename.git
cd audio-file-renamer


2. Install required packages:

bash
pip install -r requirements.txt


## Usage

1. Run the application:

bash
python main_gui.py


2. Using the Text File Generator:
   - Enter instrument name (e.g., "Electric_Guitar")
   - Enter note range (e.g., "E2-E6")
   - Click "Submit"
   - Choose "Create Text File"
   - Select save location for the text file

3. Using the File Renamer:
   - Enter instrument name (e.g., "Electric_Guitar")
   - Enter note range (e.g., "E2-E6")
   - Click "Submit"
   - Choose "Select Folder to Rename"
   - Select folder containing audio files
   - Review the preview of changes
   - Click "Rename" to process files

## File Naming Convention

The application uses the following naming convention:
- Format: `{MIDI_number}_{Note_name}_{Instrument_name}.wav`
- Example: `60_C4_Electric_Guitar.wav`

## Project Structure

audio-file-renamer/
├── main_gui.py # Main GUI application
├── extract_midi_notes.py # MIDI note mapping utilities
├── requirements.txt # Project dependencies
└── README.md # Documentation


## Safety Features

- Creates automatic backups before renaming files
- Validates note ranges before processing
- Preview changes before applying
- Error handling and user feedback

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Support

For support, please open an issue in the GitHub repository.

## Requirements.txt

watchdog==3.0.0
