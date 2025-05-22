Title: Data Flow Diagram (DFD) – Context Level

User → (Personal Information) → [ Anahata System (Process 0) ] → (Emotional Support) → User

System Description:
The Anahata system processes the user’s unbalanced emotions and tries to improve their emotional state by interacting in a personalized way.

Data Flow:
User → [ Anahata System ] → Insights → User



**Process of Our System:**

🔹 User Flow          🔹 Backend Process  
🔸 User Privacy      🔴 Developer Side Issues

1. User logs in by entering credentials into the system.
2. System authenticates user credentials.
3. User is redirected to the welcome screen and then taken to the mood questionnaire page (can answer or skip).
   - If the user answers the emotional questions, an emotional score is calculated based on input.
   - If the user skips, they can manually select their mood from predefined options.

📌 Emotional Score:
- Calculated by answering questions or selecting a predefined mood.
- Each mood option has a pre-assigned score.
  
4. User uploads a photo of their loved one (optional).
   - This photo is processed locally using a lightweight AI model to generate a memoji.
   - If skipped, a default emoji is used.

5. GPT API Call:
   - The system calls the GPT API so users can interact via voice or text.
   - [Note: GPT API pricing is still under review.]

6. For every few conversations, an emotional score is recalculated.
   - The UI dynamically adjusts based on the score (e.g., background color theme changes).

