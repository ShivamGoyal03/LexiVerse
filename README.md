# LexiVerse

## Description
LexiVerse is a Flask application that leverages OpenAI's API to generate creative content based on user prompts. It is designed to assist with generating marketing emails, blog posts, tweets, ad copy, and product descriptions in a friendly yet professional tone.

## Features
- Generate creative content based on user prompts
- Tailor writing style to user-specified audience
- Avoid harmful, hateful, or copyrighted content
- Configurable parameters for content generation

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/ShivamGoyal03/LexiVerse.git
   cd LexiVerse
   ```
2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```
3. Install the dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Set up environment variables in a `.env` file:
   ```
   OPENAI_API_KEY=your_openai_api_key
   OPENAI_ENDPOINT=your_openai_endpoint
   CHAT_COMPLETIONS_DEPLOYMENT_NAME=your_deployment_name
   TEMPERATURE=0.7
   MAX_TOKENS=150
   PRESENCE_PENALTY=0.6
   FREQUENCY_PENALTY=0.0
   TOP_P=1.0
   N_VAR=1
   ```

## Usage
1. Run the Flask application:
   ```bash
   flask run
   ```
2. Open your web browser and navigate to `http://127.0.0.1:5000`.
3. Enter your prompt in the text area and click "Generate" to receive the generated content.

## Environment Variables
- `OPENAI_API_KEY`: Your OpenAI API key
- `OPENAI_ENDPOINT`: Your OpenAI API endpoint
- `CHAT_COMPLETIONS_DEPLOYMENT_NAME`: Deployment name for chat completions
- `TEMPERATURE`: Sampling temperature for content generation
- `MAX_TOKENS`: Maximum number of tokens to generate
- `PRESENCE_PENALTY`: Presence penalty for content generation
- `FREQUENCY_PENALTY`: Frequency penalty for content generation
- `TOP_P`: Top-p sampling parameter
- `N_VAR`: Number of completions to generate

## Deployment
The application is configured to run on Vercel. The `vercel.json` file specifies the build and routing configuration.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
