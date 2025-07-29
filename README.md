# Basic-Prompts
Task 1: Zero-Shot & Role Prompting - The "Expert Summarizer"
Goal: Create a versatile prompt for summarizing various types of text efficiently, using zero-shot capabilities and simple role-playing.
Prompt Engineering Focus:
Zero-shot prompting for general summarization.
Role prompting to define the persona of the summarizer.
Instruction-based prompting for clarity.
Task Description:
Imagine you're building a tool that helps users quickly grasp the essence of long articles, emails, or reports.
Develop a single prompt that can summarize any given text.
Incorporate role-playing: Make the LLM act as a "Professional Content Analyst" or "Concise Reporter."
Specify constraints: The summary should be concise (e.g., 3-5 sentences or a maximum of 100 words) and capture the main points without losing critical information.
Test with 3 different texts:
A news article (e.g., about a recent tech development).
A scientific abstract.
A short, informal email.

Task 2: Few-Shot Prompting - The "Structured Data Extractor"
Goal: Build a prompt that can extract specific, structured information from unstructured text by providing examples.
Prompt Engineering Focus:
Few-shot prompting for pattern recognition.
Output format specification (e.g., JSON or bullet points).
Delimiter-based prompting to clearly separate examples and input.
Task Description:
You need to extract customer feedback data into a structured format for analysis.
Choose a specific entity type to extract (e.g., product name, customer sentiment, reported issue, customer location, contact email).
Create 3-5 high-quality few-shot examples where you show the LLM how to extract the chosen entity/entities from different review snippets and format them as desired (e.g., JSON or a clear Key: Value pair list).
Develop the final prompt including your examples and a clear instruction for the LLM to process new text.
Test with 3 new customer review snippets (that were not in your examples).

Task 3: Chain-of-Thought Prompting - The "Problem Solver"
Goal: Use Chain-of-Thought prompting to solve a multi-step reasoning problem and demonstrate the LLM's thinking process.
Prompt Engineering Focus:
Chain-of-Thought ("Let's think step by step") to elicit reasoning.
Analyzing the step-by-step output for correctness and clarity.
Task Description:
Select one of the following types of problems that requires logical reasoning:
A simple math word problem (e.g., "If Sarah has 5 apples and gives 2 to John, then buys 3 more, how many does she have?")
A common sense reasoning puzzle (e.g., "A bat and a ball cost $1.10 in total. The bat costs $1.00 more than the ball. How much does the ball cost?") - Be careful with this classic, LLMs can often get it wrong without CoT!
A logical inference task (e.g., "All birds can fly. A penguin is a bird. Can a penguin fly? Explain.")
Craft a prompt that asks the LLM to solve the chosen problem.
Crucially, add the CoT trigger phrase (e.g., "Let's think step by step." or "Walk me through your reasoning.").
Analyze the LLM's step-by-step output and its final answer. Note if the reasoning process leads to the correct answer.

Task 4: Iterative Prompt Refinement - The "Customer Support Chatbot Dialogue"
Goal: Simulate a customer support interaction and iteratively refine your prompts to guide the LLM towards a helpful and desired resolution.
Prompt Engineering Focus:
Iterative prompting / Multi-turn interaction.
Understanding and correcting LLM output in subsequent turns.
Role prompting (e.g., "You are a helpful customer support agent").
Handling common issues (e.g., missing information, misunderstanding context).
Task Description:
You'll play both the customer and the prompt engineer.
Initial Scenario: A customer has a common issue with a hypothetical product/service (e.g., "My internet is not working," "I can't log in to my account," "My order hasn't arrived").
Start with an initial prompt for the LLM to act as a customer support agent.
Engage in 3-5 turns of dialogue (prompting the LLM, then using its response to inform your next prompt).
Turn 1: Customer states the problem.
Turn 2: LLM (as agent) responds. Your prompt should guide it to ask clarifying questions or suggest initial troubleshooting.
Turn 3+: Based on the LLM's previous response, refine your prompt to either provide more information, ask for a specific solution, or gently correct a misunderstanding. The goal is to steer the LLM towards a satisfactory resolution.
Document the full dialogue (your prompts and the LLM's responses) and analyze the evolution of the conversation.
