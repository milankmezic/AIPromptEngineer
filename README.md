# AI Prompt Engineer

AI Prompt Engineer is a modern web-based tool for building, refining, and engineering prompts for large language models (LLMs) like OpenAI GPT and Google Gemini. It provides a guided, wizard-style interface to help users craft comprehensive prompts, experiment with model parameters, and interact with AI in a structured way.

# Demo
https://rawcdn.githack.com/milankmezic/AIPromptEngineer/0e730672df7d033dc85c47b434fefcc440599cb8/index.html

## Features

- **Wizard-based Prompt Engineering:** Step-by-step interface to clarify your intent and build detailed prompts.
- **Smart Placeholder Detection:** Automatically detects `[variable]` placeholders in your questions and generates contextual options to fill them.
- **Dynamic Question Generation:** For each placeholder, the AI generates relevant questions and options (e.g., "What country?" → ["United States", "France", "Japan", etc.]).
- **Custom Input Options:** "✏️ Other" button allows users to enter custom values for any question or placeholder.
- **OpenAI & Gemini API Support:** Easily configure your API key, model, and endpoint.
- **Parameter Tuning:** Adjust temperature, max tokens, top-p, frequency/presence penalties, and more.
- **Dark Mode:** Toggle between light and dark themes.
- **Markdown Rendering:** AI responses are rendered with full markdown support.
- **Speech-to-Text:** Use your microphone to dictate messages (Web Speech API supported browsers).
- **Local Settings Storage:** All settings are saved in your browser for convenience.
- **Automatic Follow-up Suggestions:** After each AI response, the system automatically generates relevant follow-up actions you can click to continue the conversation.
- **Auto-focus:** Input boxes automatically receive focus for seamless typing experience.
- **Clickable Header:** Click the header with robot emoji to return to the first page anytime.

## Getting Started

1. **Clone the repository:**
   ```bash
   git clone https://github.com/milankmezic/AIPromptEngineer.git
   cd AIPromptEngineer
   ```

2. **Open the App:**
   - Simply open `index.html` in your web browser (Chrome recommended).
   - No build step or server required.

3. **Configure API Settings:**
   - Click the settings (gear) icon.
   - Enter your OpenAI or Gemini API key, model, and (optionally) base URL.
   - Adjust parameters as needed.

4. **Start Engineering Prompts:**
   - Click "Get Started" and follow the wizard to build your prompt.
   - **Using Placeholders:** Enter questions with `[variable]` placeholders (e.g., "What is the capital of [country]?") and the system will automatically generate options to fill them.
   - **Custom Input:** Use the "✏️ Other" button to enter custom values for any question or placeholder.
   - Review, refine, and send prompts to the AI.
   - Use the chat interface for follow-up questions and iterative refinement.
   - Click on automatically generated follow-up suggestions to continue the conversation.

## Parameters and URL Prefill

You can prefill the API key, model, and base URL fields by passing them as URL parameters when opening the app. This is useful for sharing links or automating configuration.

- `key`: Your API key (e.g., OpenAI or Gemini)
- `model`: The model name (e.g., `gpt-4`, `google/gemini-2.5-flash-lite`)
- `url`: The base API URL (e.g., `https://api.openai.com/v1`)

**Example:**
```
https://yourdomain.com/index.html?key=YOUR_API_KEY&model=gpt-4&url=https://api.openai.com/v1
```

When you open the app with these parameters, the corresponding fields will be pre-filled automatically.

## Using Placeholders

The AI Prompt Engineer now supports smart placeholder detection and replacement. Here's how it works:

### **Placeholder Syntax**
Use square brackets to indicate variables in your questions:
- `"What is the capital of [country]?"`
- `"Tell me about [topic] in [year]"`
- `"How do I [action] with [tool]?"`

### **How It Works**
1. **Detection:** The system automatically detects `[variable]` patterns in your question
2. **Question Generation:** For each placeholder, the AI generates a contextual question
3. **Options Display:** You'll see relevant options to choose from (e.g., countries, topics, years)
4. **Custom Input:** Use the "✏️ Other" button to enter your own custom value
5. **Automatic Replacement:** Selected values automatically replace the placeholders
6. **Continue to Refinement:** After filling all placeholders, proceed to the normal refinement flow

### **Example Flow**
**Input:** `"What is the capital of [country]?"`

**System Response:**
- Detects `[country]` placeholder
- Generates: "Which country are you interested in exploring?"
- Shows options: ["United States", "France", "Japan", "Brazil", "Australia", "India"]
- User selects "France"
- Question becomes: "What is the capital of France?"
- Continues to normal refinement screen

## Recent Updates

- **Smart Placeholder Detection:** Automatically detects and handles `[variable]` placeholders in questions
- **Dynamic Question Generation:** AI generates contextual questions and options for each placeholder
- **Custom Input Feature:** "✏️ Other" button allows users to enter custom values for any question
- **Enhanced Navigation:** Improved step-by-step flow with proper button management
- **Automatic Follow-up Suggestions:** The AI now generates contextual follow-up actions after each response
- **Enhanced UX:** Auto-focus on input fields and clickable header navigation
- **Improved Defaults:** Set to use `google/gemini-2.5-flash-lite` by default
- **Streamlined Interface:** Removed stream option for cleaner settings panel
- **GitHub Integration:** Direct link to latest version on GitHub from splash screen

## Screenshots

> _Add screenshots or a demo GIF here to showcase the UI and workflow._

## Demo

🎥 **Watch the demo video:** [AI Prompt Engineer Demo](https://youtu.be/0K5Fi08m1ds)

🔗 **Try it live:** [AI Prompt Engineer](https://rawcdn.githack.com/milankmezic/AIPromptEngineer/0e730672df7d033dc85c47b434fefcc440599cb8/index.html)

## Requirements
- Modern web browser (Chrome, Edge, Firefox, Safari)
- OpenAI or Gemini API key (for actual AI responses)

## Security Note
- **API keys are stored locally in your browser and never sent to any server except the configured AI endpoint.**
- Always keep your API keys secure and do not share them.

## License

GNU AFFERO GENERAL PUBLIC LICENSE. See [LICENSE](../LICENSE) for details.

## Credits
- Built with [Tailwind CSS](https://tailwindcss.com/) and [marked.js](https://marked.js.org/).
- Inspired by the needs of prompt engineers and AI enthusiasts.

---

_Contributions, issues, and feature requests are welcome!_ 
