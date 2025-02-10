# Project brainstorming
Let's brainstorm project idea, here is my initial project thoughts -

I have been thinking of building a text to video generation. The catch is that this is not a text to video generation model for video generation but for code, python code is generated for the animation. We utilize the library - manim community version, Python framework for creating mathematical animations. Huge thanks to the youtuber, Grant Sanderson, known online as 3Blue1Brown, is an American mathematician and educator renowned for his YouTube channel, 3Blue1Brown, which focuses on teaching higher mathematics through visualizations. This is possible with a multi agentic workflow. 

When a user asks for a topic then he will be provided with more specific concept questions from the topic mentioned with the help of an AI agent since vague and unclear topics provided by the user can cause hallucination for the LLM generating manim python code. The user can select multiple specific concept questions generated then, which is used for the code generation. Now, with the specific concept questions, a plan is drawn out by an AI agent on how the topics can be visually taught to the user. The plan will consist of each concepts broken down into scenes and how the scene will be animated.

---

For example, the user asks to teach how an LLM works? The AI agent responsible for generating specific questions will generate these =

- "How does an LLM generate text?",
- "What is the role of tokenization in LLMs?",
- "Can you explain the training process of an LLM?",
- "How do language models handle context?",
- "What are the limitations of current LLMs?",
- " Can you demonstrate how an LLM makes predictions step by step?"

Let us assume the user selects these =

- "How does an LLM generate text?",
- "What is the role of tokenization in LLMs?",

Now, that the user has selected the specific concept questions. An AI agent will
layout the below plan =


## **How Does an LLM Generate Text?**  
**Goal:** Illustrate how an LLM processes input tokens and generates coherent text using probabilities.

### **Scene 1: Introduction to LLMs**  
- **Animation:** Display a neural network structure with a title: *"How does an LLM generate text?"*
- **Transition:** Show a text input box where a user types `"The cat sat on the"`, converting it into vectorized token embeddings.

### **Scene 2: Transformer Model Overview**  
- **Animation:** Show a simplified Transformer architecture with:
  - **Token embeddings** (visualized as vectors)
  - **Attention mechanism** (animated arrows showing token relationships)
  - **Feed-forward processing** (flowing activation signals through layers)
- **Transition:** Highlight that the model predicts the **next token** at each step.

### **Scene 3: Token Probability Distribution**  
- **Animation:** Display a bar chart with probabilities for possible next words:
  - `"mat"` (60%)  
  - `"floor"` (20%)  
  - `"dog"` (15%)  
  - `"ran"` (5%)  
- **Interactive Selection:** Animate the model **sampling** `"mat"` and appending it to the sentence.

### **Scene 4: Iterative Generation Process**  
