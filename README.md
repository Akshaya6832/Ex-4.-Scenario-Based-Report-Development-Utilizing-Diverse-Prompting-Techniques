# Ex-4.-Scenario-Based-Report-Development-Utilizing-Diverse-Prompting-Techniques
Objective: The goal of this experiment is to design and develop an AI-powered chatbot that can handle customer inquiries, provide support, and improve customer experience in a retail environment. Create prompts using various AI prompting techniques to guide your experiment, data collection, analysis, and report creation.
## Aim: 
The overarching aim of this experiment is to meticulously demonstrate how the strategic application of different prompting techniques can be utilized to effectively guide and fine-tune an AI model within a specific, real-world retail scenario. The experiment will focus on developing a chatbot, named "RetailGenie," for a hypothetical online fashion and home goods store called "Chic & Cozy."

## Algorithm:
To achieve the objective, we adopted the following systematic approach:

Understanding Chatbot Requirements:
The chatbot must answer customer FAQs, track orders, provide product recommendations, and handle complaints politely.

Selection of Prompting Techniques:
We selected a wide range of prompting techniques — including Zero-shot, Few-shot, Chain-of-Thought, Role Prompting, and others — to cover different aspects of chatbot development.

Prompt Design:
For each technique, prompts were specifically designed to handle real-world customer scenarios such as order tracking, damaged item reporting, and delayed delivery.

Experimentation:
Each prompting technique was applied to the same scenario to evaluate how the chatbot responded.

Observation and Analysis:
We observed the quality, tone, and accuracy of the chatbot’s responses and compared the results to determine which techniques produced the best customer experience.

## Prompt:
These are the few types of prompting techniques/types:
**1. Zero-Shot Prompting**
Without giving examples, the chatbot was asked to respond directly to a query.
Prompt: “Where is my order #12345?”
Observation: The chatbot could respond, but tone consistency varied. Sometimes the response was too generic or robotic.

**2. One-Shot Prompting**
A single example was provided before asking the chatbot to respond to a new query.
Prompt Example:
“Example: Customer asks: Where is my order #98765? → Bot: Your order is out for delivery and will arrive tomorrow.
Now answer: Where is my order #12345?”
Observation: The chatbot’s response became more aligned with the expected format and tone.

**3. Few-Shot Prompting**
Multiple examples were given to set a clear pattern for the chatbot to follow.
Observation: This significantly improved the chatbot’s tone and consistency. It maintained a polite, professional style even for new queries.

**4. Chain-of-Thought Prompting**
The chatbot was instructed to think step by step before answering.
Prompt Example:
“The customer says they received a damaged item. Think step by step: 1) Apologize, 2) Ask for details, 3) Offer a replacement.”
Observation: The responses became well-structured, covering all steps systematically.

**5. ReAct Prompting**
The chatbot was instructed to reason and then take action.
Prompt Example:
“Decide if a refund or replacement is more appropriate. Think first, then respond to the customer.”
Observation: This approach worked best for decision-making tasks like returns and refunds.

**6. Self-Consistency Prompting**
The chatbot generated multiple possible responses and selected the most appropriate one.
Observation: The final chosen response was usually more balanced and customer-friendly.

**7. Role Prompting**
The chatbot was given a role to play.
Prompt Example:
“You are a polite and empathetic customer service agent. Help the customer track their order.”
Observation: This produced highly natural, professional, and empathetic replies.

**8. Tree-of-Thought Prompting**
The chatbot was encouraged to explore multiple solutions before picking the best one.
Prompt Example:
“Generate three ways to resolve a delayed shipment: (1) Apologize and offer a discount, (2) Offer a replacement, (3) Give updated ETA. Choose the best option.”
Observation: The chatbot became more creative and considered customer satisfaction while deciding.

**9. Reflection Prompting**
The chatbot was asked to review and refine its own response.
Prompt Example:
“Here’s your answer: <response>. Make it more polite and professional.”
Observation: The response quality improved significantly, with more polished and customer-friendly wording.

**10. Multimodal Prompting**
Text and image were combined.
Example: Uploading a product image and asking: “Is this available in blue?”
Observation: Useful for product-related queries but requires an image database.

**Scenario :**
A customer reports a damaged item and wants a resolution.
We will provide the same situation to both prompting techniques and compare outputs.

**Technique 1 : Few-Shot Prompting**
Classify and respond to customer complaints in a polite, solution-oriented way.
Example 1:
Customer: My order was late.
Bot: I'm really sorry your order was delayed. I have checked and it will reach you today. Thank you for your patience!

Example 2:
Customer: I received the wrong item.
Bot: I apologize for the mix-up! I have initiated a replacement request. You will receive the correct item within 3-4 working days.
Customer: I received a damaged item.

**Technique 2 : ReAct Prompting**
Customer: I received a damaged item.
Reason step by step:
1. Identify the type of complaint (damaged product).
2. Decide whether to offer a refund or a replacement (replacement is better for customer satisfaction).
3. Respond politely and take action.

## Output:
**Technique 1 :**
Bot: I’m very sorry to hear that your product arrived damaged. I have initiated a replacement request at no extra cost. 
You will receive the new item within 3-4 working days. 
Would you like me to arrange a pickup for the damaged product?

Observation:
Polite, structured, and aligned with the examples given.
Maintains consistency and professional tone.
Automatically suggests a solution without needing extra clarification.

**Technique 2 :**
Reasoning: The complaint is about a damaged item. Offering a replacement is better than refund because it retains the sale 
and keeps the customer happy. We should apologize, confirm replacement, and ask for pickup details.

Final Response:
Bot: I’m sorry to hear your item was damaged. I have arranged a replacement for you at no cost. 
It will arrive within 3-4 business days. Could you confirm your address for the pickup of the damaged item?

Observation:
Explains reasoning before answering.
Chooses the most customer-friendly action.
Response is empathetic and actionable.

<img width="886" height="390" alt="Screenshot 2025-09-09 075902" src="https://github.com/user-attachments/assets/0f125f96-1a8e-4dca-9353-b35f3413a250" />

## Result:
Both techniques improved the chatbot’s response quality compared to a simple zero-shot prompt:
Few-Shot Prompting ensures consistency and tone alignment when many examples are available.
ReAct Prompting is more dynamic and can adapt to new or complex problems where reasoning is important.
For a retail chatbot, combining both techniques would be ideal: use Few-Shot for common FAQs and ReAct for complaints, refunds, or complex decision-making.
