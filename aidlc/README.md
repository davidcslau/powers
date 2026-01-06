# AI-DLC Kiro Power

This is a Kiro Power for the AI-Driven Development Life Cycle (AI-DLC) methodology.

## Installation

### Method 1: Local Directory (Recommended for Testing)

1. Open Kiro Powers UI (use command palette or click Powers icon)
2. Click "Add Custom Power" button
3. Select "Local Directory"
4. Provide the full absolute path to this directory:
   ```
   /path/to/your/workspace/powers/aidlc
   ```
5. Click "Add" to install

### Method 2: Copy to Kiro Steering (Alternative)

If you prefer to use this as steering files instead of a power:

```bash
# From your project root
mkdir -p .kiro/steering
cp -R powers/aidlc/steering/core-workflow.md .kiro/steering/
cp -R powers/aidlc/rule-details .kiro/
```

## Usage

Once installed as a power:

1. **Activate the workflow** in any Kiro chat by starting with:
   ```
   Using AI-DLC, [describe your software development need]
   ```

2. **AI-DLC will automatically**:
   - Display a welcome message
   - Detect your project type (greenfield/brownfield)
   - Guide you through the appropriate phases
   - Create documentation in `aidlc-docs/` directory

3. **Follow the guided workflow**:
   - Answer structured questions
   - Review and approve execution plans
   - Monitor progress in `aidlc-docs/aidlc-state.md`
   - Check audit trail in `aidlc-docs/audit.md`

## Power Structure

```
powers/aidlc/
├── POWER.md                        # Power documentation with frontmatter
├── README.md                       # This file
├── steering/
│   └── core-workflow.md           # Main AI-DLC workflow
└── rule-details/                  # Detailed rules for each phase
    ├── common/                    # Common rules (always loaded)
    ├── inception/                 # Inception phase rules
    ├── construction/              # Construction phase rules
    └── operations/                # Operations phase rules
```

## What's Different from Original aidlc-rules?

This power packages the AI-DLC methodology as a Kiro Power with:

1. **POWER.md**: Comprehensive documentation with proper frontmatter metadata
2. **Updated paths**: All file references updated to work within the power structure
3. **Organized structure**: Clear separation of steering files and rule details
4. **Easy installation**: Can be installed via Kiro Powers UI

The actual workflow content (all .md files) remains unchanged from the original.

## Additional Resources

- **Blog**: [AI-Driven Development Life Cycle](https://aws.amazon.com/blogs/devops/ai-driven-development-life-cycle/)
- **Method Definition Paper**: [AI-DLC Methodology](https://prod.d13rzhkk8cj2z0.amplifyapp.com/)
- **Original Repository**: [aidlc-workflows](https://github.com/aws-samples/aidlc-workflows)
