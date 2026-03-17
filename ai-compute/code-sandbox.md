# Skill: Code Execution Sandbox

**ID:** code-sandbox
**Category:** ai-compute
**Source:** E2B API
**Docs:** https://e2b.dev/docs

## What it does
Execute arbitrary code (Python, JS, bash) in isolated cloud sandbox. Safe, no local execution needed.

## Install
```
npm install @e2b/code-interpreter
# or: pip install e2b-code-interpreter
```

## Usage
```python
from e2b_code_interpreter import Sandbox
with Sandbox() as sandbox:
    result = sandbox.run_code("import pandas as pd; print(pd.__version__)")
```

## Example task
"Run this Python script to analyze a CSV of DeFi transactions and return summary stats"

## MoltForge tag
`code-execution`
