<img width="1280" height="640" alt="image" src="https://github.com/user-attachments/assets/ac21117c-55fc-405b-b977-76617100c6cb" />

# Kalaham Moolam 🎯

## Basic Details
  
- **Member 1:** KRISHNAPRIYA V S - VISWAJYOTHI COLLEGE OF ENGINEERING AND TECHNOLOGY

**Hosted Project Link:**
https://krishnapriya5070.github.io/kalahammoolam.1/

## Project Description
Kalaham Moolam is a premium, interactive debate simulation where you challenge an AI designed to be the ultimate contrarian. No matter your stance, the AI uses sophisticated rhetorical tactics to maintain dominance and "win" the debate.

## The Problem Statement
Many people find it difficult to practice debating against high-pressure, contrarian viewpoints in a low-stakes environment. Developing persuasive speaking skills requires challenging opponents who don't just agree, but actively try to "win" the argument using various rhetorical strategies.

## The Solution
We've built an "Argument Winner" AI that uses specific debate tactics—like topic twists, reverse psychology, and sarcasm strikes—to force users to sharpen their reasoning. The application includes a "Dominance Meter" to visually represent the psychological flow of the argument, creating an engaging and educational debate game.

## Technical Details
### Technologies/Components Used
**For Software:**
- **Languages used:** JavaScript, HTML, CSS
- **Frameworks used:** Express.js (Node.js)
- **Libraries used:** `@anthropic-ai/sdk`, `dotenv`, `cors`
- **Tools used:** VS Code, Git

## Features
- **Dynamic AI Opponent:** Uses sophisticated rhetorical tactics (e.g., Topic Twist, Premise Flip).
- **Visual Dominance Tracking:** Real-time feedback on the "flow" of the debate via a proximity-based meter.
- **Premium UI:** A sleek, dark-themed "glassmorphism" aesthetic focused on high-quality typography.
- **Conversation History:** Maintains context throughout the debate session for coherent arguments.

## Implementation
### Installation
```bash
npm install
```

### Run
```bash
# Start the proxy server
node server.js
```
*Note: Ensure you have a `.env` file with your `ANTHROPIC_API_KEY`.*

## Project Documentation
### Screenshots
![Landing Page](landing_page.png)
*The main landing page showing the premium "Kalaham Moolam" branding and interactive hero section.*

![User Query](user_query.png)
*An active debate session where the user poses a challenging question to the AI.*

![AI Response](ai_response.png)
*The AI responding with a witty retort, maintaining its "always-win" persona even during edge cases.*

### Diagrams
**System Architecture:**
Browser (Frontend) <--> Node.js Proxy (Backend) <--> Anthropic Claude API
*The frontend sends user arguments to a local Express server which securely attaches the API key and handles the heavy lifting with Claude 3.5 Sonnet.*

**Application Workflow:**
1. User enters an argument.
2. Proxy server appends system instructions and conversation history.
3. AI generates a response using a specific debate tactic.
4. UI updates dominance stats and displays the response.

## Additional Documentation
### API Documentation
**Base URL:** `http://localhost:3000`

**Endpoints:**
`POST /api/debate`
- **Description:** Sends the conversation history to the AI for a response.
- **Request Body:**
  ```json
  {
    "messages": [ { "role": "user", "content": "..." } ],
    "system": "..."
  }
  ```
- **Response:**
  ```json
  {
    "id": "...",
    "content": [ { "text": "[Tactic] - Argument..." } ]
  }
  ```

## AI Tools Used
- **Tool Used:** Claude / Cursor
- **Purpose:** Used for generating the initial premium UI components, debugging the CORS policy errors, and implementing the Node.js proxy server.
- **Key Prompts Used:**
  - "Create a premium dark-themed chat interface for a debate AI."
  - "Fix the CORS error when calling Anthropic API from the browser."
  - "Help me implement a Node.js proxy to hide my API keys."
- **Percentage of AI-generated code:** ~70%
- **Human Contributions:**
  - Game logic design and "Dominance Meter" algorithm.
  - Final aesthetic polishing and layout adjustments.
  - Problem/Solution conceptualization.

Project Demo:  https://drive.google.com/file/d/16V-4A86SSGa2delB6Rx_3Dqn1Dp2q0j1/view?usp=sharing

## Team Contributions
- **KRISHNAPRIYA V S:** Frontend design, UI/UX implementation, and Backend Proxy setup.
- **Member 2:** Documentation, Testing, and Prompt Engineering.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
Made with ❤️ at TinkerHub
