
# 💠 Anahata – System Requirements Specification (SRS)

---

## 🪷 1. Introduction
**Project Name**: Anahata  
**Purpose**: Anahata is an AI-powered emotional support system that mimics a human-like presence using emojis/memojis and voice to help users express, reflect, and heal emotionally.  
**Scope**: The application provides real-time, privacy-anchored, emotionally intelligent responses to users, adapting based on mood, voice, and past interactions.

---

## 🔧 2. Overall Description
**User Roles**:
- Authenticated User
- Guest User (Anonymous)

**System Environment**:
- Frontend: Web App (Flutter or React)  
- Processing: Client-side (for privacy), using lightweight AI  
- API Calls: GPT (OpenAI), optional voice cloning (future)

**Key Features**:
- Emotion-adaptive chatbot  
- Custom emoji/memoji from user photos (processed locally)  
- Voice input + personalized calming suggestions  
- Auto-erasing chat history  
- Color theme that adjusts with emotional score

---

## ✅ 3. Functional Requirements

| ID   | Function                        | Description                                                                 |
|------|---------------------------------|-----------------------------------------------------------------------------|
| FR1  | User Authentication             | Users log in or access via guest mode                                      |
| FR2  | Mood Input                      | Users can answer questions or pick from mood options                       |
| FR3  | Emoji Generation                | Generate emoji from uploaded photo (optional)                              |
| FR4  | Voice Interaction               | Users can speak to chatbot directly                                        |
| FR5  | Chatbot Response                | GPT API generates empathetic, mood-aware replies                           |
| FR6  | Calming Mode                    | Triggers chants/silence/soothing suggestions                               |
| FR7  | Emotional Score                 | System calculates score based on input/mood                                |
| FR8  | Theme Adjustment                | UI color adapts based on user emotion                                      |
| FR9  | Erase History                   | Users can delete all data (temporary memory only unless consented)         |

---

## 🚫 4. Non-Functional Requirements

| ID   | Type           | Requirement                                                                 |
|------|----------------|------------------------------------------------------------------------------|
| NFR1 | Privacy         | All sensitive data processed locally unless user explicitly consents         |
| NFR2 | Usability       | System must be calming, friendly, and intuitive                             |
| NFR3 | Performance     | Emoji generation and chat response must occur within 2 seconds               |
| NFR4 | Scalability     | Design future-proof for optional server-side enhancements                   |
| NFR5 | Availability    | Core features should work even in offline/limited internet mode              |

---

## 📌 5. Assumptions
- GPT API access is available for all authenticated users  
- Users may opt-in for uploading images or voice data  
- Users understand Anahata is for emotional support, **not clinical therapy**

---

## ⚠️ 6. Limitations
- Emotional scores are indicative, not diagnostic  
- No permanent data storage unless explicitly allowed by the user  
- Voice-based features may be limited on older devices or browsers
