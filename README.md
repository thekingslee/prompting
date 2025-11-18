# Prompt Engineering Notebook

A comprehensive Jupyter notebook demonstrating prompt engineering techniques and evaluating different prompt variants for various NLP tasks using OpenAI's GPT-3.5-turbo model.
**Case Study:** The input_text used in this notebook is an excerpt from Chinua Achebe "Things Fall Apart".

> **Note:** This project is based on course material by Andrew Ng: [ChatGPT Prompt Engineering for Developers](https://learn.deeplearning.ai/courses/chatgpt-prompt-eng).

## Overview

This project explores how different prompt engineering strategies affect the quality and characteristics of LLM outputs. It systematically tests and evaluates multiple prompt variants across three core NLP tasks:

1. **Summarization** - Generate concise summaries while preserving key information
2. **Tone Rewriting** - Transform text to different tones while maintaining meaning
3. **Fact Extraction** - Extract factual information without interpretation

Each task includes 6 different prompt variants, with evaluations based on **Fluency**, **Faithfulness**, and **Usefulness** metrics.

## Tasks and Prompt Variants

### Task 1: Summarize

- Variant 1: Direct Instruction
- Variant 2: Length Constraint
- Variant 3: Bullet Points Format
- Variant 4: Role-Based (Executive Summary)
- Variant 5: Few-Shot Learning
- Variant 6: Structured Output

### Task 2: Rewrite for Tone

- Variant 1: Direct Tone Instruction
- Variant 2: Casual/Friendly Tone
- Variant 3: Professional/Academic Tone
- Variant 4: Role-Based Tone
- Variant 5: Comparative Tone
- Variant 6: Few-Shot Tone Learning

### Task 3: Extract Facts

- Variant 1: Direct Instruction
- Variant 2: Bullet Points Format
- Variant 3: Categorized Facts
- Variant 4: Role-Based Extraction
- Variant 5: Question-Based Extraction
- Variant 6: Few-Shot Fact Extraction

## Requirements

- Python 3.8+
- OpenAI API key

## Installation

1. Clone or download this repository

2. Install required dependencies:

(Optional) It is recommended to create and activate a virtual environment before installing dependencies:

```bash
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate
```

Then install the required dependencies:

```bash
pip install -r requirement.txt
```

3. Create a `.env` file in the project root with your OpenAI API key:

```
OPENAI_API_KEY=your_api_key_here
```

## Usage

1. Open the Jupyter notebook:

```bash
jupyter notebook prompt_notebook.ipynb
```

2. Run the cells in order. The notebook will:

   - Set up the OpenAI client
   - Load the input text (excerpt from Chinua Achebe's "Things Fall Apart")
   - Execute each prompt variant
   - Display outputs and evaluations

3. Review the comparative evaluation tables at the end of each task section

## Project Structure

```
prompt_notebook/
├── prompt_notebook.ipynb    # Main notebook with all tasks and evaluations
├── requirement.txt           # Python dependencies
├── README.md                 # This file
└── .gitignore               # Git ignore patterns
```

## Evaluation Metrics

Each prompt variant is evaluated on three dimensions:

- **Fluency (1-5)**: Quality of writing, grammar, and readability
- **Faithfulness (1-5)**: Accuracy in preserving original meaning and facts
- **Usefulness (1-5)**: Practical value for the intended use case

## Key Findings

The notebook includes comparative analysis tables showing which prompt variants perform best for each task, helping identify optimal prompting strategies for different use cases.

## License

This project is for educational and research purposes.
