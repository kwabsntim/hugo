# Beginner's Guide to Contributing to Hugo

Welcome! This guide will help you understand what kinds of contributions beginners can make to the Hugo project and how to identify them.

## Issues Fixed in This PR

This pull request demonstrates the kind of simple, valuable contributions that beginners can make. Here's what was fixed:

### 1. Typo Fix in CONTRIBUTING.md (Line 1)
**Issue:** "apprecitate" → **Fixed:** "appreciate"
- **How to find:** Read through documentation files looking for spelling mistakes
- **Skills needed:** Good spelling and attention to detail
- **Impact:** Makes the project look more professional and easier to read

### 2. Outdated CI Reference (Line 79)
**Issue:** "Travis CI" → **Fixed:** "GitHub Actions"
- **How to find:** Look for references to old tools/services and check if they're still in use
- **Skills needed:** Basic understanding of the project's infrastructure
- **Impact:** Prevents confusion for new contributors

## How to Find Similar Issues

### 1. **Documentation Improvements**
Look through these files for issues:
- `README.md` - The main project description
- `CONTRIBUTING.md` - Contribution guidelines
- `SECURITY.md` - Security policies
- Files in the `/docs` directory

**What to look for:**
- Spelling and grammar mistakes
- Broken or outdated links
- References to deprecated tools (e.g., Travis CI when using GitHub Actions)
- Unclear instructions that could be improved
- Missing information that would help users

### 2. **Code Comments**
Search through the codebase for:
- Typos in comments
- Outdated comments that don't match the current code
- TODOs that might be completed but not removed

**Example commands:**
```bash
# Find potential typos in comments
grep -r "TODO" . --include="*.go"
grep -r "FIXME" . --include="*.go"
```

### 3. **Test Coverage**
Look for:
- Functions without test cases
- Edge cases not covered by existing tests
- Outdated test data or mocks

### 4. **Small Bug Fixes**
- Check the [issue tracker](https://github.com/gohugoio/hugo/issues) for issues labeled "good first issue" or "beginner-friendly"
- Look for simple bugs that you can reproduce and fix

## Tools to Help You

### Spell Checkers
```bash
# Install and use a spell checker
# Example with aspell (you may need to install it)
aspell check CONTRIBUTING.md
```

### Link Checkers
```bash
# Check for broken links (if you have the tool installed)
markdown-link-check README.md
```

### Linters
```bash
# The project uses Go, so format your code before submitting
go fmt ./...

# Run the project's checks
mage check
```

## Before Submitting Your Contribution

1. **Read CONTRIBUTING.md** - Understand the project's contribution guidelines
2. **Test your changes** - Make sure you haven't broken anything
3. **Follow commit message guidelines** - Use proper format (e.g., "docs: Fix typo in CONTRIBUTING.md")
4. **Create a clear PR description** - Explain what you fixed and why
5. **Sign the CLA** - Required for all contributors

## Types of Beginner-Friendly Contributions

### Very Easy 🌱
- Fix typos and grammar in documentation
- Update broken links
- Improve code comments
- Add missing documentation

### Easy 🌿
- Update outdated references (like Travis CI → GitHub Actions)
- Add examples to documentation
- Improve error messages
- Write simple tests

### Moderate 🌳
- Fix small bugs with clear reproduction steps
- Improve existing features based on user feedback
- Add validation or error handling
- Optimize simple algorithms

## What Was Learned From This PR

1. **Always verify your changes** - We checked that:
   - GitHub Actions is actually being used (checked `.github/workflows/`)
   - The typo was consistently wrong (only one instance)
   - The changes make sense in context

2. **Keep changes minimal** - Only fix what's necessary
   - Don't reformat entire files
   - Don't make multiple unrelated changes in one PR

3. **Test before submitting** - Even for documentation:
   - Read the changes in context
   - Check that links still work
   - Verify formatting is correct

## Where to Get Help

- **Forum:** [Hugo Discourse](https://discourse.gohugo.io) - For questions and discussions
- **Issue Tracker:** [GitHub Issues](https://github.com/gohugoio/hugo/issues) - For bugs and feature requests
- **Documentation:** [Hugo Docs](https://gohugo.io/documentation) - For learning about Hugo

## Next Steps

After your first contribution:
1. Look for more "good first issue" labels
2. Help answer questions on the forum
3. Improve existing documentation based on your experience
4. Test new features and report bugs
5. Gradually take on more complex issues

Remember: Every expert contributor started as a beginner. The Hugo community is welcoming and will help you learn!

---

**Good luck with your contributions! 🚀**
