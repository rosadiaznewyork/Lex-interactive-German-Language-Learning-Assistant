# German Language Learning Application

An interactive web application designed to help users practice German language skills through realistic scenario-based conversations. The application features speech recognition, text-to-speech capabilities, and real-time translations.

## Features

- 🎭 **Scenario-based Learning**: Practice German in real-life situations:
  - Supermarket conversations
  - Restaurant interactions
  - Train station dialogues

- 🎙️ **Speech Recognition**: Record your responses in German using your device's microphone

- 🔊 **Text-to-Speech**: Listen to native German pronunciations

- 🔄 **Real-time Translation**: Toggle between German and English translations

- 🤖 **AI-Powered Conversations**: Natural dialogue flow using advanced language models

## Technology Stack

### Frontend
- React.js
- RecordRTC for audio recording
- Web Speech API
- CSS for animations and styling
- FontAwesome icons

### Backend
- Node.js with Express
- TypeScript
- Integration with:
  - AssemblyAI for speech-to-text conversion
  - Deepseek AI for natural language processing
  - gTTS (Google Text-to-Speech) for audio generation

## Getting Started

### Prerequisites
- Node.js (v14 or higher)
- npm or yarn
- Modern web browser with microphone support

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/german-language-learning.git
cd german-language-learning
```

2. Install dependencies for both frontend and backend:
```bash
# Install backend dependencies
cd backend
npm install

# Install frontend dependencies
cd ../frontend
npm install
```

3. Set up environment variables:
```bash
# In backend directory
cp .env.example .env
```
Edit the `.env` file with your API keys and configuration:
```
ASSEMBLYAI_API_KEY=your_key_here
DEEPSEEK_API_KEY=your_key_here
PORT=3000
```

### Running the Application

1. Start the backend server:
```bash
# In backend directory
npm run dev
```

2. Start the frontend development server:
```bash
# In frontend directory
npm start
```

3. Open your browser and navigate to `http://localhost:3000`

## Running in docker

1. Build the docker image:
```bash
docker build -t german-language-learning .

# Run the docker container
docker run -p 3000:3000 german-language-learning

# Open your browser and navigate to # Open your browser and navigate to URL_ADDRESS:3000
```
2. Configuration
- `ASSEMBLYAI_API_KEY`: Your AssemblyAI API key
- `DEEPSEEK_API_KEY`: Your Deepseek AI API key
- `PORT`: Port on which the server will run (optional, default is 3000)

## Usage

1. Select a scenario from the available options on the home page
2. Click the microphone icon to start recording your response
3. Speak your response in German
4. The application will:
   - Convert your speech to text
   - Provide feedback on pronunciation
   - Offer suggestions for improvement
   - Generate an appropriate AI response

## Contributing

We welcome contributions! Please follow these steps:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/improvement`)
3. Make your changes
4. Commit your changes (`git commit -am 'Add new feature'`)
5. Push to the branch (`git push origin feature/improvement`)
6. Create a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Thanks to AssemblyAI for speech recognition capabilities
- Thanks to Deepseek AI for natural language processing
- Thanks to all contributors who have helped shape this project

## Support

If you encounter any issues or have questions, please:
- fix it yourself. this is just for fun.

## Roadmap

- [ ] Add more conversation scenarios
- [ ] Implement progress tracking
- [ ] Add gamification elements
- [ ] Support for different German dialects
- [ ] Mobile app development