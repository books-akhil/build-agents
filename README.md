# Building Agents

## Components of Agents

- models
- tools
- knowledge
- memory
- audio and speech
- guardrails
- orchestraction

## Agent workflows

- Prompt chaining or Sequential: output of one llm passes as input of another.
- Routing : Based on the task, a router llm routes to different llms.
- Parallelization : Work simultaneouslyt on a task and their aoutputs aggregated programmatically.
    - Sections : Breaking a task into independent subtasks
    - Voting : Running the same task multiple times to get diverse outputs.
- Orchestractor worker : Similar to paralelization, except the orchestractor create subtasks.
- Evaluator optimizer : One llm call generates a response while another provides evaluation and feedback in a loop.
- Autonomous : LLM gets feedback from the environment and it knows where to stop.

## Prompt Engineering for Agents

- Role : Can specify the style or tone also here. Normaly the first line.
- Task :
- Input :
- Output :
- Contstraints :
- Capability and Reminder :  Info about the tools it have
