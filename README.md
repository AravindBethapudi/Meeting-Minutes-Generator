## Meeting Minutes Generator
Meeting Minutes Generator is an AI-powered application that converts audio recordings of meetings into detailed, structured meeting minutes. Leveraging cutting-edge models like OpenAI's Whisper for transcription and GPT-4 for natural language processing, this tool provides an efficient and accurate way to summarize meetings with actionable insights.

Features
Automatic Speech Recognition (ASR):
Uses OpenAI's Whisper model to transcribe audio recordings into text with high accuracy.

Meeting Minutes Generation:
Employs GPT-4 via OpenAI's ChatCompletion API to generate structured meeting minutes, including:

Summary: A concise overview of the meeting objectives, discussions, and conclusions.
Attendees and Speakers: A list of key participants (note: speaker diarization is not used in this version).
Sentiments: Analysis of the overall sentiment and emotion expressed during the meeting.
Key Takeaways: Critical insights and conclusions drawn from the discussion.
Action Items & Decisions: Extraction of tasks, decisions, and responsibilities from the transcript.
Topic Segmentation: Organization of the conversation into topics for easier review.
Gradio Web Interface:
Provides a simple, interactive interface to upload audio files and view the generated meeting minutes in real time.
Installation
Clone the Repository:

bash
Copy
git clone https://github.com/your_username/meeting-minutes-generator.git
cd meeting-minutes-generator
Install Dependencies:

Ensure you have Python installed, then run:

bash
Copy
pip install -r requirements.txt
Note: The requirements.txt file includes dependencies like gradio, openai, transformers, and torch.

Usage
Set Your OpenAI API Key:

Make sure to set your API key as an environment variable. For example:

On macOS/Linux:
bash
Copy
export OPENAI_API_KEY="your_openai_api_key"
On Windows (Command Prompt):
cmd
Copy
set OPENAI_API_KEY=your_openai_api_key
Run the Application:

Start the app by executing:

bash
Copy
python app.py
This will launch a Gradio web interface. Simply upload an audio file of your meeting, and the application will:

Transcribe the audio using Whisper.
Analyze the transcript for sentiment, key takeaways, and action items.
Generate well-structured meeting minutes in Markdown format.
Contributing
Contributions are welcome! If you have any ideas or improvements, feel free to open an issue or submit a pull request.

License
This project is licensed under the MIT License.

