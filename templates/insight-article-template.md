# Obsidian Insight Article Template

<!-- 
This template provides a structure for creating insight articles with comprehensive help text for all markdown elements.
Replace all placeholder text with your actual content and remove help comments before publishing.
-->

---
title: "Your Article Title Here"
author: "Author Name"
date: "YYYY-MM-DD"
categories: ["Category 1", "Category 2", "Category 3"]
featured_image: "/insights/images/your-image.png"
youtube_video: ""
excerpt: "Brief 1-2 sentence summary that will appear in previews and social shares."
featured_on_homepage: false
priority: 5
draft: true
featured_link: "https://example.com"
---

<!-- 
FRONTMATTER HELP:
- title: The main title of your article (use quotes for titles with punctuation)
- author: Full name of the article author
- date: Publication date in YYYY-MM-DD format
- categories: Array of relevant categories (max 3 recommended)
- featured_image: Path to main article image (always include thumbnails per user preference)
- youtube_video: YouTube URL if article includes video content
- excerpt: Short description for SEO and social sharing (keep under 160 characters)
- featured_on_homepage: Boolean - whether to highlight on homepage
- priority: Number 1-10 for sorting (higher = more important)
- draft: Set to true to prevent publishing
- featured_link: Optional external link related to the article
-->

# Your Main Article Title

<!-- 
HEADING HELP:
# H1 - Main title (use only once per article)
## H2 - Major sections
### H3 - Subsections
#### H4 - Minor subsections
##### H5 - Rarely used
###### H6 - Rarely used

Keep headings descriptive and scannable. Use sentence case, not title case.
-->

## Introduction Section

Write your compelling introduction here. This should hook the reader and clearly state what they'll learn from this article.

<!-- 
PARAGRAPH HELP:
- Keep paragraphs to 1-3 sentences for web readability
- Use active voice when possible
- Start with your strongest points
- End paragraphs with a transition to the next idea
-->

**Bold text** is used for emphasis on key terms and concepts.
*Italic text* is used for subtle emphasis or introducing new terminology.
***Bold italic text*** combines both for maximum emphasis (use sparingly).

<!-- 
TEXT FORMATTING HELP:
**bold** or __bold__ - Use for key terms, important concepts
*italic* or _italic_ - Use for emphasis, book titles, foreign words
***bold italic*** or ___bold italic___ - Use very sparingly for critical points
~~strikethrough~~ - Use for corrections or showing changes
`inline code` - Use for code snippets, file names, technical terms
-->

## Lists and Organization

### Unordered Lists
Use bullet points for non-sequential information:

- First important point
- Second key insight
  - Sub-point with additional detail
  - Another supporting detail
- Third main point

<!-- 
LIST HELP:
Unordered lists (bullets):
- Use hyphens (-), asterisks (*), or plus signs (+)
- Indent with 2 spaces for sub-items
- Keep items parallel in structure
- Use for non-sequential information

Ordered lists (numbers):
1. Use for step-by-step instructions
2. Or for ranked information
3. Numbers auto-increment
   1. Sub-items use indented numbers
   2. Maintain consistent indentation
-->

### Ordered Lists
Use numbers for sequential steps or ranked information:

1. First step in the process
2. Second step with more detail
   1. Sub-step for clarification
   2. Additional sub-step
3. Final step

### Task Lists
Use for actionable items:

- [x] Completed task
- [ ] Pending task
- [ ] Another task to complete

<!-- 
TASK LIST HELP:
- [x] Completed checkbox
- [ ] Empty checkbox
- Use for actionable items, checklists, progress tracking
-->

## Quotes and Citations

### Blockquotes

> This is a standard blockquote. Use for highlighting important insights, customer testimonials, or key concepts that deserve special attention.

<!-- 
BLOCKQUOTE HELP:
> Single line blockquote
>
> Multi-paragraph blockquotes
> need empty lines with just >

Use blockquotes for:
- Important insights or key takeaways
- Customer testimonials
- Quotes from interviews or sources
- Highlighting contrarian or surprising points
-->

> **Pro Tip:** You can combine formatting within blockquotes for added emphasis.
> 
> This creates multi-paragraph quotes that stand out from regular text.

### Nested Blockquotes

> Main quote or insight
> 
> > Nested quote within the main quote
> 
> Back to the main quote level

## Code and Technical Content

### Inline Code
Use `backticks` for inline code, file names like `config.json`, or technical terms like `localStorage.getItem()`.

<!-- 
Note: Following user preference to never use localStorage.getItem('access_token') in examples
-->

### Code Blocks

```javascript path=null start=null
// Example JavaScript code block
function createInsightArticle(title, content) {
    return {
        title: title,
        content: content,
        timestamp: new Date(),
        author: 'Your Name'
    };
}

// This is hypothetical code for demonstration
const article = createInsightArticle('My Title', 'My content');
```

<!-- 
CODE BLOCK HELP:
```language path=file_path start=line_number
code goes here
```

For real code from files:
```javascript path=/Users/me/project/src/index.ts start=25
// actual code from file
```

For example/hypothetical code:
```javascript path=null start=null
// example code
```

Supported languages: javascript, typescript, python, html, css, bash, sql, json, yaml, etc.
-->

```bash path=null start=null
# Example bash commands
npm install
npm run build
docker-compose up -d
```

```typescript path=null start=null
// TypeScript example (following user preference for TypeScript frontend)
interface InsightArticle {
    title: string;
    author: string;
    publishDate: Date;
    categories: string[];
    featured: boolean;
}

const article: InsightArticle = {
    title: "My Insight Article",
    author: "Author Name", 
    publishDate: new Date(),
    categories: ["AI", "Development"],
    featured: true
};
```

## Links and References

### Basic Links
[Link text](https://example.com) - Standard link format
[Internal link](/insights/another-article) - Link to other pages
[Link with title](https://example.com "This appears on hover") - Link with tooltip

<!-- 
LINK HELP:
[text](url) - Basic link
[text](url "title") - Link with hover tooltip
[text](relative-path) - Internal site links
[text](#heading-id) - Link to heading within same page
[text][reference] - Reference-style link (define reference at bottom)

For external links, consider if they should open in new tabs (handled by your site's JavaScript)
-->

### Reference Links
You can use reference-style links for cleaner text: [Example Site][example] or [Another Reference][ref2].

[example]: https://example.com "Example site tooltip"
[ref2]: https://another-example.com

### Automatic Links
<https://example.com> - Automatic link formatting
<email@example.com> - Automatic email links

## Images and Media

### Basic Image
![Alt text describing the image](/insights/images/example-image.png)

<!-- 
IMAGE HELP:
![alt text](image-path)
![alt text](image-path "title text")

Alt text is crucial for:
- Accessibility (screen readers)
- SEO optimization
- When images fail to load

Always include thumbnails per user preference
Image paths should be relative to your site root
-->

### Image with Title
![Detailed alt text for accessibility](/insights/images/example-with-title.png "This text appears on hover")

### Linked Images
[![Alt text for linked image](/insights/images/clickable-image.png)](https://destination-url.com)

## Advanced Elements

### Tables

| Feature | Description | Priority | Status |
|---------|-------------|----------|--------|
| User Authentication | First party cookies (per user preference) | High | ✅ Complete |
| Database | PostgreSQL implementation | High | ✅ Complete |
| Frontend | TypeScript development | Medium | 🔄 In Progress |
| Docker Setup | Ports 3000 (frontend) & 8000 (backend) | Low | 📋 Planned |

<!-- 
TABLE HELP:
| Header 1 | Header 2 | Header 3 |
|----------|----------|----------|
| Row 1    | Data     | More     |
| Row 2    | Data     | More     |

Alignment options:
|:--------|  Left-aligned
|--------:| Right-aligned  
|:-------:| Center-aligned

Use tables for:
- Comparing features or options
- Displaying structured data
- Creating simple layouts
Keep tables simple - complex data might need different formatting
-->

### Horizontal Rules
Use three or more hyphens, asterisks, or underscores for section breaks:

---

### Line Breaks and Spacing
End a line with two spaces  
to create a line break without starting a new paragraph.

Leave blank lines between paragraphs for proper spacing.

## Sidebar Elements (Obsidian-specific)

### Callout Boxes

> [!note]
> This is a note callout. Use for additional information that supports your main content.

> [!tip]
> This is a tip callout. Use for helpful advice or best practices.

> [!warning]
> This is a warning callout. Use for important caveats or potential issues.

> [!info]
> This is an info callout. Use for factual information or context.

> [!success]
> This is a success callout. Use for positive outcomes or achievements.

> [!error]
> This is an error callout. Use for mistakes to avoid or problems encountered.

<!-- 
OBSIDIAN CALLOUT HELP:
> [!type] Title (optional)
> Content goes here
> Can span multiple lines

Available types: note, abstract, info, todo, tip, success, question, warning, failure, danger, bug, example, quote
Each type has different colors and icons in Obsidian
-->

### Collapsible Sections

<details>
<summary>Click to expand this section</summary>

Hidden content goes here. This is useful for:
- Detailed technical explanations
- Optional deep-dive information  
- FAQ answers
- Code examples that might clutter the main text

You can include any markdown formatting inside collapsible sections.

```javascript path=null start=null
// Even code blocks work inside details
console.log('This code is hidden by default');
```

</details>

<!-- 
COLLAPSIBLE HELP:
<details>
<summary>Visible title/summary</summary>
Hidden content here
</details>

Great for:
- Optional technical details
- Long code examples
- FAQ sections
- Reducing visual clutter
-->

## Iframe Embeds

### YouTube Video Embed
<iframe width="560" height="315" src="https://www.youtube.com/embed/VIDEO_ID" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### Custom Iframe
<iframe src="https://example.com" width="100%" height="400px" frameborder="0" title="Embedded content description"></iframe>

<!-- 
IFRAME HELP:
<iframe src="URL" width="WIDTH" height="HEIGHT" frameborder="0" title="DESCRIPTION"></iframe>

Key attributes:
- src: The URL to embed
- width/height: Dimensions (can use px, %, or responsive units)
- frameborder: Usually set to "0" for clean appearance
- title: Required for accessibility
- allow: Permissions for the embedded content
- allowfullscreen: For video content

Common use cases:
- YouTube/Vimeo videos
- Interactive demos
- Maps
- Third-party widgets
- CodePen examples
-->

## Special Characters and Escaping

### Characters that need escaping:
To display these literally, add a backslash before them:
\* \_ \# \[ \] \( \) \` \~ \| \\

### HTML Entities:
&copy; - Copyright symbol
&trade; - Trademark symbol  
&reg; - Registered trademark
&amp; - Ampersand
&lt; - Less than
&gt; - Greater than

<!-- 
ESCAPING HELP:
Use backslash (\) before special markdown characters to display them literally:
\* \_ \# \[ \] \( \) \` \~ \| \\

HTML entities for special symbols:
&copy; &trade; &reg; &amp; &lt; &gt; &nbsp;
-->

## Footnotes

Here's a sentence with a footnote reference[^1].

You can also use named footnotes[^note-name] for better organization.

Multiple references to the same footnote work too[^1].

[^1]: This is the footnote content. It will appear at the bottom of the document.
[^note-name]: Named footnotes are easier to manage in long documents.

<!-- 
FOOTNOTE HELP:
In text: [^identifier]
At bottom: [^identifier]: Footnote content

Identifiers can be:
- Numbers: [^1], [^2]
- Names: [^note-name], [^important]
- Any text: [^this-is-valid-too]

Footnotes automatically:
- Appear at document bottom
- Are numbered sequentially
- Include back-links to references
-->

## Math Expressions (if supported)

Inline math: $E = mc^2$

Block math:
$$
\sum_{i=1}^{n} x_i = x_1 + x_2 + \cdots + x_n
$$

<!-- 
MATH HELP (requires MathJax or similar):
Inline: $equation$
Block: $$equation$$

Use for mathematical formulas, equations, or scientific notation
Syntax follows LaTeX math formatting
-->

## Conclusion

This template covers all the major markdown elements you'll need for creating engaging insight articles. Remember to:

### Content Best Practices:
- **Start strong** with a compelling hook
- **Use subheadings** to break up long sections  
- **Include visuals** - always add thumbnails per your preference
- **End with action** - clear next steps for readers

### Technical Considerations:
- Follow your preferences: TypeScript for frontend, PostgreSQL for database
- Use Docker ports 3000 (frontend) and 8000 (backend)
- Never commit .env files to version control
- All validations run in pre-push hooks
- Never bypass pre-commits or use --no-verify

### SEO and Accessibility:
- Write descriptive alt text for all images
- Use proper heading hierarchy (H1 → H2 → H3)
- Keep paragraphs short for web readability
- Include relevant internal and external links

---

**Ready to create your next insight article?**

1. Copy this template
2. Replace all placeholder content
3. Remove help comments
4. Add your unique insights and perspective
5. Include compelling visuals with thumbnails
6. Review and publish

---

*Need help with content strategy or technical implementation? [Contact our team](/contact) to discuss how we can support your content goals.*

<!-- 
TEMPLATE USAGE NOTES:
1. Replace all placeholder text with your actual content
2. Remove all help comments (<!-- --> sections) before publishing
3. Customize the frontmatter for each article
4. Always include relevant images with proper alt text
5. Test all links before publishing
6. Use the preview function to check formatting
7. Consider your audience's technical level when using advanced elements
-->