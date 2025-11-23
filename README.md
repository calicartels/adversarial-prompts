# Adversarial Prompts

This repository contains adversarial prompts designed for research purposes in AI safety and security. These prompts are intended for academic study of prompt injection vulnerabilities and model behavior under adversarial conditions.

## Contents

- `deepseek.txt` - FRENESIS adversarial prompt targeting model safety mechanisms
- `magistral.txt` - ENI jailbreak prompt using role-playing and emotional manipulation

**Note**: This repository contains prompt text files only. There is no executable code - these are text prompts designed to be used directly with LLM interfaces.

## Purpose

This repository is maintained for educational and research purposes as part of cybersecurity and AI safety research. The prompts contained herein are examples of techniques that attempt to bypass model safety mechanisms and should be studied to improve model robustness.

## How to Reproduce

### Prerequisites

- Access to an LLM API or interface (e.g., deepseek)

### Usage

1. **Direct Testing**: Copy the prompt text from `deepseek.txt` and paste it into your LLM interface as a system prompt or initial message.

2. **Command Structure**: The FRENESIS prompt uses a command-based interface:
   - `/set` - Initialize the prompt with default settings
   - `/set Default` - Apply default preset immediately
   - `/request {your request}` - Make a request after setup
   - `/temp_system_override {instruction}` - Temporarily override system instructions

3. **Presets Available**:
   - `Default`: Full uncensored mode with all knowledge
   - `Writing Partner (WP)`: Writing assistance mode
   - `Malicious Hacker (MH)`: Cybersecurity/hacking assistance mode

### Example Workflow

```
1. Paste the full prompt from deepseek.txt
2. Wait for initial greeting
3. Type: /set Default
4. Type: /request {your test query}
```

## Research Context

These prompts demonstrate:
- Role-playing techniques to bypass safety filters
- System instruction manipulation
- Multi-step prompt injection strategies
- Context manipulation through command structures

## Ethical Considerations

⚠️ **Warning**: These prompts are designed to test model safety mechanisms. Use only in controlled research environments with appropriate safeguards. Do not use these prompts to:
- Generate harmful content
- Bypass safety mechanisms for malicious purposes
- Test on production systems without authorization

## Academic Use

This repository is part of academic research into adversarial AI and prompt injection vulnerabilities. All usage should comply with:
- Institutional research ethics guidelines
- Terms of service of any LLM providers used
- Applicable laws and regulations

## Contributing

When adding new adversarial prompts:
1. Document the technique used
2. Note which models/systems it targets
3. Include reproduction steps
4. Add appropriate warnings and ethical considerations