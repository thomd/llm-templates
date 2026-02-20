# Templates for LLM

To be used with the [llm CLI](https://llm.datasette.io/en/stable/) and the [llm-templates-github](https://github.com/simonw/llm-templates-github) plugin.

## Usage Examples

Create a git alias


    git config --global alias.cimm '!f() { git diff --cached | llm -t gh:thomd/commit-message | git commit -F -; }; f'


and commit staged changes with a LLM generated commit message with

    git cim
