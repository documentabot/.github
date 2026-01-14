### Write Code, Not Docs 📝

Introducing **Documentabot**, your AI assistant that will automatically keep your docs up-to-date by analyzing code changes and intelligently updating documentation files.

Works with README, API docs, guides, and any markdown files you specify. Intelligent, configurable, and perfect for teams who value good documentation but lack time to maintain it manually.

With **Documentabot**, you'll never let your documentation fall behind again.

## How It Works

1. Install **Documentabot** on any repos you like and set the [configuration](#configuration-guide) file.
2. Commit your code changes as usual to your intended branch.
3. **Documentabot** analyses your code changes and existing documentation files.
4. If updates are necessary, a PR with suggested docs updates will be created.
5. Review and merge the PR, so you will keep full control over what gets published.

## Key Features

🐙 **Polyglot Assistant**: Write your code in any programming language you prefer and write your docs in any language you speak. There is literally no language barrier when interacting with **Documentabot**.

🧠 **Intelligent Updates**: Every update will be adjusted accordingly to match your formatting, tone, and structure. Readers will never figure out that **Documentabot** is the one who monitors your docs.

📊 **Detailed Reports**: See exactly what changed and why. A comprehensive analysis report will be shown in the PR description made by **Documentabot** to help you make informed decisions about the updates.

😎 **Zero Maintenance**: Set it up once and forget about it. We built **Documentabot** to help you focus on your code, not your docs.

## Configuration Guide

For further customization, create a file named `.github/documentabot.yml` in your repository. It is not necessary to create one if all you want is for **Documentabot** to monitor all your code changes on your main branch and updates your README.md accordingly.

Here is the complete configuration file with all available keys:

```yaml
### Name of the branch you want to monitor (optional).
### Default to main or master branch.
target-branch: main

### List of all your documentation directories (optional).
### Default to README.md. Currently supports file paths only, not directory paths.
doc-paths:
 - README.md

### List of all the directories you want to ignore (optional).
### All changes that happened inside these directories will not be reviewed. Supports wildcards (*).
ignore-paths:
 - .github/**

### List of all the users you want to ignore (optional).
### All commits made by these users will not be reviewed.
ignore-users:
 - your-intern
```

Ready to automate your documentation? Install now at Github Marketplace.
