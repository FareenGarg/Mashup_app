# Music Mashup Generator

A simple web application that creates audio mashups by downloading music videos, extracting audio, and merging clips from your favorite artists.

## What Does It Do?

This project lets you:
- Search for videos of any artist
- Download the audio from those videos
- Cut the first Y seconds from each video
- Combine all the clips into one single audio file
- Get the final mashup file via email

## How to Use

### Command Line Usage

```
python 102303971.py "Artist Name" X Y output.mp3
```

**Parameters:**
- `Artist Name`: The name of the singer or artist
- `X`: Number of videos to download
- `Y`: Duration in seconds to cut from each video
- `output.mp3`: Name of the output file

**Conditions:**
- X must be greater than 10
- Y must be greater than 20

### Web Interface

1. Make sure you're in the project directory and run:
```
python app.py
```

2. Open your web browser and go to:
```
http://127.0.0.1:5000
```

3. Fill in the form:
   - Artist name
   - Number of videos (more than 10)
   - Duration per clip in seconds (more than 20)
   - Your email address

4. Submit and wait for the mashup to be created and sent to your email

## Requirements

Install the dependencies:
```
pip install -r requirements.txt
```

Key libraries used:
- `pytubefix` - Download videos from YouTube
- `moviepy` - Process and merge audio files
- `flask` - Web interface

## Installation

1. Clone or download this project
2. Install Python (3.7 or higher)
3. Install required packages:
```
pip install -r requirements.txt
```

## Important Notes

- You need at least **11 videos** to create a mashup
- Each clip must be at least **21 seconds** long
- The application downloads videos temporarily and cleans up after processing
- Email functionality requires Gmail setup with an app-specific password

## Troubleshooting

**Error: "Number of videos must be greater than 10"**
- Pass at least 11 videos when creating a mashup

**Error: "Duration must be greater than 20 seconds"**
- Set duration to at least 21 seconds

**Files not downloading?**
- Check your internet connection
- Make sure the artist name is valid and has videos available


