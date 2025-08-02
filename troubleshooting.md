# Troubleshooting Guide

## Common Setup Issues

### GPT Instructions Too Long
**Problem:** Error when pasting instructions into Custom GPT
**Cause:** Instructions exceed 8,000 character limit
**Solution:** Use the condensed version from `gpt-configuration/instructions.md` (5,484 characters)

### Knowledge Base Upload Failures
**Problem:** Files won't upload to GPT knowledge base
**Causes & Solutions:**
- **File too large (>20MB):** Split large files or create excerpts of key sections
- **Total size >100MB:** Remove less critical documents or create summary versions
- **Unsupported format:** Convert to PDF or text format
- **Corrupted file:** Re-export or recreate the file

### Custom GPT Not Accessible to Team
**Problem:** Team members can't access the GPT
**Solution:** In GPT settings, set sharing to "Anyone with the link" and share the URL

## Usage Issues

### Missing Quote Sources
**Problem:** Analysis table missing document references
**Root Cause:** GPT not following quote requirements
**Solutions:**
1. Remind the GPT: "Please include (Document Name, p.X) for every quote"
2. Restart conversation if problem persists
3. Check that instructions include the hard requirement for sources

### Incomplete Additionality Analysis
**Problem:** Only financial additionality covered, missing common practice and regulatory
**Root Cause:** Hard-coded requirement not followed
**Solutions:**
1. Explicitly ask: "Please cover all 3 additionality types: financial, common practice, and regulatory"
2. Verify the condensed instructions include the hard-coded requirement
3. Restart conversation with fresh context

### Wrong Scoring Scale
**Problem:** GPT using 1-5 scale instead of 1-4
**Root Cause:** Instructions not updated or GPT confusion
**Solution:** Remind GPT: "Please use 1-4 scoring scale only"

### Missing Species Lists
**Problem:** Environmental section lacks species planting list
**Root Cause:** Hard-coded requirement not followed
**Solution:** Ask: "Please include species planting list with scientific and common names"

### Durability Hallucinations
**Problem:** GPT making up durability benchmarks or citing non-existent standards
**Root Cause:** Not using hard-coded durability rule
**Solution:** Remind GPT of exact rule: "Durability terms range 1-1,000's years by project type. Typically clients prefer >10-year terms based on goals, claims, credit use"

## Document Upload Issues

### File Upload Errors
**Problem:** Documents won't upload during conversation
**Solutions:**
- **Check file size:** Must be <20MB per file
- **Try different format:** PDF usually works best
- **One at a time:** Upload documents individually, not in batch
- **Refresh page:** Sometimes ChatGPT interface needs refresh

### Document Not Recognized
**Problem:** GPT says it can't read uploaded document
**Solutions:**
- **Check file integrity:** Ensure file isn't corrupted
- **Remove password protection:** GPT can't read password-protected files
- **Convert format:** Try converting to PDF if using other formats
- **Re-upload:** Sometimes re-uploading the same file works

## Workflow Issues

### GPT Skips Stages
**Problem:** GPT jumps directly to final document without Stage 1 or 2A
**Solution:** Explicitly guide through stages:
1. "Please start with Stage 1 analysis table"
2. "Now provide Stage 2A bullet structure"
3. "Now let's do section-by-section collaboration"

### Section-by-Section Not Working
**Problem:** GPT creates entire document instead of working section by section
**Solutions:**
1. Say explicitly: "Please present ONLY the Overview section first"
2. After feedback: "Now present ONLY the Highlights section"
3. Continue one section at a time

### Inconsistent Output Format
**Problem:** Outputs don't match Carbon Direct template
**Solutions:**
1. Reference the template: "Please follow exact Carbon Direct format"
2. Provide specific formatting instructions for problem sections
3. Restart conversation if formatting continues to be wrong

## Performance Issues

### Slow Response Times
**Problem:** GPT takes unusually long to respond
**Causes & Solutions:**
- **Large documents:** Consider breaking into smaller files
- **Complex requests:** Break into simpler steps
- **ChatGPT server load:** Try again during off-peak hours
- **Network issues:** Check internet connection

### Incomplete Responses  
**Problem:** GPT stops mid-response or provides partial answers
**Solutions:**
- Say "Please continue" to get the rest of the response
- Break complex requests into smaller parts
- Start fresh conversation if problem persists

## Quality Control Issues

### Missing Critical Analysis
**Problem:** Stage 1 critique section too brief or missing elements
**Solution:** Ask for specific components:
- "Please provide document discrepancies analysis"
- "Please identify missing information gaps"
- "Please compare to Carbon Direct template structure"

### Bullet Points Too Brief
**Problem:** Stage 2A bullets lack sufficient detail
**Solution:** Request expansion: "Please provide more detailed bullets with additional context and quotes"

### Actions for Analyst Unclear
**Problem:** Analyst action items too vague
**Solution:** Ask for specific, actionable items: "Please make analyst actions more specific and actionable"

## Emergency Solutions

### Complete Reset
If multiple issues persist:
1. Start completely new conversation
2. Re-upload all documents
3. Follow workflow from beginning
4. Be explicit about requirements at each stage

### Escalation Process
If technical issues continue:
1. Test with simpler/smaller documents
2. Try different time of day (server load)
3. Check ChatGPT status page for outages
4. Contact IT support with specific error messages

### Backup Workflow
If GPT is completely unavailable:
1. Use manual process with saved prompts
2. Reference output templates for formatting
3. Apply quality checklist manually
4. Return to GPT when available for quality check

## Prevention Tips

### Best Practices
- **Start fresh conversations** for each new project review
- **Upload documents one at a time** and wait for confirmation
- **Be explicit about requirements** rather than assuming GPT remembers
- **Save successful conversations** as examples for future reference
- **Test with sample documents** before using on critical projects

### Maintenance
- **Update GPT instructions** when Carbon Direct standards change
- **Refresh knowledge base** periodically with new prior reviews
- **Monitor output quality** and adjust instructions as needed
- **Train team members** on proper usage patterns

## Getting Help

### Documentation Resources
- Review [User Guide](user-guide.md) for complete workflow
- Check [Quick Reference](quick-reference.md) for command shortcuts
- Reference [Configuration Guide](../gpt-configuration/configuration-steps.md) for setup issues

### Support Contacts
- **Technical Issues:** [INSERT IT SUPPORT CONTACT]
- **Process Questions:** [INSERT PROCESS OWNER CONTACT]  
- **General Support:** [INSERT MAIN SUPPORT CONTACT]

### Useful Information to Provide
When seeking help, include:
- Specific error messages
- Steps taken before the issue occurred
- Screenshots of problem areas
- Document types and sizes being used
- Which stage of the workflow the issue occurs