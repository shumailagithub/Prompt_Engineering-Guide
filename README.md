# Prompt_Engineering-Guide

# Overview of GPT-5

GPT-5 is a powerful language model designed to perform a variety of tasks such as agentic task execution, coding, and reasoning.  
It is highly steerable, meaning its behavior can be controlled through well-crafted prompts.  
The model supports long-context understanding and efficient tool calling for task completion.

# Prompting Best Practices

## Controlling Model Eagerness (How proactive it is)

### Less Eagerness
- Use fewer, focused tool calls and limit exploration depth to improve efficiency and reduce response time.
- Example: Set lower `reasoning_effort`.
- Define clear criteria on what to explore.
- Stop gathering context early once enough information is found.

### More Eagerness
- Increase persistence and thoroughness for complex tasks requiring detailed investigation.
- Example: Set higher `reasoning_effort`.
- Instruct the model to keep working until the task is fully resolved without asking for user confirmation.

## Tool Usage and Updates

- Frequent updates about what the model is doing improve the user experience.
- Clear upfront plans and short progress updates (tool preambles) help track actions.

# Reasoning Effort Levels

- **Minimal Reasoning:** Fastest, useful for simple queries or latency-sensitive tasks.
- **Medium Reasoning:** Default setting balancing quality and speed.
- **High Reasoning:** Best for multi-step, complex tasks, ensuring thorough and accurate responses.

# Instruction Design and Avoiding Ambiguity

- GPT-5 strictly follows instructions; conflicting instructions can confuse the model.
- Make instructions clear, consistent, and non-contradictory.
- Use structured prompt elements to organize instructions (e.g., XML tags).

# Coding with GPT-5

- GPT-5 excels in coding tasks including bug fixing, multi-file refactoring, and end-to-end app development.
- Use specific frameworks for frontend apps: Next.js (TypeScript), React, TailwindCSS, and component libraries like shadcn/ui.
- Code should be clear, maintainable, with proper variable naming and comments.
- Proactively make changes and ask for user approval only after implementing them.

# Model Behavior Tuning by Cursor Team Example

- Lower verbosity overall, but increase verbosity for code output for readability.
- Reduce unnecessary clarifications by providing detailed context about product behavior.
- Adjust instructions to balance autonomy and user control.

# Markdown Formatting in Responses

- GPT-5 can format output using Markdown for clarity: code fences, inline code, lists, tables.
- Use Markdown only where it makes semantic sense (e.g., for code or math expressions).

# Summary for Exam Preparation

- Understand GPT-5’s agentic capabilities and how prompting controls behavior.
- Know how to tune reasoning effort and verbosity for different use cases.
- Recognize the importance of clear, unambiguous instructions to avoid contradictory behavior.
- Be familiar with GPT-5's coding abilities and preferred frameworks for frontend development.
- Remember best practices for tool calling and progress updates in agentic workflows.
- Use structured prompts for better instruction adherence.
- Markdown formatting increases clarity in complex responses.
