# 📚 Developer Guide for Hyena Website

Welcome! This guide will help you make simple changes to the Hyena Realty website, even if you're not a technical person. Everything is explained step-by-step with examples.

## 📋 Quick Reference

- **Add new blog post**: Create a file in `_posts/` folder
- **Upload images**: Add files to `assets/images/` folder
- **Edit existing post**: Open and modify files in `_posts/` folder
- **File naming**: Use `YYYY-MM-DD-title-of-post.md` format

---

## 🆕 How to Add a New Blog Post

### Step 1: Create the File

1. Go to the `_posts/` folder in your repository
2. Create a new file with this naming format:
   ```
   YYYY-MM-DD-title-of-your-post.md
   ```

**Example:**
- If today is February 4, 2026, and you want to write about "New Property Listings", name your file:
  ```
  2026-02-04-new-property-listings.md
  ```

### Step 2: Add the Front Matter

Every blog post starts with "front matter" - a section at the top between `---` lines that contains information about the post.

Copy and paste this template at the very beginning of your file:

```markdown
---
layout: post
title: "Your Post Title Here"
author: admin
categories: [ ]
image: assets/images/your-image.jpg
---
```

**Example:**
```markdown
---
layout: post
title: "5 Beautiful Homes Available This Week"
author: admin
categories: [ ]
image: assets/images/homes-feb-2026.jpg
---
```

**What each field means:**
- `layout: post` - Always use "post" for blog posts (don't change this)
- `title` - The title that appears at the top of your post (use quotes)
- `author` - Your author name (use: admin, sal, or john)
- `categories` - Leave empty `[ ]` or add categories like `[ Real Estate, Tips ]`
- `image` - Path to the featured image (must be in `assets/images/` folder)

### Step 3: Write Your Content

After the closing `---` of the front matter, write your blog post content using Markdown formatting.

**Complete Example:**

```markdown
---
layout: post
title: "Top 3 Tips for First-Time Home Buyers"
author: admin
categories: [ Tips, Buyers ]
image: assets/images/home-buyers-guide.jpg
---

Buying your first home is an exciting journey! Here are three essential tips to help you succeed.

## 1. Get Pre-Approved for a Mortgage

Before you start house hunting, get pre-approved for a mortgage. This shows sellers you're serious.

## 2. Work with a Real Estate Agent

A good agent knows the market and can guide you through the process.

## 3. Don't Skip the Home Inspection

Always get a professional inspection to avoid costly surprises later.

![Happy family]({{ site.baseurl }}/assets/images/happy-family.jpg)

Ready to start your home buying journey? Contact us today!
```

---

## 🖼️ How to Upload and Use Images

### Step 1: Add Your Image

1. Get your image file (JPEG, PNG, or GIF)
2. Go to the `assets/images/` folder in your repository
3. Upload your image file there

**Tips:**
- Use descriptive file names: `beach-house-sunset.jpg` instead of `IMG_1234.jpg`
- Keep file names lowercase with dashes between words
- Recommended image size: 800-1200px wide for featured images

### Step 2: Reference the Image in Your Post

There are two ways to use images in your posts:

**Method 1: As a Featured Image (appears at the top)**
```markdown
---
image: assets/images/your-image-name.jpg
---
```

**Method 2: Inside Your Post Content**
```markdown
![Description of image]({{ site.baseurl }}/assets/images/your-image-name.jpg)
```

**Complete Example:**
```markdown
---
layout: post
title: "Beautiful Beachfront Property"
author: admin
categories: [ Listings ]
image: assets/images/beach-house-main.jpg
---

This stunning beachfront property offers breathtaking ocean views.

## Interior Photos

![Spacious living room]({{ site.baseurl }}/assets/images/beach-house-living.jpg)

The living room features floor-to-ceiling windows.

![Modern kitchen]({{ site.baseurl }}/assets/images/beach-house-kitchen.jpg)

The kitchen is equipped with top-of-the-line appliances.
```

---

## ✏️ How to Edit an Existing Post

1. Go to the `_posts/` folder
2. Find the file you want to edit (look at the date and title in the filename)
3. Open the file
4. Make your changes
5. Save the file

**Example:**
- Want to edit the post about "Powerful things you can do with the Markdown editor"?
- Look for: `2020-01-12-powerful-things-markdown-editor.md`
- Open it, make changes, and save

---

## 📝 Markdown Formatting Guide

Markdown is a simple way to format text. Here are the most common formatting options:

### Headings
```markdown
# Heading 1 (Largest)
## Heading 2
### Heading 3
#### Heading 4
```

### Text Formatting
```markdown
**Bold text**
*Italic text*
~~Strikethrough text~~
```

**Result:**
- **Bold text**
- *Italic text*
- ~~Strikethrough text~~

### Lists

**Bullet List:**
```markdown
- First item
- Second item
- Third item
```

**Numbered List:**
```markdown
1. First step
2. Second step
3. Third step
```

### Links

```markdown
[Link text here](https://www.example.com)
```

**Example:**
```markdown
[Visit our contact page](https://hyenarealty.com/contact)
```

### Quotes
```markdown
> This is a quote or testimonial
```

**Result:**
> This is a quote or testimonial

### Code or Special Text
```markdown
Use `backticks` for inline code or special formatting
```

---

## 📋 Common Tasks

### Task 1: Publish a New Property Listing

**Filename:** `2026-02-04-downtown-home-listing.md`

```markdown
---
layout: post
title: "Stunning 3-Bedroom Home in Downtown"
author: admin
categories: [ Listings, Downtown ]
image: assets/images/downtown-home-exterior.jpg
---

**Price:** $450,000  
**Bedrooms:** 3  
**Bathrooms:** 2  
**Square Feet:** 2,100

This beautifully renovated home is located in the heart of downtown.

## Key Features

- Updated kitchen with granite countertops
- Hardwood floors throughout
- Large backyard with patio
- Two-car garage

## Photos

![Kitchen]({{ site.baseurl }}/assets/images/downtown-home-kitchen.jpg)

![Master bedroom]({{ site.baseurl }}/assets/images/downtown-home-bedroom.jpg)

**Interested?** Contact us today to schedule a viewing!
```

### Task 2: Post a Blog Article with Tips

**Filename:** `2026-02-04-home-staging-tips.md`

```markdown
---
layout: post
title: "How to Stage Your Home for a Quick Sale"
author: admin
categories: [ Tips, Sellers ]
image: assets/images/home-staging.jpg
---

Selling your home? Here's how to make it irresistible to buyers.

## 1. Declutter Every Room

Remove personal items and excess furniture to make spaces look larger.

## 2. Deep Clean Everything

A spotless home shows that it's been well-maintained.

## 3. Add Fresh Flowers or Plants

Greenery brings life and color to any space.

## 4. Fix Minor Repairs

Replace burnt-out bulbs, fix leaky faucets, and patch wall holes.

## Before and After

![Before staging]({{ site.baseurl }}/assets/images/before-staging.jpg)

![After staging]({{ site.baseurl }}/assets/images/after-staging.jpg)

Need help staging your home? We're here to help!
```

### Task 3: Announce an Event or Open House

**Filename:** `2026-02-04-open-house-oak-street.md` (use today's date to publish immediately)

```markdown
---
layout: post
title: "Open House This Sunday - 123 Oak Street"
author: admin
categories: [ Events, Open House ]
image: assets/images/oak-street-home.jpg
---

Join us this **Sunday, February 9th from 2:00 PM to 4:00 PM** for an open house!

**Address:** 123 Oak Street, Springfield

This charming colonial features:
- 4 bedrooms
- 2.5 bathrooms
- Updated kitchen
- Beautiful landscaped yard

![Front view]({{ site.baseurl }}/assets/images/oak-street-front.jpg)

We look forward to seeing you there!
```

---

## 🔍 Troubleshooting

### My post doesn't appear on the website

**Check these things:**
1. ✅ Is the filename in the correct format? `YYYY-MM-DD-title.md`
2. ✅ Is the file in the `_posts/` folder?
3. ✅ Does the front matter have opening and closing `---` lines?
4. ✅ Is the date in the filename today or in the past? (Future-dated posts won't show)

### My image doesn't show up

**Check these things:**
1. ✅ Is the image uploaded to `assets/images/` folder?
2. ✅ Is the path correct? Should be: `assets/images/filename.jpg`
3. ✅ Is the filename spelled exactly the same in your post and in the folder?
4. ✅ Did you include the `{{ site.baseurl }}/` part for images in content?

### Formatting looks weird

**Common fixes:**
1. ✅ Make sure there's a blank line before and after headings
2. ✅ Make sure there's a blank line before and after lists
3. ✅ Check that you closed all formatting (e.g., `**bold**` needs two asterisks on each side)
4. ✅ Ensure the front matter is at the very top of the file

---

## 📚 Quick Tips

### Do's ✅
- Always use the date format YYYY-MM-DD in filenames
- Keep image files reasonably sized (under 2MB when possible)
- Use descriptive titles and filenames
- Preview your post after publishing to make sure it looks right
- Save images with descriptive names
- Use headings to organize your content

### Don'ts ❌
- Don't use spaces in filenames (use dashes instead)
- Don't forget the `.md` extension on post files
- Don't skip the front matter section
- Don't use special characters in filenames (stick to letters, numbers, and dashes)
- Don't upload extremely large images (they slow down the website)

---

## 🎯 Checklist for Publishing a New Post

Use this checklist every time you publish a new post:

- [ ] Created file in `_posts/` folder
- [ ] Named file as `YYYY-MM-DD-title.md`
- [ ] Added front matter with `---` at start and end
- [ ] Set title, author, and categories
- [ ] Uploaded featured image to `assets/images/`
- [ ] Referenced image correctly in front matter
- [ ] Wrote post content in Markdown
- [ ] Added any additional images to `assets/images/`
- [ ] Previewed post on website
- [ ] Checked that all images display correctly
- [ ] Verified all links work

---

## 📞 Need Help?

If you get stuck or have questions:

1. **Review this guide** - Most common questions are answered here
2. **Check existing posts** - Look at files in `_posts/` folder for examples
3. **Test small changes** - Make one change at a time to see what works
4. **Take notes** - Write down what works for you for next time

---

## 🎓 Learning Resources

Want to learn more about Markdown?
- [Markdown Guide](https://www.markdownguide.org/basic-syntax/)
- [Markdown Cheat Sheet](https://www.markdownguide.org/cheat-sheet/)

---

**Remember:** It's okay to make mistakes! You can always edit or delete posts. Start with small changes and build your confidence. You've got this! 🎉
