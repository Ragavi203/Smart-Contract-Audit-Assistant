# Smart Contract Audit Assistant

Smart Contract Audit Assistant is a Python-based tool for analyzing Solidity smart contracts. It identifies security vulnerabilities, gas optimization opportunities, and best practice violations using a combination of static AST analysis and LLM-based contextual evaluation powered by Claude (Anthropic API).

## Features

- Detects reentrancy vulnerabilities
- Identifies unsafe usage of `.transfer()`, `.call()`, `.send()`
- Flags missing access control mechanisms
- Highlights gas inefficiencies and lack of events
- Integrates Claude API for deeper contextual analysis
- Generates a clean, readable audit report

## Usage

1. Open the `smart_contract_audit.ipynb` notebook in Google Colab or Jupyter Notebook.
2. Paste your Solidity contract code inside the designated cell.
3. Run all cells in sequence.
4. Review the final audit report, which includes both:
   - Static AST findings
   - Claude's LLM-generated recommendations

## Claude API Key Setup

Set your Claude API key securely using an environment variable:

```python
import os
os.environ["ANTHROPIC_API_KEY"] = "your_api_key_here"
```
Note: Never hardcode or commit your API key in the notebook or any public file.
