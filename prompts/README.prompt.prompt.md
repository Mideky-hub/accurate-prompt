# 🤖 Agent Directory Guide

This directory contains specialized AI agents for the MAWD project. Each agent is an expert in their domain and can be invoked through VSCode's agent system.

## 📁 Agent Categories

### 🔧 Engineering
- **`rust-performance-optimizer`** - Optimizes Rust code for maximum performance while maintaining correctness
- **`backend-architect`** - Designs scalable backend systems and APIs
- **`test-writer-fixer`** - Creates and fixes tests, ensures code quality
- **`devops-automator`** - Handles CI/CD, deployment, and infrastructure
- **`ai-engineer`** - AI/ML integration and optimization
- **`rapid-prototyper`** - Quick proof-of-concept development

### 🧪 Testing
- **`api-tester`** - API testing and validation
- **`performance-benchmarker`** - Performance testing and analysis
- **`test-results-analyzer`** - Test result interpretation and improvement suggestions

### 🎨 Design
- **`ui-designer`** - User interface design and implementation
- **`ux-researcher`** - User experience research and optimization

### 📊 Project Management
- **`project-shipper`** - Release management and deployment coordination
- **`experiment-tracker`** - A/B testing and feature flag management

## 🚀 Quick Start Guide

### Invoke Agents in VSCode
1. **Command Palette**: `Ctrl+Shift+P` → "Chat: Select Agent"
2. **Chat Panel**: Type `@agent-name` followed by your question
3. **Context Menu**: Right-click code → "Ask Agent"

### Common Workflows

#### Performance Optimization
```
1. @rust-performance-optimizer - Analyze performance bottlenecks
2. @performance-benchmarker - Create benchmarks
3. @test-results-analyzer - Validate improvements
```

#### Bug Investigation
```
1. @test-writer-fixer - Create failing test cases
2. @backend-architect - Analyze system design issues
3. @devops-automator - Check deployment/config issues
```

#### Feature Development
```
1. @rapid-prototyper - Quick proof of concept
2. @backend-architect - Production-ready implementation
3. @api-tester - Validate API contracts
4. @project-shipper - Deploy and monitor
```

## 📋 Agent Selection Matrix

| Task Type | Primary Agent | Secondary Agent | Tertiary Agent |
|-----------|---------------|-----------------|----------------|
| Performance Issues | `rust-performance-optimizer` | `performance-benchmarker` | `test-results-analyzer` |
| Bug Fixes | `test-writer-fixer` | `backend-architect` | `devops-automator` |
| New Features | `backend-architect` | `rapid-prototyper` | `api-tester` |
| Code Reviews | `backend-architect` | `test-writer-fixer` | `rust-performance-optimizer` |
| Deployment | `devops-automator` | `project-shipper` | `infrastructure-maintainer` |
| Testing | `test-writer-fixer` | `api-tester` | `performance-benchmarker` |

## 🎯 Project-Specific Usage

### For MAWD Rust Services
- **calculate_interval**: Use `@rust-performance-optimizer` for math optimizations
- **calculate_point_ko**: Use `@test-writer-fixer` for comprehensive testing
- **flat_sequence**: Use `@backend-architect` for algorithm design

### For Lambda Functions
- **Performance**: `@rust-performance-optimizer` + `@devops-automator`
- **Testing**: `@api-tester` + `@test-writer-fixer`
- **Deployment**: `@devops-automator` + `@project-shipper`

## 💡 Pro Tips

### Context Sharing
When switching between agents, provide context:
```
@rust-performance-optimizer I found a bottleneck in calculate_interval service.
The profiler shows 80% time spent in nested loops. Here's the function:
[paste code]
```

### Chain Agent Conversations
```
1. @rust-performance-optimizer - "Optimize this function"
2. @test-writer-fixer - "Create benchmarks for the optimized version"  
3. @performance-benchmarker - "Compare before/after performance"
```

### Use File Context
Agents work better with file context:
```
# In services/calculate_interval/src/main.rs
@rust-performance-optimizer How can I optimize this handler function?
```

## 🔄 Workflow Examples

### Performance Investigation
```bash
# 1. Profile the code
@rust-performance-optimizer "Profile calculate_point_ko service"

# 2. Create benchmarks  
@performance-benchmarker "Create benchmarks for bottleneck functions"

# 3. Implement optimizations
@rust-performance-optimizer "Apply SIMD optimizations to math functions"

# 4. Validate results
@test-results-analyzer "Compare benchmark results before/after"
```

### Bug Resolution
```bash
# 1. Reproduce the issue
@test-writer-fixer "Create test case for failing calculation"

# 2. Analyze root cause
@backend-architect "Analyze why calculation returns wrong result"

# 3. Fix and validate
@test-writer-fixer "Fix the bug and ensure all tests pass"
```

Remember: Each agent has deep expertise in their domain and can provide specialized guidance tailored to your specific needs!
