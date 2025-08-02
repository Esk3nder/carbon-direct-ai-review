# Custom GPT Configuration Guide

## Prerequisites
- ChatGPT Plus subscription (required for Custom GPTs)
- All static documents organized per the Document Audit Checklist
- Files optimized to meet size limits (20MB per file, 100MB total)

## Step 1: Access GPT Builder
1. Go to [chat.openai.com](https://chat.openai.com)
2. Click on your profile in the bottom left
3. Select "My GPTs" 
4. Click "Create a GPT"

## Step 2: Basic Configuration
### In the "Create" tab:
1. **Name**: "AI Review Assistant"
2. **Description**: "Conducts structured project reviews against quality criteria for ARR, IFM, and other project types"
3. **Profile Picture**: Upload company logo or relevant icon (optional)

### Initial Conversation with Builder:
The GPT Builder will ask what you want to create. Respond:
```
"I want to create an AI assistant that helps conduct project reviews. It should guide users through uploading project documents, apply quality criteria automatically based on project type (ARR, IFM, etc.), and output structured evaluation tables. The assistant should be simple for non-technical users but thorough in analysis."
```

## Step 3: Upload Knowledge Base
### In the "Configure" tab, under "Knowledge":
Upload these files in order:

1. **Quality Criteria.pdf** 
   - Core quality standards (universal)

2. **ARR Shoulds and Musts documents**
   - All ARR-specific criteria files

3. **IFM Shoulds and Musts documents** 
   - All IFM-specific criteria files

4. **Prior ARR Reviews**
   - Representative examples (if > 20MB, split into multiple files)

5. **Prior IFM Reviews**
   - Representative examples (if > 20MB, split into multiple files)

### File Organization Tips:
- If splitting large files, name them clearly: "Prior_ARR_Reviews_Part1.pdf", "Prior_ARR_Reviews_Part2.pdf"
- Verify all files uploaded successfully (green checkmarks)
- Total knowledge base should stay under 100MB

## Step 4: Configure Instructions
### In the "Configure" tab, under "Instructions":
Copy and paste the entire content from `custom-gpt-instructions.md`

### Key sections to verify:
- ✅ Conversation flow is included
- ✅ Output format requirements are specified  
- ✅ Table structure is defined
- ✅ Behavioral guidelines are included

## Step 5: Configure Capabilities
### Enable these capabilities:
- ✅ **Web Browsing**: OFF (not needed, reduces confusion)
- ✅ **DALL-E Image Generation**: OFF (not needed)
- ✅ **Code Interpreter**: ON (helps with data analysis if needed)

## Step 6: Conversation Starters
Add these suggested conversation starters:
```
1. "Start new ARR project review"
2. "Start new IFM project review"  
3. "Help me review a project"
4. "What documents do I need for review?"
```

## Step 7: Privacy Settings
### Under "Additional Settings":
- **Sharing**: Set to "Only people with the link" (for team access)
- **Data Usage**: Keep default settings
- **Custom Actions**: Leave blank (not needed)

## Step 8: Testing Phase
### Test with sample documents:
1. Start a new conversation with your Custom GPT
2. Test ARR project flow:
   - Say "Start new ARR project review"
   - Follow the prompts
   - Upload sample ARR documents
   - Verify output matches template format

3. Test IFM project flow:
   - Start fresh conversation
   - Say "Start new IFM project review"  
   - Upload sample IFM documents
   - Verify output quality

### What to verify during testing:
- ✅ GPT asks for project type correctly
- ✅ GPT requests developer name
- ✅ GPT guides document upload process
- ✅ GPT applies correct criteria for project type
- ✅ Output table matches template format
- ✅ Scoring is consistent and reasonable
- ✅ Recommendations are actionable

## Step 9: Sharing with Team
1. Click "Save" in the GPT Builder
2. Your GPT will be available at a unique URL
3. Share this URL with team members
4. Create bookmark or add to team documentation

### Team Access Instructions:
```
Team GPT Access: [Your Custom GPT URL]

How to use:
1. Click the link above (requires ChatGPT Plus)
2. Start conversation with project type (e.g., "Start new ARR project review")
3. Follow the prompts to upload documents
4. Copy the resulting table for your workflow
```

## Step 10: Maintenance and Updates

### When to update the GPT:
- Quality criteria documents change
- New project types added
- Prior review examples need refreshing
- User feedback suggests improvements

### How to update:
1. Go to "My GPTs" in ChatGPT
2. Find "AI Review Assistant" 
3. Click "Edit"
4. Update knowledge base files or instructions as needed
5. Re-test with sample documents
6. Save changes

### Version Control:
Keep a record of updates:
```
Version 1.0 - Initial setup with ARR/IFM support
Version 1.1 - Added [new project type] support  
Version 1.2 - Updated quality criteria (Date: XX/XX/XXXX)
```

## Troubleshooting Common Issues

### Knowledge Base Upload Failures:
- **Issue**: File too large
- **Solution**: Split into smaller files or create "key excerpts" version

### Inconsistent Outputs:
- **Issue**: GPT gives different table formats
- **Solution**: Make instructions more specific, add more examples

### Missing Project Types:
- **Issue**: GPT doesn't recognize project type
- **Solution**: Add project type to instructions and upload relevant criteria

### User Confusion:
- **Issue**: Users don't know how to start
- **Solution**: Update conversation starters, create user guide

## Success Metrics
Track these to measure Custom GPT success:
- Time saved per review (target: 50% reduction)
- Output consistency (target: 95% match template format)
- User adoption rate within team
- Reduction in manual prompt creation errors

## Backup Plan
Always maintain:
- Backup copies of all knowledge base files
- Copy of current GPT instructions 
- Access to original manual process documentation