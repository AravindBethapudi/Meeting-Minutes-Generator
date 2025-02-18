<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <title>Meeting Minutes Generator</title>
    <style>
      body {
        font-family: Arial, sans-serif;
        line-height: 1.6;
        margin: 20px;
        color: #333;
      }
      h1, h2, h3 {
        color: #2c3e50;
      }
      pre {
        background-color: #f4f4f4;
        padding: 10px;
        overflow: auto;
      }
      code {
        background-color: #f4f4f4;
        padding: 2px 4px;
      }
    </style>
  </head>
  <body>
    <h1>Meeting Minutes Generator</h1>
    <p>
      Meeting Minutes Generator is an AI-powered application that converts audio
      recordings of meetings into detailed, structured meeting minutes. Leveraging
      cutting-edge models like OpenAI's Whisper for transcription and GPT-4 for natural
      language processing, this tool provides an efficient and accurate way to summarize
      meetings with actionable insights.
    </p>

    <h2>Features</h2>
    <ul>
      <li>
        <strong>Automatic Speech Recognition (ASR):</strong> Uses OpenAI's Whisper model
        to transcribe audio recordings into text with high accuracy.
      </li>
      <li>
        <strong>Meeting Minutes Generation:</strong> Employs GPT-4 via OpenAI's
        ChatCompletion API to generate structured meeting minutes, including:
        <ul>
          <li>
            <strong>Summary:</strong> A concise overview of the meeting objectives,
            discussions, and conclusions.
          </li>
          <li>
            <strong>Attendees and Speakers:</strong> A list of key participants (note:
            speaker diarization is not used in this version).
          </li>
          <li>
            <strong>Sentiments:</strong> Analysis of the overall sentiment and emotion
            expressed during the meeting.
          </li>
          <li>
            <strong>Key Takeaways:</strong> Critical insights and conclusions drawn from
            the discussion.
          </li>
          <li>
            <strong>Action Items & Decisions:</strong> Extraction of tasks, decisions, and
            responsibilities from the transcript.
          </li>
          <li>
            <strong>Topic Segmentation:</strong> Organization of the conversation into
            topics for easier review.
          </li>
        </ul>
      </li>
      <li>
        <strong>Gradio Web Interface:</strong> Provides a simple, interactive interface to
        upload audio files and view the generated meeting minutes in real time.
      </li>
    </ul>

    <h2>Installation</h2>
    <ol>
      <li>
        <strong>Clone the Repository:</strong>
        <pre>git clone https://github.com/your_username/meeting-minutes-generator.git
cd meeting-minutes-generator</pre>
      </li>
      <li>
        <strong>Install Dependencies:</strong>
        <p>Ensure you have Python installed, then run:</p>
        <pre>pip install -r requirements.txt</pre>
        <p>
          <em>Note:</em> The <code>requirements.txt</code> file includes dependencies
          such as <code>gradio</code>, <code>openai</code>, <code>transformers</code>, and
          <code>torch</code>.
        </p>
      </li>
    </ol>

    <h2>Usage</h2>
    <ol>
      <li>
        <strong>Set Your OpenAI API Key:</strong>
        <p>
          Make sure to set your API key as an environment variable.
          <br /><em>On macOS/Linux:</em>
        </p>
        <pre>export OPENAI_API_KEY="your_openai_api_key"</pre>
        <p>
          <em>On Windows (Command Prompt):</em>
        </p>
        <pre>set OPENAI_API_KEY=your_openai_api_key</pre>
      </li>
      <li>
        <strong>Run the Application:</strong>
        <p>Start the app by executing:</p>
        <pre>python app.py</pre>
        <p>
          This will launch a Gradio web interface. Simply upload an audio file of your
          meeting, and the application will:
        </p>
        <ul>
          <li>Transcribe the audio using Whisper.</li>
          <li>
            Analyze the transcript for sentiment, key takeaways, and action items.
          </li>
          <li>
            Generate well-structured meeting minutes in HTML/Markdown format.
          </li>
        </ul>
      </li>
    </ol>

    <h2>Contributing</h2>
    <p>
      Contributions are welcome! If you have any ideas or improvements, feel free to
      open an issue or submit a pull request.
    </p>

    <h2>License</h2>
    <p>This project is licensed under the MIT License.</p>
  </body>
</html>
