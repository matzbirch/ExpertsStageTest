# Popup Configuration Guide

## Overview
The popup cards that appear when clicking on author objects can be easily customized by editing the `popup-config.json` file.

## File Location
- **Configuration File**: `popup-config.json`
- **Report Images**: `Reports webp/` folder (Report1.webp through Report8.webp)

## Configuration Structure

The configuration file contains information for each author (1-8) with the following structure:

```json
{
  "authors": {
    "1": {
      "name": "Author 1",
      "title": "Expert Title 1", 
      "subtext": "Detailed description of the expert's background and expertise..."
    }
  }
}
```

## Editing Content

### To modify an author's information:

1. Open `popup-config.json` in any text editor
2. Find the author number you want to edit (1-8)
3. Modify the following fields:
   - **name**: The author's name (appears in top-left)
   - **title**: The main title (appears as large text on the right)
   - **subtext**: The description text (appears below the title)

### Example:
```json
"3": {
  "name": "Dr. Sarah Johnson",
  "title": "AI Research Specialist",
  "subtext": "Leading expert in machine learning and artificial intelligence with over 15 years of experience in developing cutting-edge algorithms for enterprise solutions."
}
```

## Image Management

- **Report Images**: The popup displays images from `Reports webp/Report[X].webp` where [X] is the author number
- **Image Requirements**: 
  - Format: WebP
  - Recommended size: 300x300 pixels (will be automatically cropped to fit)
  - Naming: Report1.webp, Report2.webp, etc.

## Tips for Writing Content

### Title Guidelines:
- Keep titles concise (2-4 words)
- Use professional titles or specializations
- Examples: "Data Science Expert", "Cloud Architect", "Security Specialist"

### Subtext Guidelines:
- Aim for 2-3 sentences
- Highlight key expertise areas
- Mention years of experience if relevant
- Keep it professional and engaging
- Recommended length: 100-200 characters

## Validation

After editing the configuration file:
1. Ensure the JSON syntax is valid (use a JSON validator if needed)
2. Save the file
3. Refresh the webpage to see changes
4. Test by clicking on author objects

## Troubleshooting

**If popup content doesn't update:**
- Check that the JSON syntax is valid
- Ensure the file is saved as `popup-config.json`
- Clear browser cache and refresh

**If images don't display:**
- Verify image files exist in `Reports webp/` folder
- Check that filenames match the pattern `Report[X].webp`
- Ensure images are in WebP format

## Backup

Always keep a backup of your `popup-config.json` file before making changes, especially when making bulk edits. 