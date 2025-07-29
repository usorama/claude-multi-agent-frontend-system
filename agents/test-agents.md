# Agent Testing Commands

Use these commands to test the specialized agents:

## Test UI Designer Agent

```bash
# Test 1: Create a dashboard component
/agent:ui-designer Create a responsive student dashboard with progress cards using shadcn components

# Test 2: Design an accessible form
/agent:ui-designer Design a login form with proper accessibility features using shadcn Form components

# Test 3: Component with animations
/agent:ui-designer Create an achievement badge component with micro-interactions using Framer Motion
```

## Test Frontend Builder Agent

```bash
# Test 1: Optimize build
/agent:frontend-builder Analyze and optimize the current Next.js build configuration

# Test 2: Set up testing
/agent:frontend-builder Configure Jest and React Testing Library for the project

# Test 3: Performance audit
/agent:frontend-builder Run a Lighthouse audit and improve Core Web Vitals
```

## Test Agent Collaboration

```bash
# Combined task requiring both agents
Create a new feature: Student Progress Dashboard
1. UI Designer: Design responsive progress cards with charts
2. Frontend Builder: Optimize bundle size and set up tests
```

## Verify Agent Colors

The agents should appear with their designated colors in Claude Code output:
- UI Designer: Purple (#9333EA)
- Frontend Builder: Green (#10B981)

## Common Issues

1. **Agent not found**: Ensure files are in `.claude/agents/` directory
2. **MCP server error**: Verify shadcn MCP server is installed and configured
3. **Context overflow**: Use parallel agents for large tasks

---

*Run these tests after setting up the agents to ensure they're working correctly.*