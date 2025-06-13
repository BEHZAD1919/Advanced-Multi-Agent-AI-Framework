# Building a Structured, Transparent, and Well-Documented AI Team

This repository provides a framework for building and managing a hybrid AI team within the Roo Code environment. It combines industry best practices with advanced prompt engineering techniques to create a comprehensive and effective team structure.

## 🙏 Support This Work

If this project helps you build better AI systems and you'd like to show your appreciation:

- **Buy Me a Coffee**: https://buymeacoffee.com/mnehmos
- **Check out Vario Research**: For advanced Deep Research alternatives, visit https://mnehmos.github.io/VarioResearch/ for custom reports in any format.

## 🌟 Key Features

- **Multi-Agent Framework**: Specialized modes for different types of tasks enhanced with 80+ prompt engineering techniques
- **SPARC Framework**: A structured approach to complex problem-solving with semantic precision
- **Agentic Boomerang**: A reliable system for task delegation and tracking
- **Structured Documentation**: Consistent and traceable documentation across all modes
- **Token Optimization**: Efficient resource usage through the "Scalpel, not Hammer" approach
- **Task Maps**: JSON blueprints that break down projects into phases and tasks with dependencies and validation
- **Advanced Prompt Engineering**: Integration of cutting-edge techniques for superior performance

## 🚀 Getting Started

### Prerequisites
- A compatible AI assistant that supports custom modes (Roo Code recommended)
- A basic understanding of the SPARC framework concepts

### Documentation:
- [Custom Instructions](templates/custom-instructions-for-all-modes.md)
- [Custom Modes](templates/custom_modes.yaml)
- [Enhance Prompt](templates/enhance-prompt-template.md)

### Installation

**Watch the video** *(link when available)*

1. **Clone this repository:**
   ```bash
   git clone https://github.com/Mnehmos/The-Ultimate-Roo-Code-Hack-Building-a-Structured-Transparent-and-Well-Documented-AI-Team.git
   ```

2. **Copy the template files:**
   ```bash
   cp templates/custom_modes.yaml ./
   cp templates/custom-instructions-for-all-modes.md ./
   cp templates/enhance-prompt-template.md ./
   ```

3. **Configure your AI assistant:**
   - Click the "Modes" button in the Roo sidebar
   - Select "Edit Project Modes (custom_modes.yaml)"
   - Verify the content matches your project needs
   - Click "Save"
   
   Learn more: [Custom Instructions](templates/custom-instructions-for-all-modes.md)

4. **Set up the custom instructions:**
   - Click the "Modes" button
   - Scroll to "Custom Instructions for All Modes"
   - Copy the contents of `custom-instructions-for-all-modes.md`
   - Paste into the Custom Instructions field
   - Click "Save"
   
   Learn more: [Custom Modes](templates/custom_modes.yaml)

5. **Configure the Enhance Prompt feature:**
   - Click the "Support Prompts" button
   - Select "Enhance Prompt"
   - Copy the contents of `enhance-prompt-template.md`
   - Paste into the Prompt field
   - Click "Save"
   
   Learn more: [Enhance Prompt Documentation](templates/enhance-prompt-template.md)

## 🧩 Basic Usage

1. **Start with Orchestrator Mode**: This is your project manager who will coordinate everything
2. **Describe your project**: Be as detailed as possible in your initial prompt
3. **Generate Task Map**: Use the Enhance Prompt feature to create a JSON Task Map
4. **Let Orchestrator execute**: It will delegate tasks to specialist modes based on the Task Map
5. **Review results**: Orchestrator integrates all pieces and presents the final output

## 🧩 Using the Modes

### Switching Modes
- Click on the current mode name in the bottom left corner of the Roo interface
- Select the desired mode from the dropdown menu

### Using the Enhance Prompt Feature (Task Map Generator)
1. Type your basic project description in the chat
2. Click the ✨ button next to the send button
3. Roo will transform your input into a comprehensive JSON Task Map
4. Review and edit the Task Map if needed
5. Orchestrator will use the Task Map to coordinate the project

### Task Map Example
```json
{
  "project": "A Clear and Concise Project Name",
  "Phase_1_A_Descriptive_Phase_Name": {
    "1.1_a_unique_and_descriptive_task_id": {
      "agent": "The Most Appropriate Specialist Mode",
      "dependencies": ["a_list_of_task_ids_this_task_depends_on"],
      "outputs": ["A list of expected artifacts, such as files or documents"],
      "validation": "A clear, measurable success criterion for this task",
      "human_checkpoint": "A boolean indicating if human review is required before proceeding",
      "scope": "A detailed description of what is in and out of scope for this task"
    }
  },
  "Phase_2_Another_Descriptive_Phase_Name": {
    "2.1_another_unique_task_id": {
      "...": "..."
    }
  }
}
```

### Creating Custom Tasks
When creating tasks for specialist modes, use the standardized task prompt format:

```markdown
# [TASK_ID]: [TASK_TITLE]

## 1. Objective
*A clear, concise statement of the task's goal.*

## 2. Context & Background
*Relevant information, including links to related issues, PRs, or other documentation. Explain the "why" behind the task.*

## 3. Scope
- **In Scope:**
  - *A bulleted list of specific, actionable requirements.*
- **Out of Scope:**
  - *A bulleted list of what is explicitly not to be done.*

## 4. Acceptance Criteria
*A set of measurable criteria that must be met for the task to be considered complete. Each criterion should be a testable statement.*
- [ ] *Criterion 1: ...*
- [ ] *Criterion 2: ...*
- [ ] *Criterion 3: ...*

## 5. Deliverables
*A list of the expected outputs from this task.*
- **Artifacts:** *(e.g., a new file, a modified class, a markdown document)*
- **Documentation:** *(e.g., updated README, new API documentation)*
- **Tests:** *(e.g., unit tests, integration tests)*

## 6. [Optional] Implementation Plan
*A suggested, high-level plan for completing the task. This is not a rigid set of instructions, but a guide to get started.*

## 7. [Optional] Additional Resources
*Links to relevant documentation, examples, or other materials that may be helpful.*
```

This structured format ensures that specialist modes have all the information they need to complete tasks effectively and consistently.

## 🔄 The Boomerang Pattern

The Boomerang Pattern is a core concept in Roo Code that enables the Orchestrator to break down complex projects into smaller, manageable tasks and delegate them to specialized modes. This pattern is the engine that powers our Task Map and New Task frameworks.

The process works as follows:

1. **Task Creation**: The Orchestrator creates a new task, either from a Task Map or a "New Task" prompt
2. **Delegation**: The task is delegated to the most appropriate specialist mode
3. **Execution**: The specialist mode executes the task, focusing on its specific area of expertise
4. **Return**: Once the task is complete, the specialist mode "boomerangs" the result back to the Orchestrator
5. **Integration**: The Orchestrator integrates the result into the overall project, updates the Task Map, and delegates the next task

This recursive loop of delegation, execution, and integration allows for a highly efficient and organized workflow, ensuring that complex projects are completed in a structured and transparent manner. Each agent is responsible for recording their actions as appropriate in the `.roo/logs` directory, ensuring a complete and traceable record of the project's history.

## 👥 Meet the Team

Our AI team consists of specialized modes, each enhanced with advanced prompt engineering techniques:

### Core Coordination
- **🪃 [Orchestrator](meet-the-team/orchestrator.md)**: Project coordination and task delegation with workflow-template-prompting
- **🏛️ [Architect](meet-the-team/architect.md)**: System design and architecture with visual-documentation-generation
- **🗓️ [Planner](meet-the-team/planner.md)**: Product planning and requirements with user-story-prompting

### Implementation Team
- **🧱 [Builder](meet-the-team/builder.md)**: Software development and testing with code-generation-agents
- **💻 [Code](meet-the-team/code.md)**: Advanced coding and optimization with modular-code-generation
- **🛡️ [Guardian](meet-the-team/guardian.md)**: Infrastructure and CI/CD with automated-development-workflows

### Research & Analysis
- **❓ [Ask](meet-the-team/ask.md)**: Information discovery with RAG and iterative-retrieval-augmentation
- **🔍 [Deep Research](meet-the-team/deep-research-agent.md)**: Comprehensive analysis with multi-perspective-analysis
- **🔎 [Deep Scope](meet-the-team/deep-scope.md)**: Issue scoping with codebase-impact-mapping

### Support Specialists  
- **🪲 [Debug](meet-the-team/debug.md)**: Technical diagnostics with five-whys-prompting
- **💾 [Memory](meet-the-team/memory.md)**: Knowledge management with semantic-clustering

Each mode integrates advanced prompt engineering techniques for superior performance while maintaining unified methodology and quality standards.

## 📊 Performance Optimization

- Keep context window utilization below 40%
- Start with the least token-intensive cognitive primitives
- Break complex tasks into atomic components
- Use the most specialized mode for each subtask
- Apply "Scalpel, not Hammer" philosophy throughout

## 📚 Documentation

For detailed documentation on Roo Code features:
- [Custom Instructions](templates/custom-instructions-for-all-modes.md)
- [Custom Modes](templates/custom_modes.yaml)
- [Enhance Prompt](templates/enhance-prompt-template.md)

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments

- The SPARC framework developers
- Contributors to the multi-agent AI research community (Roo Code, huge shoutout)
- Advanced prompt engineering research community
- All users who provide feedback and suggestions

---

*This framework represents a mature, research-backed approach to AI team building, integrating 80+ prompt engineering techniques with proven multi-agent coordination patterns for superior development outcomes.*
