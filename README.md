# Building a Structured Transparent and Well Documented AI Team (In Roo Code)

**Building a Structured, Transparent, and Well-Documented AI Team that Delegates Its Own Tasks**

## 🙏 Support This Work

If this project helps you build better AI systems and you'd like to show your appreciation:

- **Buy Me a Coffee**: [https://buymeacoffee.com/mnehmos](https://buymeacoffee.com/mnehmos)
- **Check out Vario Research**: For advanced Deep Research alternatives (Talking about you Gemini, ChatGPT), visit [https://mnehmos.github.io/VarioResearch/](https://mnehmos.github.io/VarioResearch/) for custom reports in any format (I Prefer customized websites so i can add in API functionalities into your dashboards as needed. (Alpha Vantage, Yahoo Finance, Arxiv, google maps, etc))

## 🌟 Key Features

- **Multi-Agent Framework**: Specialized modes for different types of tasks
- **SPARC Framework**: Structured approach to complex problem-solving
- **Agentic Boomerang**: Reliable task delegation and tracking system
- **Structured Documentation**: Consistent, traceable documentation
- **Token Optimization**: Efficient resource usage through the "Scalpel, not Hammer" approach
- **Task Maps**: JSON blueprints that break down projects into phases/tasks with dependencies and validation

## 🧩 Specialized Modes

The system includes the following specialized modes:

- **🪃 Orchestrator**: Task decomposition, assignment, and verification using JSON Task Maps
- **💻 Code**: Software implementation and optimization
- **🏛️ Architect**: System design and pattern application
- **❓ Ask**: Information retrieval, evaluation, and communication
- **🪲 Debug**: Problem diagnosis and极 validation
- **💾 Memory**: Knowledge storage, organization, and retrieval
- **🔍 Deep Research**: In-depth investigation and analysis

## 🏗️ Architecture

Below is an architectural overview of how the Roo framework operates:

```
┌─────────────────────────────────┐
│            VS Code              │
│     (Primary Development        │
│          Environment)           │
└───────────────┬─────────────────┘
                │
                ▼
┌─────────────────────────────────┐
│             Roo Code            │
│                ↓                │
│          System Prompt          │
│   (Contains SPARC Framework:    │
│    • Specification, Pseudocode, │
│      Architecture, Refinement,  │
│      Completion methodology     │
│    • Advanced reasoning models  │
│    • Best practices enforcement │
│    • Memory Bank integration    │
│    • Boomerang pattern support) │
└───────────────┬─────────────────┘
                │
                ▼
┌─────────────────────────────────┐      ┌─────────────────────────┐
│           Orchestrator          │      │         User            │
│     (System Prompt contains:    │      │     (Customer with      │
│      roles, definitions,        │◄─────┤     minimal context)    │
│      systems, processes,        │      │                         │
│      nomenclature, etc.)        │      └─────────────────────────┘
└───────────────┬─────────────────┘
                │
                ▼
┌─────────────────────────────────┐
│        Query Processing         │
└───────────────┬─────────────────┘
                │
                ▼
┌─────────────────────────────────┐
│     Structured Prompt Creation  │
│                                 │
│       Project Prompt Eng.       │
│       Project Context           │
│       System Prompt             │
│       Role Prompt               │
└───────────────┬─────────────────┘
                │
                ▼
┌─────────────────────────────────┐
│           Orchestrator          │
│     (System Prompt contains:    │
│      roles, definitions,        │
│      systems, processes,        │
│      nomenclature, etc.)        │
└───────────────┬─────────────────┘
                │
                ▼
┌─────────────────────────────────┐
│         Subtask Prompt         │
│   (Generated by Orchestrator    │
│        with structure)          │
│                                 │
│    ┌─────────┐  ┌─────────┐    │
│    │  Topic  │  │ Context │    │
│    └─────────┘  └─────────┘    │
│                                 │
│    ┌─────────┐  ┌─────────┐    │
│    │  Scope  │  │ Output  │    │
│    └─────────┘  └─────────┘    │
│                                 │
│    ┌─────────────────────┐     │
│    │       Extras        │     │
│    └─────────────────────┘     │
└───────────────┬─────────────────┘
                │
                ▼
┌─────────────────────────────────┐   ┌────────────────────────────────────┐
│       Specialized Modes         │   │           MCP Tools                 │
│                                 │   │                                     │
│  ┌────────┐ ┌────────┐ ┌─────┐ │   │ ┌─────────┐  ┌─────────────────┐   │
│  │  Code  │ │ Debug  │ │ ... │ │──►│ │ Basic   │  │ CLI/Shell        │   │
│  └────┬───┘ └────┬───┘ └──┬──┘ │   │ │ CRUD    │  │ (cmd/PowerShell) │   │
│       │          │        │    │   │ └─────────┘  └─────────────────┘   │
└───────┼──────────┼────────┼────┘   │                                     │
        │          │        │        │ ┌─────────┐  ┌─────────────────┐   │
        │          │        │        │ │ API     │  │ Browser          │   │
        │          │        └───────►│ │ Calls   │  │ Automation       │   │
        │          │                 │ │ (Alpha  │  │ (Playwright)     │   │
        │          │                 │ │ Vantage)│  │                  │   │
        │          │                 │ └─────────┘  └─────────────────┘   │
        │          │                 │                                     │
        │          └────────────────►│ ┌──────────────────────────────┐   │
        │                            │ │        LLM Calls              │   │
        │                            │ │                               │   │
        │                            │ │ • Basic Queries               │   │
        └───────────────────────────►│ │ • Reporter Format            │   │
                                     │ │ • Logic MCP Primitives        │   │
                                     │ │ • Sequential Thinking         │   │
                                     │ └──────────────────────────────┘   │
                                     └────────────────┬─────────────────┬─┘
                                                      │                 │
                                                      ▼                 │
┌─────────────────────────────────────────────────────────────────┐    │
│                   Recursive Loop                                │    │
│                                                                 │    │
│  ┌────────────────────────┐    ┌───────────────────────┐       │    │
│  │     Task Execution     │    │      Reporting        │       │    │
│  │                        │    │                       │       │    │
│  │ • Execute assigned task│───►│ • Report work done    │       │◄───┘
│  │ • Solve specific issue │    │ • Share issues found  │       │
│  │ • Maintain focus       │    │ • Provide learnings   │       │
│  └────────────────────────┘    └─────────┬─────────────┘       │
│                                           │                     │
│                                           ▼                     │
│  ┌────────────────────────┐    ┌───────────────────────┐       │
│  │   Task Delegation      │    │    Deliberation       │       │
│  │                        │◄───┤                       │       │
│  │ • Identify next steps  │    │ • Assess progress     │       │
│  │ • Assign to best mode  │    │ • Integrate learnings │       │
│  │ • Set clear objectives │    │ • Plan next phase     │       │
│  └────────────────────────┘    └───────────────────────┘       │
│                                                                 │
└────────────────────────────────┬────────────────────────────────┘
                                 │
                                 ▼
┌─────────────────────────────────────────────────────────────────┐
│                     Memory Mode                                  │
│                                                                 │
│  ┌────────────────────────┐    ┌───────────────────────┐       │
│  │  Project Archival      │    │   SQL Database        │       │
│  │                        │    │                       │       │
│  │ • Create memory folder │───►│ • Store project data  │       │
│  │ • Extract key learnings│    │ • Index for retrieval │       │
│  │ • Organize artifacts   │    │ • Version tracking    │       │
│  └────────────────────────┘    └─────────┬─────────────┘       │
│                                           │                     |
│                                           ▼                     │
│  ┌────────────────────────┐    ┌───────────────────────┐       │
│  │  Memory MCP            │    │   RAG System          │       │
│  │                        │◄───┤                       │       │
│  │ • Database writes      │    │ • Vector embeddings   │       │
│  │ • Data validation      │    │ • Semantic indexing   │       │
│  │ • Structured storage   │    │ • Retrieval functions │       │
│  └─────────────┬──────────┘    └───────────────────────┘       │
│                │                                               │
└────────────────┼───────────────────────────────────────────────┘
                 │
                 └───────────────────────────────────┐
                                                      ▼
┌─────────────────────────────────┐      ┌─────────────────────────┐
│           Orchestrator          │      │         User            │
│     (System Prompt contains:    │      │     (Customer with      │
│      roles, definitions,        │◄─────┤     minimal context)    │
│      systems, processes,        │      │                         │
│      nomenclature, etc.)        │      └─────────────────────────┘
└───────────────┬─────────────────┘
|
              Restart Recursive Loop
```
## 🚀 Getting Started

### Prerequisites

- A compatible AI assistant that supports custom modes
- Basic understanding of the SPARC framework concepts

> **Documentation**:  
> - [Custom Instructions](https://docs.roocode.com/features/custom-instructions)  
> - [Custom Modes](https://docs.roocode.com/features/custom-modes)  
> - [Enhance Prompt](https://docs.roocode.com/features/enhance-prompt)  

### Installation

#### Option 2: Manual Setup

1. Clone this repository:
   ```
   git clone https://github.com/Mnehmos/The-Ultimate-Roo-Code-Hack-Building-a-Structured-Transparent-and-Well-Documented-AI-Team.git
   ```

2. Copy the template files:
   ```bash
   cp templates/custom_modes.yaml ./
   cp templates/custom-instructions-for-all-modes.md ./
   cp templates/enhance-prompt-template.md ./
   ```

3. Configure your AI assistant:
   - Click the "Modes" button in the Roo sidebar
   - Select "Edit Project Modes (custom_modes.yaml)"
   - Verify the content matches your project needs
   - Click "Save"

4. Set up the custom instructions:
   - Click the "Modes" button
   - Scroll to "Custom Instructions for All Modes"
   - Copy the contents of `custom-instructions-for-all-modes.md`
   - Paste into the Custom Instructions field
   - Click "Save"

5. Configure the Enhance Prompt feature:
   - Click the "Support Prompts" button
   - Select "Enhance Prompt"
   - Copy the contents of `enhance-prompt-template.md`
   - Paste into the Prompt field
   - Click "Save"
   > Learn more: [Enhance Prompt Documentation](https://docs.roocode.com/features/enhance-prompt)

6. Create the project structure:
   ```bash
   mkdir .roo
   echo "{}" > .roo/boomerang-state.json
   mkdir -p .roo/logs .roo/memory
   ```

#### Option 1: NPM (Coming Soon)

```

```


### Additional Configuration

#### Configure Enhance Prompt (Optional)
1. Click the "Support Prompts" button in the Roo sidebar
2. Select "Enhance Prompt"
3. Copy the contents of `templates/enhance-prompt-template.md`
4. Paste into the Prompt field
5. Click "Save"
> Learn more: [Enhance Prompt Documentation](https://docs.roocode.com/features/enhance-prompt)

## 🧩 Basic Usage

1. **Start with Orchestrator Mode** - This is your project manager who will coordinate everything
2. **Describe your project** - Be as detailed as possible in your initial prompt
3. **Generate Task Map** - Use the Enhance Prompt feature to create a JSON Task Map
4. **Let Orchestrator execute** - It will delegate tasks to specialist modes based on the Task Map
5. **Review results** - Orchestrator integrates all pieces and presents the final output

## 🧩 Using the Modes

### Switching Modes
1. Click on the current mode name in the bottom left corner of the Roo interface
2. Select the desired mode from the dropdown menu

### Using the Enhance Prompt Feature (Task Map Generator)
1. Type your basic project description in the chat
2. Click the ✨ button next to the send button
3. Roo will transform your input into a comprehensive JSON Task Map
4. Review and edit the Task Map if needed
5. Orchestrator will use the Task Map to coordinate the project

### Task Map Example
```json
{
  "project": "SaaS Dashboard",
  "Phase_1_Foundation": {
    "1.1_setup": {
      "agent": "Orchestrator",
      "outputs": ["package.json", "folder_structure"],
      "validation": "npm run dev works"
    },
    "1.2_database": {
      "agent": "Architect",
      "outputs": ["schema.sql", "migrations/"],
      "human_checkpoint": "Review schema"
    }
  },
  "Phase_2_Backend": {
    "2.1_api": {
      "agent": "Code",
      "dependencies": ["1.2_database"],
      "outputs": ["routes/", "middleware/"]
    },
    "2.2_auth": {
      "agent": "Code",
      "scope": "JWT auth only - NO OAuth",
      "outputs": ["auth endpoints", "tests"]
    }
  }
}
```

### Creating Custom Tasks
When creating tasks for specialist modes, use the standardized task prompt format:

```markdown
# [Task Title]

## Context
[Background information and relationship to the larger project]

## Scope
[Specific requirements and boundaries for the task]

## Expected Output
[Detailed description of deliverables]

## Additional Resources
[Relevant tips, examples, or reference materials]
```

This structured format ensures that specialist modes have all the information they need to complete tasks effectively and consistently.

## 🔄 The Boomerang Pattern

The Boomerang Pattern ensures reliable task delegation and tracking:

1. Add new modes by updating `custom_modes.yaml`
2. Create corresponding rule files in `.roo/rules-{new-mode}/rules.md`
3. Implement mode-specific logging in `.roo/logs/{new-mode}-activity.md`
4. Update memory indexes to accommodate new artifact types

> **Note**: The `.roo` directory structure is used for keeping notes, logs, and documenting activity and changes.

## 📊 Performance Optimization

- Keep context window utilization below 40%
- Start with the least token-intensive cognitive primitives
- Break complex tasks into atomic components
- Use the most specialized mode for each subtask

## 📚 Documentation

For detailed documentation on Roo Code features:
- [Custom Instructions](https://docs.roocode.com/features/custom-instructions)
- [Custom Modes](https://docs.roocode.com/features/custom-modes)
- [Enhance Prompt](https://docs.roocode.com/features/enhance-prompt)

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments

- The SPARC framework developers
- Contributors to the multi-agent AI research community (Roo Code, huge shoutout)
- All users who provide feedback and suggestions
