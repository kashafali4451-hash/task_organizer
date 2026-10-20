# AI Task Organizer (LangGraph + Gemini)

Turns an informal message like
"I need to finish my assignment tomorrow, buy groceries today, and prepare for my meeting next week."
into an organized, prioritized to-do list.

## Workflow
```
User input -> Node 1: Task extraction (Gemini)
           -> Node 2: Task prioritization (High/Medium/Low, Gemini)
           -> Node 3: Format results
           -> END (Organized to-do list)
```

## Setup
1. `python -m venv venv` then activate it
   - Windows: `venv\Scripts\activate`
2. `pip install -r requirements.txt`
3. Copy `.env.example` to `.env` and put your Gemini API key
   (get one free at https://aistudio.google.com/apikey)
4. `python main.py`

## Example output
```
========================================
        YOUR ORGANIZED TO-DO LIST
========================================
1. 🔴 [High] Buy groceries (today)
2. 🔴 [High] Finish assignment (tomorrow)
3. 🟡 [Medium] Prepare for meeting (next week)
========================================
```
