# Using Prompts with ChatGPT

This guide explains how to use prompts from this repository with ChatGPT, including setting up Custom Instructions and GPTs.

## Using Prompts Directly

The simplest way to use our prompts with ChatGPT:

1. Go to [chat.openai.com](https://chat.openai.com)
2. Open the ChatGPT version of the prompt (e.g., `prompts/research/chatgpt.md`)
3. Copy the prompt
4. Paste it into ChatGPT
5. Follow the conversation flow

## Using Custom Instructions

Custom Instructions apply to all your ChatGPT conversations automatically.

### Setting Up

1. **Open Settings**
   - Click your profile icon (bottom-left)
   - Select "Settings"

2. **Find Custom Instructions**
   - Click "Personalization"
   - Select "Custom Instructions"

3. **Configure**
   There are two boxes:
   - **"What would you like ChatGPT to know about you?"** - Add context about yourself, your role, preferences
   - **"How would you like ChatGPT to respond?"** - Add response format preferences

4. **Add Prompt Instructions**
   Copy relevant portions of our prompts into the appropriate box.

### Example Setup

**About You:**
```
I'm a Product Manager at a tech startup. I write PRDs, user stories, and
release notes regularly. I prefer concise, actionable documentation.
```

**Response Style:**
```
- Use clear, professional language
- Structure responses with headers and bullet points
- Ask clarifying questions before long outputs
- Include examples when explaining concepts
```

## Creating a GPT

For frequently-used prompts, create a custom GPT:

### Steps

1. **Access GPT Builder**
   - Go to [chat.openai.com/gpts](https://chat.openai.com/gpts)
   - Click "Create a GPT"

2. **Configure the GPT**
   - **Name**: Give it a descriptive name (e.g., "PRD Writer")
   - **Description**: Explain what it does
   - **Instructions**: Paste the full prompt content here
   - **Conversation Starters**: Add example prompts users can click

3. **Set Capabilities**
   - Enable/disable web browsing, image generation, code interpreter as needed

4. **Save and Share**
   - Save your GPT
   - Optionally share with others via link

### Example GPT Configuration

**Name:** Research Assistant

**Description:** Helps conduct comprehensive research on any topic with intelligent source selection.

**Instructions:**
```
[Paste the ChatGPT version of the research prompt here]
```

**Conversation Starters:**
- "Research the latest trends in AI"
- "Help me understand the competitive landscape for..."
- "Find information about..."

## Tips for ChatGPT

### Be Explicit About Format
ChatGPT sometimes needs more explicit formatting instructions than Claude:
```
Format your response as:
1. Executive Summary (2-3 sentences)
2. Key Findings (bullet points)
3. Detailed Analysis (paragraphs with headers)
4. Sources (numbered list)
```

### Use Examples
ChatGPT responds well to examples:
```
Here's an example of the output format I want:

## Summary
[Brief overview]

## Details
- Point 1
- Point 2
```

### Chain Prompts
For complex tasks, break into steps:
1. First message: Set up the context and task
2. Second message: Provide specific inputs
3. Third message: Request the output

## Limitations vs Claude

| Feature | ChatGPT | Claude |
|---------|---------|--------|
| File Uploads | Yes | Yes |
| Web Browsing | Yes (Plus) | Limited |
| Code Execution | Yes (Plus) | No |
| Long Context | 128K | 200K |
| Custom Instructions | Yes | Yes (Projects) |
| API Access | Yes | Yes |

Choose based on your specific needs and the task at hand.
