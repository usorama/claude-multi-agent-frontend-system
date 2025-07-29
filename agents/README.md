# Claude Code Specialized Agents

This directory contains specialized AI agents for Claude Code that enhance development capabilities for the Virtual Tutor project.

## Available Agents

### 🎨 UI Designer Agent (`ui-designer.md`)
**Color**: Purple (#9333EA)

Specialized in creating beautiful, accessible UI components using:
- shadcn/ui v4 components (via `--shadcn` MCP server)
- Tailwind CSS v4 with CSS variables
- React 19 component patterns
- Educational UI best practices
- WCAG AA accessibility standards

### 🔨 Frontend Builder Agent (`frontend-builder.md`)
**Color**: Green (#10B981)

Expert in building and optimizing frontend applications:
- Build system configuration (Vite, Next.js, Webpack)
- Testing frameworks (Jest, Playwright, Cypress)
- Performance optimization
- CI/CD pipeline setup
- Deployment strategies

## Installation

These agents are automatically detected by Claude Code when placed in the `.claude/agents/` directory. No additional configuration is required.

## Usage

Claude Code will automatically delegate tasks to the appropriate agent based on the task context. You can also explicitly request an agent by mentioning their specialty:

```bash
# UI Design tasks
"Create a responsive dashboard component using shadcn"
"Design an accessible form with proper ARIA labels"

# Frontend Build tasks
"Optimize the bundle size for production"
"Set up E2E testing with Playwright"
```

## Agent Collaboration

The agents are designed to work together:
1. UI Designer creates optimized components
2. Frontend Builder ensures they're production-ready
3. Both agents follow the project's design system (@design.md)

## shadcn MCP Server

The UI Designer agent requires the shadcn MCP server. Key commands:

```bash
# List components
--shadcn list_components

# Get component code
--shadcn get_component [component-name]

# Get usage examples
--shadcn get_demo [component-name]
```

## Best Practices

1. **Context Efficiency**: Agents spawn with their own context, preserving the main agent's context
2. **Parallel Execution**: Use multiple agents in parallel for complex tasks
3. **Verification**: Agents can verify each other's work for quality assurance
4. **Documentation**: Each agent maintains its own quality standards and checklists

## Resources

- [Claude Code Documentation](https://docs.anthropic.com/claude-code)
- [shadcn/ui Documentation](https://ui.shadcn.com)
- [MCP Servers Directory](https://mcpservers.org)

---

*Created: July 26, 2025 - Based on the latest Claude Code agent architecture*