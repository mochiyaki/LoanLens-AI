# LoanLens-AI

An intelligent loan document analysis tool that helps users understand complex loan terms, evaluate documents for potential issues, and make informed financial decisions.

## Project Structure

```
loanlens-ai/
├── index.html              # Main HTML file with React app entry point
├── index.js                # Main JavaScript file containing the React application logic
├── index.css               # CSS styling for the application
├── README.md               # This documentation file
└── .git/                   # Git version control directory
```

## Workflow

### 1. Application Initialization
- The app loads from `index.html` which includes React and Tailwind CSS
- React is initialized in the root div with `index.js`
- CSS styling is applied via `index.css`

### 2. User Interaction Flow
1. **User Input**: User types questions or pastes loan documents into the chat input
2. **Chat Creation**: New chats are created automatically when user starts a conversation
3. **Message Processing**:
   - User messages are stored in local storage
   - System prompts guide AI behavior for loan document analysis
   - Messages are sent to API endpoints (cloud or local models)
4. **AI Response Generation**:
   - Responses can be streamed or non-streamed
   - Streaming provides real-time feedback during generation
5. **Response Display**:
   - Messages are rendered in the chat interface
   - Code blocks with HTML content can be launched directly from the UI
   - Messages are animated for better UX

### 3. Features
- **Document Analysis**: Understand complex loan terms and conditions
- **Financial Calculations**: Calculate monthly payments, total interest, amortization schedules
- **Risk Assessment**: Identify predatory lending practices or unfavorable terms
- **Comparison Tool**: Compare different loan options and their implications
- **Educational Content**: Explain APR, interest rates, fees in simple terms
- **Export Functionality**: Export conversations as JSON or Markdown
- **Settings Management**: Configure API endpoints, models, and generation parameters

### 4. Technical Architecture
- **Frontend**: React.js with functional components and hooks
- **Styling**: Tailwind CSS for responsive design
- **State Management**: React's useState and useEffect hooks
- **Persistence**: LocalStorage for saving chats and settings
- **API Integration**: Supports both cloud (OpenAI, Anthropic) and local (Ollama, LM Studio) models
- **Responsive Design**: Mobile-friendly interface with sidebar toggle

### 5. Settings Configuration
The application supports:
- Cloud API configuration (OpenAI, Anthropic, etc.)
- Local model configuration (Ollama, LM Studio)
- Generation parameters (temperature, top_p, max_tokens)
- Custom system prompts for AI behavior
- Streaming response toggles

## Usage

1. Open `index.html` in a web browser
2. Configure API settings via the settings modal
3. Start chatting with LoanLens AI about loan documents
4. Use quick prompts to get started or paste document text for analysis
5. Export conversations when needed

## Dependencies

- React 18
- Tailwind CSS
- IBM Plex Sans font
- LocalStorage for persistence