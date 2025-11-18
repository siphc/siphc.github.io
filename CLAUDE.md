# CLAUDE.md - AI Assistant Guide for siphc.github.io

## Repository Overview

This is a minimalist personal website hosted on GitHub Pages. The entire site is intentionally kept simple, lightweight, and accessible, following a philosophy of minimal web design where "most of the web should consist of converted extended markdown documents - because that's all you need."

**Key Stats:**
- Total site size: 22.9KB
- No build process or dependencies
- No JavaScript
- Pure HTML + CSS
- Repository: https://github.com/siphc/siphc.github.io

## Design Philosophy

**CRITICAL:** This site embraces extreme minimalism. Any changes must respect these core principles:

1. **Keep it lightweight** - The site should load instantly, even on slow connections
2. **No JavaScript** - Pure HTML/CSS only
3. **No build tools** - Direct HTML editing, no preprocessors or bundlers
4. **Accessibility first** - Works in even pre-alpha browsers
5. **Content over presentation** - Focus on readable text, not fancy designs
6. **Static and simple** - No frameworks, no complex dependencies

## Project Structure

```
siphc.github.io/
├── index.html       # Main homepage (2.9KB)
├── main.css         # Minimal stylesheet (372 bytes)
├── ffmpeg.webp      # Single image asset (19.7KB)
└── CLAUDE.md        # This file
```

### File Descriptions

#### `index.html` (index.html:1)
- The main and only HTML page
- Contains personal philosophy, recommended readings, and contact info
- Uses semantic HTML with minimal markup
- No divs, no complex structure
- Direct link to CSS, no external dependencies

#### `main.css` (main.css:1)
- Minimal stylesheet with only 6 rules
- Defines:
  - Body layout: centered, max-width 800px, monospace font
  - Link colors: tomato red (#ff6347)
  - Simple hover effects
  - Blockquote and image styling
- Total size: 372 bytes

#### `ffmpeg.webp` (ffmpeg.webp)
- Single image asset referenced in the page
- Quote from @FFmpeg Twitter: "Talk is cheap, send patches."

## Development Workflow

### Making Changes

1. **Edit files directly** - No build process required
2. **Test locally** - Open index.html in a browser to preview
3. **Commit with clear messages** - Keep commit history clean
4. **Push to GitHub** - Changes go live automatically via GitHub Pages

### Git Workflow

```bash
# Create a feature branch
git checkout -b claude/description-sessionid

# Make your changes
# Edit index.html or main.css directly

# Commit with descriptive message
git add .
git commit -m "Brief description of changes"

# Push to remote
git push -u origin claude/description-sessionid
```

### Branch Naming Convention

- Feature branches should start with `claude/`
- Must end with the session ID for AI assistant work
- Example: `claude/claude-md-mi4fm16f3zxz7lu2-01VobkVFRvX6G1AUVAkdn6Fo`

## Coding Conventions

### HTML Guidelines

1. **Minimal markup** - Use as few tags as possible
2. **No classes or IDs** - CSS targets elements directly
3. **Semantic HTML** - Use appropriate tags (h1, h2, p, blockquote, etc.)
4. **No inline styles** - All styling in main.css
5. **No JavaScript** - Ever. Period.
6. **Links without quotes** - Attribute values can be unquoted for brevity
7. **No meta tags** - Only essential: title, favicon, stylesheet

### CSS Guidelines

1. **Minimal selectors** - Target elements directly, no classes
2. **No vendor prefixes** - Keep it simple
3. **Basic properties only** - margin, padding, color, font
4. **Monospace font** - Consistent with design philosophy
5. **Simple colors** - Limited palette (#f2f2f2, #444444, #ff6347)
6. **Max-width for readability** - Keep lines readable on large screens

### Content Guidelines

1. **Plaintext philosophy** - Encourage simple, readable text
2. **External links** - Keep external references as-is
3. **Quotes and references** - Use blockquotes for citations
4. **Technical focus** - Content leans toward programming/systems topics
5. **Minimalist tone** - Avoid verbosity, be direct

## Common Tasks

### Adding a New Link

```html
<!-- In index.html, add to the recommended readings section -->
<p><a href=https://example.com/article>Article Title</a></p>
```

### Modifying Styles

```css
/* In main.css, edit existing rules or add minimal new ones */
/* Keep selectors simple - no classes or complex hierarchies */
```

### Adding an Image

1. **Optimize first** - Use WebP format, compress aggressively
2. **Add to root** - Place image file in repository root
3. **Reference in HTML** - Use simple img tag with alt text
4. **Update size** - Recalculate total site size at bottom of page

### Updating Contact Info

Edit the contacts section in index.html (index.html:24-25)

## Testing Checklist

Before committing changes, verify:

- [ ] Site still loads instantly
- [ ] Total file size hasn't increased significantly
- [ ] No JavaScript has been added
- [ ] CSS is still minimal and readable
- [ ] HTML validates (basic structure check)
- [ ] Links work and are correctly formatted
- [ ] Images are optimized (WebP format, small size)
- [ ] Works without CSS (graceful degradation)
- [ ] Readable in text-only browsers
- [ ] Mobile responsive (via CSS max-width)

## Anti-Patterns (DO NOT DO)

❌ **Never add:**
- JavaScript or TypeScript
- Build tools (webpack, vite, rollup, etc.)
- CSS frameworks (Bootstrap, Tailwind, etc.)
- Package.json or dependencies
- Complex animations or transitions
- External font loading (Web Fonts)
- Analytics or tracking scripts
- Social media widgets
- Multiple pages or navigation
- Backend or API integrations

❌ **Never use:**
- Class names or IDs (unless absolutely necessary)
- Inline styles
- Complex CSS selectors
- Vendor prefixes
- CSS preprocessors (SASS, LESS)
- Heavy images (keep WebP, optimize)

## Performance Considerations

The site is designed to be extremely fast:
- **Target load time:** < 100ms on decent connection
- **Total size budget:** < 30KB for everything
- **HTML size:** < 3KB
- **CSS size:** < 500 bytes
- **Image budget:** < 25KB total

When making changes, monitor file sizes:
```bash
ls -lh index.html main.css ffmpeg.webp
```

## Accessibility

The site is inherently accessible due to its simplicity:
- Semantic HTML structure
- No JavaScript required
- High contrast text
- Readable font size (18px)
- No color-only indicators
- Works with screen readers
- Keyboard navigation (native links)

## Deployment

The site is automatically deployed via GitHub Pages:
- **URL:** https://siphc.github.io
- **Source:** Main/master branch root directory
- **Deploy time:** ~1-2 minutes after push
- **No build step** - Files served as-is

## Git History

Recent commits:
- `08acc73` - Hopefully improve readability on mobile devices
- `03bf3d4` - Squashed commit of the following
- `4c56a13` - first commit

Keep commit messages clear and concise.

## Key Files to Never Delete

- `index.html` - The main page
- `main.css` - The stylesheet
- `ffmpeg.webp` - Referenced image

## Resources and References

The site itself references these concepts:
- Lightweight web design philosophy
- Unix philosophy applied to web
- Minimalist coding practices
- Plain text communication

## Contact

For questions about the site content or design decisions, refer to the contact section in index.html (index.html:25).

---

**Last Updated:** 2025-11-18
**Repository Owner:** siphc
**AI Assistant:** Claude (Anthropic)
**Purpose:** Guide for AI assistants working on this minimalist personal website
