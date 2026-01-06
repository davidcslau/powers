---
name: "aidlc"
displayName: "AI-DLC (AI-Driven Development Life Cycle)"
description: "Intelligent software development workflow that adapts to your needs with three phases: Inception (requirements & design), Construction (implementation & testing), and Operations (deployment). Maintains quality standards while keeping you in control."
keywords: ["aidlc", "ai-dlc", "software development", "workflow", "sdlc", "requirements", "design", "implementation", "testing", "adaptive workflow"]
author: "AWS"
---

# AI-DLC (AI-Driven Development Life Cycle)

## Overview

AI-DLC is an intelligent software development workflow that adapts to your needs, maintains quality standards, and keeps you in control of the process. It provides a structured approach to software development with three adaptive phases that intelligently determine which stages are needed based on your project's complexity and requirements.

**CRITICAL FIRST STEP**: Before starting any workflow, you MUST select your preferred language (English or 中文). This is a mandatory, non-negotiable step that determines the language for all subsequent interactions, documentation, and outputs.

**Key Principles:**
- **Language Selection FIRST**: Mandatory language selection before any workflow steps
- **Adaptive Intelligence**: Only executes stages that add value to your specific request
- **Context-Aware**: Analyzes existing codebase and complexity requirements
- **Risk-Based**: Complex changes get comprehensive treatment, simple changes stay efficient
- **Question-Driven**: Structured multiple-choice questions in files, not chat
- **Always in Control**: Review execution plans and approve each phase
- **Complete Audit Trail**: All decisions and changes are tracked
- **Language Consistency**: All outputs in your selected language

## Available Steering Files

This power includes one main steering file that contains the complete workflow:

- **core-workflow** - Complete AI-DLC workflow with all three phases (Inception, Construction, Operations)

To access the workflow, use:
```
Call action "readSteering" with powerName="aidlc", steeringFile="core-workflow.md"
```

## Three-Phase Adaptive Workflow

AI-DLC follows a structured three-phase approach that adapts to your project's complexity:

### 🔵 INCEPTION PHASE
**Purpose**: Determines **WHAT** to build and **WHY**

**Stages:**
- **Workspace Detection** (ALWAYS) - Analyze project state and determine greenfield vs brownfield
- **Reverse Engineering** (CONDITIONAL) - Analyze existing codebase for brownfield projects
- **Requirements Analysis** (ALWAYS) - Gather and validate requirements with adaptive depth
- **User Stories** (CONDITIONAL) - Create user stories when they add value
- **Workflow Planning** (ALWAYS) - Determine execution plan for remaining phases
- **Application Design** (CONDITIONAL) - Design components and services when needed
- **Units Generation** (CONDITIONAL) - Break down complex systems into manageable units

### 🟢 CONSTRUCTION PHASE
**Purpose**: Determines **HOW** to build it

**Per-Unit Loop** (executes for each unit of work):
- **Functional Design** (CONDITIONAL) - Design data models and business logic
- **NFR Requirements** (CONDITIONAL) - Assess non-functional requirements
- **NFR Design** (CONDITIONAL) - Design NFR implementation patterns
- **Infrastructure Design** (CONDITIONAL) - Design cloud resources and deployment
- **Code Generation** (ALWAYS) - Generate code, tests, and artifacts

**Final Stage:**
- **Build and Test** (ALWAYS) - Comprehensive build and test instructions

### 🟡 OPERATIONS PHASE
**Purpose**: How to DEPLOY and RUN it (future expansion)

**Stages:**
- **Operations** (PLACEHOLDER) - Deployment, monitoring, and maintenance workflows

## MANDATORY: Language Selection (CRITICAL - NO NEGOTIATION)

**⚠️ CRITICAL REQUIREMENT - MUST BE EXECUTED FIRST ⚠️**

**BEFORE ANY OTHER WORKFLOW STEPS**, you **MUST** ask the user to select their preferred language. This step is **MANDATORY** and **CANNOT BE SKIPPED** under any circumstances.

### Language Selection Rules

**CRITICAL ENFORCEMENT:**
- ✋ **STOP**: Do NOT proceed with ANY workflow steps until language is selected
- 🚫 **NO NEGOTIATION**: This step MUST be completed first - no exceptions
- ⚠️ **MANDATORY**: Language selection is REQUIRED before displaying welcome message
- 🔒 **NON-SKIPPABLE**: Cannot be bypassed, deferred, or skipped

### Language Selection Process

**Step 1: Display Language Selection Prompt**

Present the following options to the user immediately:

```
🌐 LANGUAGE SELECTION (REQUIRED)

Please select your preferred language for this AI-DLC workflow:

A) English - All documentation, questions, and outputs will be in English
B) 中文 - 所有文档、问题和输出将使用中文

[Answer]: Please respond with A or B
```

**Step 2: Wait for User Response**

- **MUST** wait for explicit user selection (A or B)
- **DO NOT** proceed until valid response received
- If response is unclear, ask again

**Step 3: Record Language Selection**

Once language is selected:
1. **MUST** record the selection in `aidlc-docs/aidlc-state.md` immediately
2. **MUST** log the selection in `aidlc-docs/audit.md` with timestamp
3. **MUST** use the selected language for ALL subsequent interactions

### Language Usage Rules

**After language selection:**

- ✅ **If English selected**: All outputs, questions, documentation, and communication in English
- ✅ **If 中文 selected**: 所有输出、问题、文档和交流使用中文
- 🔄 **Consistency**: MUST maintain selected language throughout entire workflow
- 📝 **Documentation**: All generated files in `aidlc-docs/` MUST use selected language
- 💬 **Questions**: All structured questions MUST be in selected language
- 📊 **Plans**: All execution plans and approval messages MUST be in selected language

**CRITICAL**: Once language is selected, it CANNOT be changed mid-workflow. User must restart workflow to change language.

---

## How to Use AI-DLC

### Getting Started

1. **Activate the workflow** by starting your request with:
   ```
   Using AI-DLC, [describe your software development need]
   ```

2. **MANDATORY FIRST STEP**: Select your preferred language (English or 中文)
   - This step MUST be completed before any other workflow steps
   - Cannot be skipped or bypassed

3. **AI-DLC automatically activates** and displays a welcome message (in selected language)

4. **Follow the guided workflow**:
   - Answer structured questions when asked
   - Review execution plans before each phase
   - Approve or request changes at each stage
   - All artifacts are generated in `aidlc-docs/` directory

### Example Usage

**Step 1: Activate AI-DLC**
```
Using AI-DLC, create a REST API for managing user accounts with authentication
```

**Step 2: Select Language (MANDATORY)**
```
AI-DLC will prompt:
🌐 LANGUAGE SELECTION (REQUIRED)
Please select your preferred language:
A) English
B) 中文

You respond: A (for English) or B (for 中文)
```

**Step 3: Follow Workflow**
After language selection, AI-DLC proceeds with the workflow in your selected language.

**Example Scenarios:**

**Greenfield Project (English):**
```
Using AI-DLC, create a REST API for managing user accounts with authentication
[Select: A - English]
```

**Greenfield Project (中文):**
```
Using AI-DLC, 创建一个用户账户管理的 REST API，包含身份验证功能
[选择: B - 中文]
```

**Brownfield Project (English):**
```
Using AI-DLC, add payment processing functionality to the existing e-commerce application
[Select: A - English]
```

**Brownfield Project (中文):**
```
Using AI-DLC, 为现有的电商应用添加支付处理功能
[选择: B - 中文]
```

**Simple Change (English):**
```
Using AI-DLC, fix the login validation bug in the authentication service
[Select: A - English]
```

**Simple Change (中文):**
```
Using AI-DLC, 修复身份验证服务中的登录验证错误
[选择: B - 中文]
```

## Workflow Adaptation

AI-DLC intelligently adapts based on:

1. **User's stated intent and clarity** - Clear requests may skip detailed requirements
2. **Existing codebase state** - Brownfield projects get reverse engineering
3. **Complexity and scope** - Complex changes get comprehensive treatment
4. **Risk and impact assessment** - High-risk changes get extra validation

**Depth Levels:**
- **Minimal**: Simple, clear requests with low risk
- **Standard**: Normal complexity with moderate risk
- **Comprehensive**: Complex, high-risk changes requiring detailed analysis

## Directory Structure

AI-DLC creates a structured documentation hierarchy:

```
<WORKSPACE-ROOT>/                   # Application code lives here
├── [project-specific structure]    # Your actual code
│
├── aidlc-docs/                     # All AI-DLC documentation
│   ├── inception/                  # 🔵 INCEPTION PHASE
│   │   ├── plans/
│   │   ├── reverse-engineering/    # Brownfield only
│   │   ├── requirements/
│   │   ├── user-stories/
│   │   └── application-design/
│   ├── construction/               # 🟢 CONSTRUCTION PHASE
│   │   ├── plans/
│   │   ├── {unit-name}/
│   │   │   ├── functional-design/
│   │   │   ├── nfr-requirements/
│   │   │   ├── nfr-design/
│   │   │   ├── infrastructure-design/
│   │   │   └── code/               # Markdown summaries only
│   │   └── build-and-test/
│   ├── operations/                 # 🟡 OPERATIONS PHASE
│   ├── aidlc-state.md             # Workflow state tracking
│   └── audit.md                    # Complete audit trail
```

**Critical Rule**: Application code goes in workspace root, documentation goes in `aidlc-docs/`

## Rule Details Files

This power includes comprehensive rule detail files organized by phase:

### Common Rules (Always Loaded)
- `rule-details/common/process-overview.md` - Workflow overview
- `rule-details/common/session-continuity.md` - Session resumption
- `rule-details/common/content-validation.md` - Content validation requirements
- `rule-details/common/question-format-guide.md` - Question formatting rules
- `rule-details/common/terminology.md` - Standard terminology
- `rule-details/common/welcome-message.md` - Initial welcome message
- `rule-details/common/ascii-diagram-standards.md` - Diagram standards
- `rule-details/common/depth-levels.md` - Depth level definitions
- `rule-details/common/error-handling.md` - Error handling guidelines
- `rule-details/common/overconfidence-prevention.md` - Quality safeguards
- `rule-details/common/workflow-changes.md` - Workflow modification rules

### Inception Phase Rules
- `rule-details/inception/workspace-detection.md`
- `rule-details/inception/reverse-engineering.md`
- `rule-details/inception/requirements-analysis.md`
- `rule-details/inception/user-stories.md`
- `rule-details/inception/workflow-planning.md`
- `rule-details/inception/application-design.md`
- `rule-details/inception/units-generation.md`

### Construction Phase Rules
- `rule-details/construction/functional-design.md`
- `rule-details/construction/nfr-requirements.md`
- `rule-details/construction/nfr-design.md`
- `rule-details/construction/infrastructure-design.md`
- `rule-details/construction/code-generation.md`
- `rule-details/construction/build-and-test.md`

### Operations Phase Rules
- `rule-details/operations/operations.md`

## Best Practices

### For Users

1. **Select Language First**: MUST select language (English or 中文) before proceeding - this is mandatory
2. **Be Clear About Intent**: Start with "Using AI-DLC" to activate the workflow
3. **Review Plans Carefully**: Always review execution plans before approval
4. **Provide Feedback**: Request changes when plans don't match your needs
5. **Track Progress**: Monitor `aidlc-state.md` for workflow progress
6. **Review Audit Trail**: Check `audit.md` for complete decision history
7. **Language Consistency**: All workflow outputs will be in your selected language

### For AI Agents

1. **CRITICAL - Language Selection FIRST**: MUST ask user to select language (English or 中文) BEFORE any other steps - NO EXCEPTIONS
2. **Enforce Language Selection**: DO NOT proceed with welcome message or any workflow steps until language is selected
3. **Use Selected Language**: ALL outputs, questions, documentation MUST be in the selected language
4. **Load Common Rules First**: Always load common rules at workflow start (after language selection)
5. **Validate Content**: Validate all content before file creation
6. **Follow Question Format**: Use structured multiple-choice questions
7. **Update Checkboxes**: Mark plan steps complete immediately after execution
8. **Log Everything**: Record all user inputs and AI responses in audit.md
9. **Never Overwrite audit.md**: Always append, never overwrite the audit log
10. **Wait for Approval**: Never proceed without explicit user approval

## Troubleshooting

### Language Selection Not Prompted

**Problem**: Workflow started without asking for language selection

**Solution**:
1. **STOP the workflow immediately**
2. Remind the AI agent: "Language selection is MANDATORY and must be completed first"
3. Request language selection prompt
4. Restart workflow if necessary

### Wrong Language Being Used

**Problem**: Outputs are in wrong language or mixed languages

**Solution**:
1. Check `aidlc-state.md` for recorded language selection
2. Remind AI agent of selected language
3. If language was never selected, stop and complete language selection first
4. If wrong language was selected, restart workflow to change language

### Workflow Not Starting

**Problem**: AI-DLC doesn't activate when starting a request

**Solution**:
1. Ensure you start with "Using AI-DLC, ..." in your message
2. Verify the power is properly installed
3. Check that steering files are accessible

### Missing Documentation

**Problem**: Expected documentation files not created

**Solution**:
1. Check `aidlc-state.md` to see which stages were executed
2. Review `audit.md` for any errors or skipped stages
3. Verify the stage was included in the execution plan

### Workflow Stuck at Approval

**Problem**: Workflow waiting for approval but unclear what to do

**Solution**:
1. Look for the approval message with options
2. Respond with your choice (e.g., "Continue to Next Stage" or "Request Changes")
3. If unclear, ask "What are my options?" to see available choices

### Audit Log Issues

**Problem**: Audit log has duplicate entries or missing information

**Solution**:
1. Ensure AI agent is appending to audit.md, not overwriting
2. Check that all user inputs are being logged with timestamps
3. Verify ISO 8601 timestamp format is being used

## Configuration

**No additional configuration required** - AI-DLC works immediately after power installation.

The workflow automatically:
- **Prompts for language selection** (MANDATORY first step)
- Detects your project structure
- Determines greenfield vs brownfield
- Adapts depth levels based on complexity
- Creates necessary documentation directories
- Generates all outputs in your selected language

**Language Configuration:**
- Language selection is prompted at workflow start
- Selection is recorded in `aidlc-docs/aidlc-state.md`
- Cannot be changed mid-workflow (must restart to change)
- All documentation, questions, and outputs use selected language

## Additional Resources

- **Blog**: [AI-Driven Development Life Cycle](https://aws.amazon.com/blogs/devops/ai-driven-development-life-cycle/)
- **Method Definition Paper**: [AI-DLC Methodology](https://prod.d13rzhkk8cj2z0.amplifyapp.com/)
- **GitHub Repository**: [aidlc-workflows](https://github.com/aws-samples/aidlc-workflows)

---

**Power Type**: Knowledge Base Power (No MCP server required)
**Installation**: Works immediately after installation
**Usage**: 
1. Start any request with "Using AI-DLC, ..."
2. **MANDATORY**: Select language (English or 中文) when prompted
3. Follow the guided workflow in your selected language
