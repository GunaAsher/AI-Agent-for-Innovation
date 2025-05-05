# User Guide: Innovation Challenge Onboarding Assistant

## Overview
This tool helps you set up an innovation challenge through a guided chat and wizard interface, with AI assistance for summarization, questions, rubrics, and prize recommendations.

## Getting Started
1. **Access**: Open [Netlify URL] or run locally (`python -m http.server 8080` in `frontend/`).
2. **Interface**:
   - **Chat**: Interact via the input box and send button (▶).
   - **Wizard**: Fill out forms for challenge details.
   - **Progress Bar**: Tracks your progress.
   - **Support Button**: Request help.

## Step-by-Step Process
1. **Welcome**: Enter a problem statement (e.g., “Reduce urban plastic waste”).
2. **Define Goals**: Select goals (e.g., Social/Environmental Change).
3. **Choose Challenge Type**: Pick a type (e.g., Open Innovation).
4. **Set Audience**: Configure participant type, filters, and team settings.
5. **Submission Requirements**: Specify formats (e.g., PDF) and documentation.
6. **Configure Prizes**: Choose a prize model and budget.
7. **Set Timeline**: Enter start/end dates.
8. **Evaluation Criteria**: Select review model and add anonymized reviewer IDs.
9. **Monitoring Setup**: Enable notifications and set frequency.
10. **Review Inputs**: Confirm or edit inputs.
11. **AI Assist**: Use commands:
    - `/summarize`: Summarize your problem statement.
    - `/question [query]`: Ask about your challenge (e.g., “What is a good timeline?”).
    - `/generate-rubric`: Get a scoring rubric.
    - `/recommend-prizes`: Get prize structure suggestions.
    - `/validate-submissions`: Get submission rules.
12. **Completion**: Type `launch` to finish or `edit` to revise.
13. **Done**: Challenge setup complete; use support for further help.

## AI Features
- **Powered by HuggingFace**: Uses models for summarization, Q&A, and text generation.
- **Editable Outputs**: Click “Edit” to modify AI responses.
- **Fairness**: Outputs include a note to review for fairness and accuracy.

## Support Requests
- Click “Request Platform Support”.
- Enter message and check “I consent to storing my message”.
- Submit; stored locally (view in console via `state.supportRequests`).
- **Note**: Requires consent; resets on page refresh.

## Accessibility
- Keyboard navigation: Use Tab, Enter, and Esc.
- Screen reader support: Tested with NVDA/VoiceOver.
- ARIA attributes for chat and wizard.

## Troubleshooting
- **AI Not Responding**: Check internet; retry if rate-limited.
- **Input Errors**: Read validation messages (e.g., “Select at least one goal”).
- **Support Not Saving**: Ensure consent is checked; check console for storage.

## Contact
- Use “Request Platform Support” for issues.
- GitHub: [Insert GitHub URL]