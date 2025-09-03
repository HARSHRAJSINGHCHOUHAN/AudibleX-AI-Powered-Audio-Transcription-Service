# AudibleX: AI-Powered Audio Transcription Service🎙️
AudibleX is a Spring Boot application that uses OpenAI’s Whisper model to convert audio files into accurate, high-quality transcriptions. 
Designed with both developers and non-technical users in mind, AudibleX offers a seamless API for transforming speech into readable text,
providing a flexible solution for various industries.

---

## Table of Contents
- [Why AudibleX?](#why-audiblex)
- [Features](#features)
- [Use Cases](#use-cases)
- [Technology Stack](#technology-stack)
- [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [Contributing](#contributing)

---

## Why AudibleX?
AudibleX was created to address the growing need for accessible and efficient audio transcription. 
By automating the process with AI, it allows users to save time and increase productivity, especially in industries where documentation,
accessibility, and content management are critical.

## Features

- 🎯 High-Quality Transcriptions:  Powered by OpenAI Whisper for precise and natural speech-to-text conversion.
- 🌍 Simple API Integration:  Designed as a RESTful API for easy integration into applications.
- 🔌Multiple File Format Support:  Supports popular audio formats like WAV, MP3, etc.
- 💻Fast Processing:  Returns transcriptions quickly, ideal for real-time applications.
- ⚡Customizable Settings:  Adjustable language and response formats for diverse needs. 

---

## Use Cases

- Education: Convert lectures and discussions into text for students and educators.
- Podcasting: Make audio content accessible by providing transcripts to your audience.
- Business Meetings: Generate text records of meetings for better documentation.
- Content Accessibility: Make audio content readable for those with hearing impairments.
- Personal Notes: Use as a tool for transcribing voice memos or brainstorming sessions.


---

## Technology Stack

- Backend: Java 17, Spring Boot 3.3.5
- AI: OpenAI Whisper model for speech-to-text processing
- Build: Maven for dependency management and project build
- APIs: RESTful services for easy access and integration 

---

## Installation

1. Clone the repository:  
   ```bash
   git clone https://github.com/your-username/AudibleX.git

2. Configure API Key: In your application.properties, add your OpenAI API key:
   spring.ai.openai.api-key=YOUR_OPENAI_API_KEY
   
4. Build and Run the Application:
   mvn clean install
mvn spring-boot:run
 The application should now be running on http://localhost:8080.

---

## Usage

AudibleX provides a simple API endpoint to upload audio files and receive a transcription. Make a POST request to /api/transcribe with your audio file.

Example Request
curl -X POST -F "file=@path_to_audio_file.wav" http://localhost:8080/api/transcribe

Example Response
{
  "transcription": "Your transcribed text here..."
}

---

## API Endpoints
- -POST /api/transcribe
Description: Accepts an audio file and returns the transcribed text.
Parameters:
file (MultipartFile): The audio file to be transcribed.
- Response:
200 OK: JSON response with the transcription result.
400 Bad Request: If the file format is unsupported or the request is invalid.

---

## Contributing

Contributions are welcome! If you would like to enhance AudibleX.




