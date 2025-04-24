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

## Build Coding Agents

### Thinking

- Logical
- Analytical
- Computational
- Procedural

### Frameworks

### Checkpoints / Versions

### Debugging

### Context

---

## ReAct Loop

- Thought --> Action --> Observation
- Agent actions should be in a json format. {tool_name: ... , args: ...} --> Tool calling. Tool calling creates more steps and more tokens.
- Code Agents use a code format for taking actions like
  ```py
  answer = fn_name(**kwargs)
  print(answer)
  ```

### Security threats using code agents (Smol agents)

- LLM error
- Supply chain attack
- Prompt injections

These attacks can harm your system. Safe gaurds

- Any undefined command is ignored
- Import securitization
- prevent infinite loops

- Run code snippets in a sandbox

## Monitoring Agents

