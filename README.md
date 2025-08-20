# OpenSearch SQL Cline Memory Bank & Development Rules

This repository contains a comprehensive development environment setup for Cline (Claude Engineer) specifically designed for the OpenSearch SQL plugin project. It includes automated Memory Bank management, development standards, and workflow patterns that enable Cline to maintain context across sessions and work effectively on complex software projects.

## What This Provides

### 🧠 Memory Bank System
- **Persistent Context**: Cline automatically reads project context at the start of every session
- **Structured Documentation**: Organized knowledge base covering project goals, architecture, and current status
- **Feature Investigation**: Systematic approach to analyzing and designing new features
- **Progress Tracking**: Clear visibility into what's working, what's left to build, and current status

### 📋 Development Standards
- **Java Coding Standards**: Comprehensive guidelines for Java development
- **OpenSearch Project Patterns**: Specific patterns for OpenSearch plugin development
- **Testing Requirements**: Built-in testing standards and coverage requirements
- **Workflow Integration**: Automated development workflow patterns

### 🔧 Project-Specific Configuration
- **Multi-Module Architecture**: Tailored for OpenSearch SQL's complex module structure
- **ANTLR Integration**: Specialized support for grammar-based parser development
- **Calcite Integration**: Patterns for Apache Calcite query optimization
- **PPL/SQL Support**: Specific guidance for both SQL and PPL language implementation

## Repository Structure

```
.clinerules/
├── README.md                   # This file
├── .gitignore                  # Manages temporary development files
├── 01-memory-bank.md          # Memory Bank system integration
├── 02-java-standards.md       # Java development standards
├── 03-opensearch-project.md   # OpenSearch-specific guidelines
├── 04-testing.md              # Testing requirements
├── 05-workflow.md             # Development workflow patterns
└── memory-bank/               # Memory Bank core files
    ├── projectbrief.md        # Project foundation and scope
    ├── productContext.md      # Product goals and user experience
    ├── activeContext.md       # Current work focus (gitignored)
    ├── systemPatterns.md      # Architecture and design patterns
    ├── techContext.md         # Technical setup and dependencies
    ├── progress.md            # Project status and evolution
    ├── features/              # Feature investigation system
    │   ├── README.md          # Feature documentation guide
    │   ├── feature-template.md # Template for new features
    │   └── [feature files]    # Individual feature investigations (gitignored)
    └── opensearch-specific/   # OpenSearch-specialized documentation
        ├── ppl-parser-patterns.md     # PPL parser implementation
        ├── calcite-integration.md     # Calcite integration patterns
        └── module-architecture.md     # Module organization
```

## How It Works

### Automatic Context Loading
Every time Cline starts a new session, it automatically:
1. **Reads all Memory Bank files** to understand the current project state
2. **Loads relevant feature investigations** when working on specific features
3. **Summarizes key findings** and identifies next steps
4. **Applies development standards** and workflow patterns

### Memory Bank Management
The Memory Bank consists of 6 core files that build upon each other:
- **projectbrief.md**: Foundation document defining scope and requirements
- **productContext.md**: Why the project exists and how it should work
- **activeContext.md**: Current work focus and recent changes (session-specific)
- **systemPatterns.md**: Architecture decisions and design patterns
- **techContext.md**: Technologies, dependencies, and development setup
- **progress.md**: What works, what's left, and project evolution

### Feature Investigation System
- **Systematic Analysis**: Structured approach to investigating new features
- **Design Documentation**: Preserves investigation results and design decisions
- **Knowledge Retention**: Captures technical discoveries and lessons learned
- **Implementation Planning**: Detailed strategies for feature development

## Installation & Usage

### For OpenSearch SQL Development
1. **Clone this repository** into your OpenSearch SQL project:
   ```bash
   cd your-opensearch-sql-project
   git clone https://github.com/ykmr1224/opensearch-sql-cline-memory-bank-rules.git .clinerules
   ```

2. **Cline will automatically detect** the `.clinerules` folder and start using the Memory Bank system

3. **Begin development** - Cline will read all context files at session start

### For Other Projects
This system is specifically tailored for OpenSearch SQL development, but the patterns can be adapted:

1. **Copy the structure** to your project's `.clinerules` folder
2. **Customize the Memory Bank files** for your project's context
3. **Modify the development standards** to match your technology stack
4. **Update the workflow patterns** for your development process

## Key Features

### 🔄 Session Continuity
- Cline maintains perfect context across sessions
- No loss of project knowledge or current work status
- Automatic loading of relevant documentation

### 📊 Progress Tracking
- Clear visibility into project status
- Evolution of architectural decisions
- Success metrics and quality tracking

### 🎯 Feature Development
- Systematic investigation and design process
- Preservation of technical discoveries
- Reusable implementation strategies

### 🧪 Quality Assurance
- Built-in testing requirements
- Code quality standards
- Performance considerations

### 🔧 Development Efficiency
- Automated workflow patterns
- Consistent development standards
- Reduced context switching overhead

## Benefits

### For Individual Developers
- **Faster Onboarding**: Complete project context available immediately
- **Consistent Quality**: Built-in standards and best practices
- **Reduced Cognitive Load**: Automated context management
- **Better Documentation**: Systematic knowledge capture

### For Teams
- **Shared Understanding**: Common development patterns and standards
- **Knowledge Preservation**: Technical decisions and rationale documented
- **Consistent Approach**: Standardized development workflow
- **Easy Collaboration**: Clear project structure and context

### For Complex Projects
- **Multi-Module Support**: Handles complex project architectures
- **Technology Integration**: Specialized support for project-specific technologies
- **Scalable Patterns**: Grows with project complexity
- **Long-term Maintenance**: Preserves institutional knowledge

## Customization

### Adapting for Your Project
1. **Update projectbrief.md** with your project's scope and requirements
2. **Modify productContext.md** to reflect your product goals
3. **Customize systemPatterns.md** for your architecture
4. **Update techContext.md** with your technology stack
5. **Adjust development standards** in the numbered rule files

### Adding New Features
1. **Use the feature template** in `memory-bank/features/feature-template.md`
2. **Document investigation results** and design decisions
3. **Update activeContext.md** to reference new features
4. **Preserve knowledge** for future development cycles

## Contributing

This repository represents a working example of Cline development rules for the OpenSearch SQL project. If you find patterns that could be improved or have suggestions for better development workflows, please:

1. **Open an issue** to discuss the improvement
2. **Submit a pull request** with your enhancements
3. **Share your experience** with adapting these patterns to other projects

## License

This project is licensed under the same terms as the OpenSearch SQL project - Apache License 2.0.

## Acknowledgments

- **OpenSearch Community**: For the excellent SQL plugin architecture
- **Cline Development Team**: For creating such a powerful development assistant
- **Apache Calcite**: For the robust query optimization framework
- **ANTLR**: For the powerful parser generation capabilities

---

**Note**: This system is designed to work automatically with Cline. Simply having the `.clinerules` folder in your project root will activate the Memory Bank system and development standards.
