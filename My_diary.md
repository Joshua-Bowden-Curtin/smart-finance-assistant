Test for diary

# Diary record

## Monday 15/6/2026

### Progress notes so far

I have been invistigating the components given in the assignment. I realised I needed background info on how they work. I did a tutorial on markdown and pandas to start with. Next up I plan to do a tutorial on jupyter notebook in colab because it all looks very confusing so far.

I have created a project folder in Claude where I can upload all of my assessment documentation to provide it context for generating understandable and context relevant code. I then asked it for recommendations for how to proceed with working on the assessment:
> Great learning project to pick up Colab/Jupyter basics. Here are the main workflows people use, roughly from most to least friction:
> 
> ---
> 
> **1. Chat directly in Colab (built-in Gemini)**
> Colab now has an AI assistant (Gemini) baked in — you can ask it to generate or explain cells right inside the notebook. The upside is it can see your existing code and context. The downside is it's Gemini-only and sometimes shallow on complex multi-cell logic.
> 
> **2. Give the whole notebook to an AI (your best option here)**
> Export/download the `.ipynb` file, then upload it to Claude, ChatGPT, etc. and say "fill in this notebook". This works well because the AI sees the full structure — existing markdown, instructions, cell order — and can return a completed version you re-upload to Colab. This is probably the **highest-leverage approach** for a structured assignment like this one, since the spec and starter skeleton are already well-defined.
> 
> **3. Iterative copy-paste (most common workflow)**
> Write a prompt describing what you want one cell or function to do, paste the output into Colab, run it, then paste errors back to the AI. Slower but gives you more control and you actually learn what's happening. Good for the "working in AI as a partner" angle this assignment is clearly teaching.
> 
> **4. Claude Artifacts / code canvas**
> Some AI tools (including this one) can write a full self-contained script you then adapt into notebook cells. You'd ask for "a Python function that does X" and then manually paste it into the right cell. Less notebook-aware but fine for individual components (the tool, the RAG logic, etc.).
> 
> **5. Claude Code / Cursor (local IDE approach)**
> If you install Jupyter locally and use an AI-integrated editor like Cursor, you get inline completions and multi-file awareness. Overkill for Colab-based learning but worth knowing exists.
> 
> ---
> 
> **Practical suggestion for this project:**
> 
> Given the structure (chat + RAG + tool + Gradio UI), I'd do it in phases:
> 
> - Get the starter notebook, then ask an AI to scaffold each of the four components one at a time (not all at once — easier to debug)
> - Run each piece in Colab as you go so you catch errors early
> - The `hands-on-ai` package and the specific Ollama base URL/key in the spec are the unusual constraints — make sure any AI you use is aware of those, since it won't know them from training
> 
> Want help understanding any specific component (RAG, Gradio, the six-step methodology, etc.)?
