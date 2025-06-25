# English Accent Analyzer

## Overview
The English Accent Analyzer is a sophisticated tool that analyzes spoken English accents from video content. It's designed to help hiring managers, language instructors, and HR professionals evaluate English pronunciation patterns for recruitment, training, and development purposes.

## Features

- **Multi-Platform Video Support**:
  - YouTube, Vimeo, Loom videos
  - Google Drive and Dropbox links
  - Direct MP4, AVI, MOV, and other video files
  - Automatically handles video download and processing

- **Advanced Speech Analysis**:
  - Accurate transcription using OpenAI's Whisper model
  - Vocabulary pattern recognition for accent classification
  - Phonetic pattern analysis of pronunciation
  - Grammatical structure analysis
  - Phrase identification for accent markers

- **Comprehensive Accent Classification**:
  - American English detection
  - British English detection
  - Australian English detection
  - Neutral/International English recognition

- **Detailed Reporting**:
  - Confidence scores with weighted multi-factor analysis
  - Detailed explanation of accent classification
  - Full transcript with punctuation
  - Speech statistics (WPM, word count, sentence count)
  - Debugging information for transparency

## Technical Implementation

The system consists of three main components:

1. **Video Processor**: Handles downloading and extracting audio from videos using yt-dlp and FFmpeg.

2. **Audio Analyzer**: Transcribes speech using Whisper and extracts speech statistics.

3. **Accent Detector**: Analyzes transcripts and audio using multiple detection strategies:
   - Vocabulary differences (e.g., "color" vs. "colour")
   - Phonetic patterns (e.g., rhotic vs. non-rhotic 'r')
   - Grammatical structures (e.g., "I've got" vs. "I have")
   - Distinctive phrases (e.g., "bloody hell" vs. "y'all")

## Installation

### Prerequisites
- Python 3.7 or higher
- FFmpeg (automatically used via imageio-ffmpeg)
- Internet connection for downloading videos

### Installation Steps

1. Clone the repository:
   ```bash
   git clone https://github.com/Aoukacha-Moussa/english_accent_detection.git
   cd english_accent_detection