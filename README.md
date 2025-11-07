# real-ai

AI Assistant that Listens and Sees the World

This project is an AI assistant that utilizes both audio and video inputs to provide responses based on the user's queries. It leverages a webcam to capture images and a microphone to capture audio, combining these inputs to generate intelligent responses using a large language model.

## Features

- **Audio Recognition:** Captures audio using a microphone and converts speech to text using OpenAI's Whisper model.
- **Image Processing:** Captures images from a webcam and encodes them in base64 format.
- **Language Model Integration:** Uses ChatGoogleGenerativeAI or OpenAI's GPT-4o to generate responses based on the captured audio and image inputs.
- **Text-to-Speech (TTS):** Converts the generated text responses back to speech for audio output.
- **Real-time Processing:** Continuously listens to audio input and processes video frames in real-time.

## Technologies Used

- **Python**: Main programming language.
- **OpenAI**: Whisper model for speech recognition and TTS.
- **Google Generative AI**: Language model for generating responses.
- **LangChain**: Framework for chaining together prompts and models.
- **PyAudio**: Library for capturing and playing audio.
- **OpenCV**: Library for capturing and processing video.
- **Streamlit**: Library for creating web applications.

## Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/nizrhm/real-ai.git
   cd real-ai
   ```

2. **Create and activate a virtual environment:**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```

3. **Install the required packages:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Set up environment variables:**
   Create a `.env` file in the project root and add your OpenAI API key and Google Generative AI credentials:
   ```plaintext
   GROQ_API_KEY=your_groq_api_key
   OPENAI_API_KEY=your_openai_api_key
   ```

## Usage

1. **Run the AI assistant:**
   ```bash
   python app.py
   ```

2. **Interact with the assistant:**
   - Speak into the microphone to ask questions.
   - The assistant will process the audio and video inputs and provide responses.

## Code Structure

- `assistant.py`: Main script that initializes and runs the AI assistant.
- `requirements.txt`: List of dependencies required for the project.
- `.env`: File containing environment variables for API keys (not included in the repo).

## Example Output

When you run the assistant, it will display the webcam feed and listen for audio input. You can ask questions, and it will respond with both text and audio output.

## Contributing

Feel free to submit issues and pull requests. For major changes, please open an issue first to discuss what you would like to change.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.

## Acknowledgements

- [OpenAI](https://openai.com) for their Whisper and GPT models.
- [Google Generative AI](https://ai.google/tools) for their language model.
- [LangChain](https://langchain.com) for providing the framework to chain together the models and prompts.
- [Streamlit](https://streamlit.io) for their web application framework.
- [PyAudio](https://people.csail.mit.edu/hubert/pyaudio/) for audio capturing and playback.
- [OpenCV](https://opencv.org) for image capturing and processing.

---

Feel free to customize this README file further to better fit your specific project needs and personal preferences.