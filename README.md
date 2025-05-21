# Exno.3-Scenario-Based Report Development Utilizing Diverse Prompting Techniques
### DATE:21.05.2025                                                                            
### REGISTER NUMBER : 212222060042

### Aim: To design an AI-powered chatbot that assists customers in resolving issues related to product troubleshooting, order tracking, and general inquiries. The chatbot should handle various customer queries efficiently while maintaining a conversational and user-friendly tone. In this experiment, we will employ different prompt patterns to guide the development process of the chatbot, ranging from basic task-oriented prompts to more complex, persona-driven prompts.

### Algorithm:  1. Direct Instruction Prompts
Objective: Guide the chatbot to respond concisely to customer inquiries.
Prompt Pattern:
Prompt: "When a customer asks for the status of their order, reply with: 'Your order is currently being processed and will be delivered by [date].'"
2. Contextual Prompting
Objective: Incorporate specific context to provide detailed answers based on the user’s previous interaction.
Prompt Pattern:
Prompt: "If the customer previously mentioned that they haven’t received their order, say, 'I see that you mentioned your order hasn't arrived yet. Let me check the details for you and get back shortly.'"
3. Persona-Based Prompting
Objective: Design the chatbot to adopt a specific persona, making the interaction more engaging.
Prompt Pattern:
Prompt: "Pretend you are a friendly, helpful customer service representative. Use a conversational tone, such as 'Hey there! I’m here to help with any questions you might have. Let’s get your issue sorted!'"

**4. Few-Shot Prompting**

Objective: Teach the AI how to respond using a few examples, enabling it to generalize for similar situations.

**Prompt Pattern:**

**Prompt:** "Here are some examples of how to handle technical questions:
'My phone isn't charging.' → 'Have you tried using a different cable? If that doesn’t work, it may be an issue with the port.'
'The screen is flickering.' → 'It sounds like a display issue. Have you tried restarting the device?'
Now, respond to: 'My app keeps crashing.'"

**5. Chain of Thought Prompting**

Objective: Use a step-by-step reasoning approach for resolving more complex or technical issues.

**Prompt Pattern:**

**Prompt:** "When a customer reports their laptop overheating, guide them through the following steps:
Ask if they are using the laptop on a soft surface.
Suggest moving the laptop to a flat, hard surface for better airflow.
Ask if they’ve cleaned the vents recently.
Recommend restarting the device to see if the issue persists.
Now, solve: 'My laptop fan is making a loud noise.'"

**6. Instruction with Constraints**
Objective: Instruct the chatbot to provide assistance while adhering to specific constraints (e.g., response length or tone).

**Prompt Pattern:**

**Prompt:** "Respond to order inquiries in no more than 50 words and avoid using technical jargon. For example, 'Your order is on the way and should arrive by [date]. Feel free to reach out if you need anything else.'"

**7. Reflective Prompting**
Objective: Ensure that the chatbot reflects the user’s query back to them before providing a response, reducing misunderstandings.

**Prompt Pattern:**

**Prompt:** "When a customer asks for help, first reflect their question back to them. 
For example, if they ask 'How can I reset my password?' respond with 'You're asking how to reset your password, correct? Here’s how you can do it.'"

Procedure: AI-Powered Chatbot Development Using Prompt Patterns
Step 1: Define Use Cases and Scope
Identify the main functionalities of your chatbot:

Product troubleshooting

Order tracking

General customer inquiries

Define boundaries: What the chatbot can and cannot handle (e.g., no payment processing).

Step 2: Choose Your Platform
Decide where the chatbot will live (e.g., website, WhatsApp, Messenger).

Choose a backend or tool (e.g., OpenAI API, Dialogflow, Microsoft Bot Framework, Rasa).

Step 3: Design Prompt Templates by Pattern
1. ✅ Direct Instruction Prompts
Goal: Give clear instructions to generate concise, task-focused replies.

Example Implementation:

Trigger: "Where is my order?"

Response Template:
"Your order is currently being processed and will be delivered by [date]."

2. 🧩 Contextual Prompting
Goal: Use customer history or previous messages for better response relevance.

Example Implementation:

If history shows: “My order hasn’t arrived.”

Response Template:
"I see that you mentioned your order hasn't arrived yet. Let me check the details for you and get back shortly."

3. 😃 Persona-Based Prompting
Goal: Make the bot sound human-like, friendly, and brand-consistent.

Example Implementation:

Prompt Style:
"Hey there! I’m here to help with any questions you might have. Let’s get your issue sorted!"

4. 📚 Few-Shot Prompting
Goal: Train the model on a few sample cases so it can generalize new ones.

Steps:

Provide 2–3 examples of user queries and ideal responses.

Ask the bot to generate a reply for a new but related case.

Example:

sql
Copy code
'My phone isn't charging.' → 'Have you tried using a different cable?...'
'The screen is flickering.' → 'It sounds like a display issue...'
'My app keeps crashing.' → ?
5. 🧠 Chain of Thought Prompting
Goal: For complex problems, guide the bot through multi-step reasoning.

Example:

User: "My laptop fan is making a loud noise."

Bot Thinking Steps:

Ask about surface usage

Recommend airflow-friendly placement

Ask about vent cleaning

Suggest restart

Response: "Let's troubleshoot that. First, are you using your laptop on a soft surface like a bed or couch?..."

6. 📏 Instruction with Constraints
Goal: Guide tone and structure, like keeping responses short or avoiding jargon.

Rule: Limit reply to 50 words, no tech terms.

Example:
"Your order is on the way and should arrive by [date]. Feel free to reach out if you need anything else."

7. 🪞 Reflective Prompting
Goal: Confirm user query to prevent misunderstanding.

Example:

User: "How do I reset my password?"

Response:
"You're asking how to reset your password, correct? Here’s how you can do it..."

Step 4: Implement Prompt Logic in Code or Platform
Map each prompt type to specific intent recognition.

Example logic:

python
Copy code
if "order status" in user_input:
    apply_direct_instruction_prompt()
elif "hasn't arrived" in history:
    apply_contextual_prompt()
elif "reset password" in user_input:
    apply_reflective_prompt()
Step 5: Test Each Pattern
Use sample inputs for each scenario.

Evaluate for:

Accuracy

Tone consistency

Relevance

User satisfaction

Step 6: Refine & Add Fallbacks
Add fallback responses:

"I'm not sure I understood that. Could you rephrase it?"

Improve prompts based on common errors.

**Step 7: Deploy and Monitor**
Deploy the chatbot to your chosen platform.

Use analytics to track:

Query types

Response success

Drop-off rates

**Step 8: Continuous Learning**
Periodically re-train or fine-tune prompt responses.

Collect user feedback to improve tone and usability.

# Result: Thus the Prompts were exected succcessfully .

