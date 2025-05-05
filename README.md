# Innovation Challenge Onboarding Assistant

A frontend-only web tool to guide users in launching crowdsourced innovation challenges, powered by HuggingFace AI.

## Features
- **Step-by-Step Guidance**: Hybrid chat/wizard interface for challenge setup.
- **AI Capabilities**: Summarization, question answering, rubric generation, prize recommendation via HuggingFace.
- **Support Requests**: Stored locally with user consent.
- **Ethics**: Consent for support, anonymized reviewers, fairness notes on AI outputs.
- **Usability**: Responsive, accessible, with inline help and progress bar.

## Technology Stack
- **Frontend**: HTML, CSS, JavaScript
- **AI**: HuggingFace Inference API (facebook/bart-large-cnn, deepset/roberta-base-squad2, distilgpt2)
- **Deployment**: Netlify

## Setup
### Local
1. Navigate: `cd frontend`
2. Serve: `python -m http.server 8080`
3. Open: http://localhost:8080
4. Ensure internet for HuggingFace API.
5. Update `index.html` with `HUGGINGFACE_API_KEY` (replace `YOUR_HUGGINGFACE_API_KEY`).

### Deployed
- **URL**: [Insert Netlify URL]
- Access via Netlify URL.

## Usage
1. Enter problem statement (e.g., “Sustainable packaging”).
2. Follow chat/wizard steps (goals, challenge type, etc.).
3. Use AI commands: `/summarize`, `/question [query]`, `/generate-rubric`, `/recommend-prizes`, `/validate-submissions`.
4. Edit AI outputs via “Edit” button.
5. Request support (requires consent; stored locally).

## Cost Coverage Report
- **HuggingFace**: Free tier
- **Netlify**: Free tier
- **Total Cost**: $0/month

## Ethics
- **Privacy**: Support requests stored locally only with consent.
- **Fairness**: AI outputs include “Review for fairness” note.
- **Anonymity**: Reviewers use anonymized IDs.

## Limitations
- Local storage for support requests (resets on page refresh).
- HuggingFace free tier may have rate limits or delays.
- Client-side API key exposure (mitigated in production via environment variable).

## Future Enhancements
- Add backend for persistent support request storage.
- Use advanced HuggingFace models for better AI responses.
- Implement localStorage for persistent state.

## Deployment
- Hosted on Netlify with `HUGGINGFACE_API_KEY` as environment variable.
- Repo: [Insert GitHub URL]
