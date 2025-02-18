# Meeting Minutes Generator

**Meeting Minutes Generator** is an AI-powered application that transforms audio recordings of meetings into detailed, structured meeting minutes. By leveraging state-of-the-art models such as OpenAI's Whisper for transcription and GPT-4 for natural language processing, this tool efficiently summarizes meetings with actionable insights.

---

## Features

- **Automatic Speech Recognition (ASR):**  
  Utilizes OpenAI's Whisper model to accurately transcribe audio recordings into text.

- **Meeting Minutes Generation:**  
  Uses GPT-4 via OpenAI's ChatCompletion API to produce structured meeting minutes that include:
  - **Summary:**  
    A concise overview of the meeting objectives, discussions, and conclusions.
  - **Attendees and Speakers:**  
    A list of key participants. *(Note: Speaker diarization is not implemented in this version.)*
  - **Sentiments:**  
    Analysis of the overall sentiment and emotion expressed during the meeting.
  - **Key Takeaways:**  
    Critical insights and conclusions derived from the discussion.
  - **Action Items & Decisions:**  
    Extraction of tasks, decisions, and assigned responsibilities from the transcript.
  - **Topic Segmentation:**  
    Organization of the conversation into topics for easier review.

- **Gradio Web Interface:**  
  Offers a user-friendly, interactive interface to upload audio files and view the generated meeting minutes in real time.

---

## Installation

### 1. Clone the Repository

Open your terminal and run:

```bash
git clone https://github.com/your_username/meeting-minutes-generator.git
cd meeting-minutes-generator
