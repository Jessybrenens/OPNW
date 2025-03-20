# GitHub Version Control Guidelines

**Note: The repository URL and Personal Access Token are located in the README.txt file.**

## Initial Setup

```bash
# Clone the repository using credentials from README.txt
git clone https://[PERSONAL_ACCESS_TOKEN]@[REPOSITORY_URL without https://]

# Configure Git user information
git config --global user.email "manus@example.com"
git config --global user.name "Manus AI"

# Verify repository contents
ls -la [repository directory]

# Review prompt file
cat [repository directory]/Prompt.md

# Create project structure
mkdir -p planning drafts final exercises

# Create progress tracking file
touch PROGRESS.md

# Initial commit
git add .
git commit -m "[INIT] Create project directory structure"
git push origin main
```

## Document Creation and Management

1. Create Parameters.md with all novel specifications
   - Commit with message "[INIT] Define novel parameters"

2. Create all planning documents in /planning directory
   - Commit each document separately with descriptive messages
   - Update PROGRESS.md after each milestone

## Development Phases

- Foundation Building (15% of process)
- Structural Development (25% of process)
- Content Creation (40% of process)
- Refinement (20% of process)

## Commit Guidelines

Commit at logical breakpoints using these prefixes:
- [PLAN] - Planning document updates
- [DRAFT] - New chapter drafts
- [REVISE] - Content revisions
- [EDIT] - Editorial improvements
- [EXERCISE] - Writing exercises and experiments
- [FINAL] - Final version files

Remember to push changes regularly:
```bash
git push origin main
```

## Implementation References

Reference Appendix in Prompt.md for:
- Four-Stage Editing Process
- Practical Exercises Implementation
- Emotional Impact Strategy
- Argumentation and Persuasion Framework
- Rhetorical Device Implementation

Create implementation files in /exercises directory
Apply techniques to draft chapters in /drafts directory
Track improvements in PROGRESS.md

## Editing Process

Apply four-layer editing pyramid:
- Structural Editing
- Content Editing
- Paragraph and Sentence Editing
- Technical Editing

## Final Delivery

Compile final manuscript in /final directory:
- Create individual chapter files
- Create complete manuscript as [TITLE].md
- Generate COMPLETION.md with word count and summary

```bash
git add .
git commit -m "[FINAL] Complete [TITLE] narrative"
git push origin main
```

## When to Commit

Commit after:
- Completing planning documents
- Drafting chapters
- Major revision phases
- Implementing techniques
- Reaching word count milestones
- Before taking breaks

## Commit Message Format

```
[PREFIX] Brief description of changes

- Detailed bullet point about specific change
- Another specific detail about the changes made
- Any challenges addressed or decisions made
```

## Troubleshooting

Authentication issues:
- Verify Personal Access Token from README.txt
- Ensure token has appropriate permissions
- Try HTTPS URL format with embedded token

Merge conflicts:
```bash
git pull origin main
# Resolve conflicts by editing files
git add [conflicted-files]
git commit -m "Resolve merge conflicts"
```

Connection problems:
- Verify internet connectivity
- Try again after brief pause
- Save work locally and attempt push later

## Deliverables

Deliver as:
- Individual chapter files in /final/ directory
- Complete manuscript as [TITLE].md in repository root
- Final word count and completion report in COMPLETION.md
- Development process documentation in PROCESS.md
