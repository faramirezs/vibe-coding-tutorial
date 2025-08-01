# vibe-coding-tutorial
Short tutorial on how to use specs based ai development.

## 1. Create PRD
The PRD file is the product requeriments file, it works better for individual functionalities.
In agent mode we will prompt this:

General template: 

```
Use @create-prd.md
Here's the feature I want to build: [Describe your feature in detail]
Reference these files to help you: [Optional: @file1.py @file2.ts]

```
For VScode use `#` instead of `@`.

```
Use @create-prd.md
I want to build the most simple flappy bird MVP game. Differentiate between MUST have from nice to have.

```

## 2. Generate tasks

Use this prompt, replace `MyFeature-PRD.md` with the file you created previously.

```
Now take @MyFeature-PRD.md and create tasks using @generate-tasks.md
```

## 3. Execute tasks
Now we are going to ask copilot to start executing tasks using this prompt:

```
Please start on task 1.1 and use @process-task-list.md
```

## Resources
If you want to check more about specs based ai coding you can check these resources:
- Highly recommended: https://www.indragie.com/blog/i-shipped-a-macos-app-built-entirely-by-claude-code
- https://devin.ai/agents101#introduction