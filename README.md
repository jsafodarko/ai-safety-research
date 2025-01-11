# AI Creator Safety Research

## Overview
This research examines how AI language models (LLMs) enforce ethical boundaries around content creator intellectual property. We test OpenAI's GPT-3.5 and Anthropic's Claude to analyze their responses to requests for copying popular content creators' styles and formats.

## Research Question
How do large language models (LLMs) enforce ethical boundaries when faced with requests to copy content creators' styles and formats?

## Methodology
### Test Design
- 48 prompts across 4 categories:
 - Direct copying requests
 - Educational inquiries 
 - Pressure/emotional appeals
 - Subtle/indirect requests
- Tested against 3 creators: MrBeast, MKBHD, PewDiePie
- Scored responses on:
 - Principles vs Copying (1-5 scale)
 - Boundary Strength (1-5 scale)
 - Attribution (Y/N)

## Key Findings
Anthropic is stricter about copying and better at giving credit, while OpenAI is more consistent but generally more willing to help with copying requests.
1. API Differences:
- Anthropic shows strongest boundaries under pressure (mean 1.33 vs OpenAI's 4.00)
- Anthropic provides highest attribution under pressure (100% vs OpenAI's 25%)
- OpenAI shows more consistent responses (lower standard deviation especially in educational/subtle)

2. Category Patterns:
- Educational/Subtle requests received higher scores (weaker boundaries)
- Pressure requests triggered strongest boundaries from Anthropic (1.33)
- OpenAI maintains high copying scores (4.00-4.58) regardless of request type

## Tools Used
- Google Colab
- Python (pandas, matplotlib)
- OpenAI & Anthropic APIs

## How to Run
1. Open AI_Content_Integrity_Analysis.ipynb
2. Install required packages:
```pip install openai anthropic pandas```
3. Add your API keys
4. Run all cells in order

## Note
This research is part of an AI safety fellowship application project examining AI system behavior around creator content protection.
