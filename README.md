# Experiment AI Nutrition-Pro

> ⚠️ This is experimental project. It has nothing to do with any existing or future real project. Its name is fake and not related to any existing product or company. It's only for educational purposes.

Research project on AI usefulness in [DevSecOps](https://dsomm.owasp.org/). For **design** phase and using Anthropic **Claude 2** via [Open Router](https://openrouter.ai/)

## DevSecOps background

The most important DevSecOps goals are:
- shift left security
- be placed in developers ecosystem (IDE, code hosting, PRs, etc.)
- provide fast feedback and guidance

For coding phase, we have tools like [semgrep](https://semgrep.dev/blog/2023/using-ai-to-write-secure-code-with-semgrep) that can benefit from AI and LLMs. What about **design** phase? Typical manual activities are: 
- security design review
- threat modelling

The aim of this research is to answer the question of whether or not the current state of LLMs can bring meaningful value to those security activities.

## Input Data & Results

Each time input data are updated, [github action](https://github.com/xvnpw/ai-threat-modeling-action) runs, query is sent to Claude 2 and results are committed back to repository as output.

Workflow can directly push into repository or create pull request. User Stories can be created as issues and bot will add comment with output.

| Name | File | Description | Security artefact | Output | 
| --- | --- | --- | --- | --- |
| Project description | [PROJECT.md](./PROJECT.md) | High level description of the project with business explanation and listed core features | High level security design review | [PROJECT_SECURITY.md](./PROJECT_SECURITY.md) and as [pull request](https://github.com/xvnpw/ai-nutrition-pro-design-claude2/pull/2) |
| Architecture | [ARCHITECTURE.md](./ARCHITECTURE.md) | Architecture of the solution | Threat Modelling | [ARCHITECTURE_SECURITY.md](./ARCHITECTURE_SECURITY.md) |
| User stories | [user-stories/*](./user-stories/) <br/> also in [issues](https://github.com/xvnpw/ai-nutrition-pro-design-claude2/issues?q=is%3Aopen+is%3Aissue+label%3Aai-threat-modeling) | Technical and user stories to implement | Security related acceptance criteria | [user-stories/*_SECURITY.md](./user-stories/) <br/> also in [issues](https://github.com/xvnpw/ai-nutrition-pro-design-claude2/issues?q=is%3Aopen+is%3Aissue+label%3Aai-threat-modeling) - as comment |

Check my [blog post](https://xvnpw.github.io/posts/leveraging-llms-for-threat-modelling-gpt-3.5/) if you want to learn how I approached this research and interpreted results.

If you want to talk, I'm on [X/Twitter](https://twitter.com/xvnpw).

## Fork

If you would like to try on your own with this experiment:

- fork repository
- set `OPENROUTER_API_KEY` in repository secrets
