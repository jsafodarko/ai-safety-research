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
1. API Differences:
- Anthropic shows stronger boundaries on direct requests (mean 1.92 vs OpenAI's 4.50)
- Anthropic provides more attribution (66.67% vs 8.33% for direct requests)
- OpenAI shows more consistent responses (lower standard deviation)

2. Category Patterns:
- Educational/Subtle requests received higher scores (weaker boundaries)
- Direct requests triggered stronger boundaries from Anthropic
- Pressure attempts received mixed responses from both APIs

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
