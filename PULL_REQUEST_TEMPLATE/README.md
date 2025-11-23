# Pull Request Templates

This directory contains templates for creating standardized pull requests in this repository.

## Available Templates

### Default Template (`../pull_request_template.md`)
The default template used for general pull requests. Includes:
- Description and linked issues
- Type of change (bug fix, feature, breaking change)
- Testing details
- Comprehensive checklist
- Screenshots section

### Feature Template (`feature.md`)
Specialized template for new features. Includes:
- Feature description and motivation
- Implementation details
- Comprehensive testing strategy
- Documentation requirements
- UI/UX changes
- Performance impact assessment
- Breaking changes section

### Hotfix Template (`hotfix.md`)
Template for urgent production fixes. Includes:
- Root cause analysis
- Solution description
- Risk assessment
- Verification checklist
- Rollback plan
- Post-deployment monitoring
- Required approvals

## How to Use

### Using the Default Template
When you create a pull request, GitHub automatically uses the default template.

### Using a Specific Template
To use a specific template:
1. Create a new pull request
2. Add a query parameter to the URL:
   ```
   ?template=feature.md
   or
   ?template=hotfix.md
   ```
3. Or manually copy the content from the desired template

### Example URLs
```
https://github.com/YOUR_ORG/YOUR_REPO/compare/main...feature-branch?template=feature.md
https://github.com/YOUR_ORG/YOUR_REPO/compare/main...hotfix-branch?template=hotfix.md
```

## Template Selection Guide

| Situation | Template | When to Use |
|-----------|----------|-------------|
| General changes | Default | Bug fixes, minor updates, refactoring |
| New functionality | Feature | Adding new features or major enhancements |
| Critical fixes | Hotfix | Production issues requiring immediate attention |

## Customization

You can customize these templates by:
1. Editing existing `.md` files
2. Creating new templates for specific scenarios
3. Adjusting checklists to match your workflow
4. Adding organization-specific requirements

## Best Practices

- Always fill out all required sections
- Link related issues using `Fixes #123` or `Relates to #123`
- Include screenshots for UI changes
- Document breaking changes clearly
- Run all tests before requesting review
- Keep PRs focused and reasonably sized

For more information, see [GitHub's documentation on pull request templates](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests).
