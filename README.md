# realtime-sales-negotiator

A voice-based AI shopping assistant that helps users find and negotiate prices for products. Built during a weekend hackathon in collaboration with https://github.com/kushal-10. Also check out some of his projects!

## Features
- Voice-based conversational interface
- Product recommendations based on user preferences
- Real-time price negotiation capabilities
- Integration with vector database for product search
- Agentic tool use

## ⚠️ Important Notes
- **Hardware Requirement**: Currently only works with headphones due to playback/microphone limitations
- **Cost Warning**: OpenAI's real-time API costs can reach more than $0.50/minute of conversation
- **Beta Status**: The OpenAI real-time API is in beta and may experience audio issues
- **Disclaimer**: The creators of this repository are not responsible for any costs or issues arising from its use

## Prerequisites
1. Set up your OpenAI API key as an environment variable: `OPENAI_API_KEY`
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Create a Weaviate account
4. Create a Weaviate vector database
5. Configure environment variables:
   - Rename `.env.example` to `.env`
   - Add your Weaviate credentials (VDB link and API key) to `.env`
6. Fill vector database with data:
   ```code
   python data/vector_setup.py
   ```

## Quick Start
Run the following command in your terminal:
```code
python conversation.py
```