# AI Prompt Engineer

AI Prompt Engineer is a modern web-based tool for building, refining, and engineering prompts for large language models (LLMs) like OpenAI GPT and Google Gemini. It provides a guided, wizard-style interface to help users craft comprehensive prompts, experiment with model parameters, and interact with AI in a structured way.

🌐 Try It Online
Test the AI Prompt Engineer instantly in your browser: https://raw.githack.com/milankmezic/AIPromptEngineer/blob/main/index.html

## Features

- **Wizard-based Prompt Engineering:** Step-by-step interface to clarify your intent and build detailed prompts.
- **OpenAI & Gemini API Support:** Easily configure your API key, model, and endpoint.
- **Parameter Tuning:** Adjust temperature, max tokens, top-p, frequency/presence penalties, and more.
- **Dark Mode:** Toggle between light and dark themes.
- **Markdown Rendering:** AI responses are rendered with full markdown support.
- **Speech-to-Text:** Use your microphone to dictate messages (Web Speech API supported browsers).
- **Local Settings Storage:** All settings are saved in your browser for convenience.

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
   - Review, refine, and send prompts to the AI.
   - Use the chat interface for follow-up questions and iterative refinement.

## Parameters and URL Prefill

You can prefill the API key, model, and base URL fields by passing them as URL parameters when opening the app. This is useful for sharing links or automating configuration.

- `key`: Your API key (e.g., OpenAI or Gemini)
- `model`: The model name (e.g., `gpt-4`, `google/gemini-2.5-pro`)
- `url`: The base API URL (e.g., `https://api.openai.com/v1`)

**Example:**
```
https://yourdomain.com/index.html?key=YOUR_API_KEY&model=gpt-4&url=https://api.openai.com/v1
```

When you open the app with these parameters, the corresponding fields will be pre-filled automatically.

## Screenshots

> _Add screenshots or a demo GIF here to showcase the UI and workflow._

## Requirements
- Modern web browser (Chrome, Edge, Firefox, Safari)
- OpenAI or Gemini API key (for actual AI responses)

## Security Note
- **API keys are stored locally in your browser and never sent to any server except the configured AI endpoint.**
- Always keep your API keys secure and do not share them.

## License
GNU AFFERO GENERAL PUBLIC LICENSE. See LICENSE for details.

## Credits
- Built with [Tailwind CSS](https://tailwindcss.com/) and [marked.js](https://marked.js.org/).
- Inspired by the needs of prompt engineers and AI enthusiasts.

---

_Contributions, issues, and feature requests are welcome!_ 
