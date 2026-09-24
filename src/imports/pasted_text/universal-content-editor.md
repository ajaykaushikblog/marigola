PHASE 14 — CREATE THE ADVANCED UNIVERSAL CONTENT EDITOR

Keep the entire existing project intact.

DO NOT redesign the public website.

DO NOT remove or break:

- Homepage
- Universal Category Pages
- Article Pages
- Recipe Pages
- DIY Pages
- Author Pages
- Search
- CMS Dashboard
- SEO Control Center
- Media Library
- Advertisement System
- Pinterest System
- Social Sharing
- Responsive layouts
- Existing routes
- Existing components
- Existing data structures

This phase creates the main professional editorial content editor for the CMS.

The editor must be capable of creating thousands of high-quality lifestyle articles without requiring developers.

==================================================
1. UNIVERSAL CONTENT EDITOR
==================================================

Create:

/admin/content/new/article

and:

/admin/content/:id/edit

The same editor architecture should eventually support:

- Articles
- Listicles
- Guides
- Product Guides
- Future content types

Use a reusable block-based content editor.

==================================================
2. EDITOR LAYOUT
==================================================

Desktop:

Left/main:
- Content editor

Right:
- Publishing
- Taxonomy
- SEO
- Pinterest
- Social
- Featured image

Top:
- Back
- Save Draft
- Preview
- Publish

Mobile/tablet:

- Single-column editor
- Collapsible settings sections
- Sticky save/publish controls where appropriate

Do not create excessive sticky UI.

==================================================
3. BASIC CONTENT INFORMATION
==================================================

Fields:

- Title
- Slug
- Excerpt
- Featured image
- Author
- Content type
- Publish status
- Publish date
- Updated date

Show:

- Word count
- Estimated reading time
- Last saved time

Create autosave status:

Saving...
Saved
Unsaved changes

These are UI states for the future backend.

==================================================
4. TITLE / SLUG EDITOR
==================================================

Title field:

- Large editorial title input
- Character/length guidance
- Preview

Slug:

- Auto-generated from title conceptually
- Editable
- URL preview

Example:

Title:
25 Elegant Christmas Nail Ideas

Slug:
/christmas/christmas-nail-ideas/

Do not force a specific slug structure for every content type.

==================================================
5. RICH CONTENT BLOCK EDITOR
==================================================

Create a reusable block system.

Available blocks:

- Paragraph
- Heading
- Subheading
- Image
- Gallery
- Video
- Quote
- Ordered List
- Unordered List
- Checklist
- Table
- Callout
- Divider
- Button
- Embed
- Product Card
- Affiliate Product
- Sponsored Content
- Advertisement
- Newsletter
- Recipe
- Related Content
- Author Box
- Pinterest Image

Each block should have:

- Drag/reorder
- Duplicate
- Edit
- Delete
- Preview

==================================================
6. ADD BLOCK MENU
==================================================

Create a professional "Add Block" interface.

Categories:

TEXT
- Paragraph
- Heading
- Quote
- List
- Checklist

MEDIA
- Image
- Gallery
- Video

EDITORIAL
- Callout
- Table
- Divider
- Button

MONETIZATION
- Affiliate Product
- Advertisement
- Sponsored Content

CONTENT
- Recipe
- Related Content
- Author Box

SOCIAL
- Pinterest Image
- Social Share

Do not create hundreds of unnecessary blocks.

==================================================
7. TEXT EDITOR
==================================================

Create rich text controls:

- Bold
- Italic
- Link
- Unordered list
- Ordered list
- Heading
- Quote
- Alignment where appropriate

Allow links to:

- Internal content
- External websites
- Affiliate destinations

Show link editing UI.

==================================================
8. INTERNAL LINKING
==================================================

When inserting a link, provide:

Search existing content.

Search by:

- Title
- Category
- Occasion
- Tag

Show results with:

- Title
- Content type
- URL

Allow:

Insert Link

This should connect conceptually to the Phase 12 internal linking system.

==================================================
9. IMAGE BLOCK
==================================================

When adding an image:

Open the Media Library picker.

Allow:

- Select existing
- Upload
- Edit metadata

Image settings:

- Alt text
- Caption
- Alignment
- Size
- Link
- Optional Pinterest Save action

Show desktop/mobile preview.

==================================================
10. GALLERY BLOCK
==================================================

Allow:

- Select multiple images
- Reorder
- Remove
- Set cover image
- Captions

Gallery layouts:

- Grid
- Masonry-style concept
- Carousel where appropriate

Keep the public implementation lightweight.

==================================================
11. VIDEO BLOCK
==================================================

Create a video block supporting future:

- Video URL
- Poster image
- Caption
- Accessibility text

Do not autoplay videos by default.

Do not add unnecessary background video.

==================================================
12. CALLOUT BLOCK
==================================================

Create reusable callout styles:

Tip
Note
Important
Recipe Tip
DIY Tip
Editor's Note

Allow:

- Title
- Content
- Optional icon

Keep styling consistent with the existing design system.

==================================================
13. TABLE BLOCK
==================================================

Create a responsive table editor.

Support:

- Rows
- Columns
- Header row
- Cell editing

On mobile:

Allow horizontal scrolling within the table container when genuinely necessary.

Do not create horizontal scrolling for the entire page.

==================================================
14. PRODUCT / AFFILIATE BLOCK
==================================================

Connect to the existing monetization architecture.

Fields:

- Product image
- Product name
- Description
- Price
- Merchant
- Affiliate URL
- CTA
- Disclosure

Allow selecting products from a future:

Affiliate Product Library.

Do not hard-code Amazon specifically into the component.

==================================================
15. ADVERTISEMENT BLOCK
==================================================

Allow editors to insert an advertisement placeholder.

Fields:

- Ad slot
- Placement
- Desktop/mobile behavior

Use the existing Phase 8 AdSlot system.

Editors should select a configured ad slot rather than manually entering arbitrary ad code.

==================================================
16. SPONSORED CONTENT BLOCK
==================================================

Allow:

- Brand
- Logo
- Image
- Title
- Description
- CTA
- Destination URL
- Sponsored disclosure

Clearly label sponsored content.

==================================================
17. NEWSLETTER BLOCK
==================================================

Allow insertion of the existing newsletter component.

Options:

- Default newsletter
- Custom heading
- Custom description
- CTA text

Do not create a separate newsletter design for every article.

==================================================
18. RELATED CONTENT BLOCK
==================================================

Allow:

- Automatic related content
- Manual related content

Automatic mode should conceptually use:

- Same subcategory
- Same category
- Same occasion
- Same season
- Shared tags
- Same content type

Manual mode:

Editor searches and selects content.

This connects to the existing related-content system.

==================================================
19. PINTEREST BLOCK
==================================================

Allow editors to insert Pinterest-friendly visual content.

Fields:

- Pinterest image
- Pinterest title
- Pinterest description
- Destination URL

Connect to the existing Phase 9 Pinterest system.

==================================================
20. CONTENT OUTLINE / TABLE OF CONTENTS
==================================================

Create an automatic TOC concept.

Extract:

H2
H3

Show preview:

Table of Contents

Allow:

- Enable
- Disable
- Position

Do not require manual TOC creation for every article.

==================================================
21. ARTICLE SETTINGS
==================================================

Right sidebar sections:

CONTENT
TAXONOMY
FEATURED IMAGE
SEO
PINTEREST
SOCIAL
PUBLISHING

Keep these sections collapsible.

==================================================
22. TAXONOMY PANEL
==================================================

Fields:

Category
Subcategory
Occasion
Season
Tags
Styles
Colors
Audience

Allow multiple selections where appropriate.

Example:

Category:
Beauty

Subcategory:
Nails

Occasion:
Christmas

Season:
Winter

Style:
Elegant

Audience:
Women

Do not limit content to one taxonomy.

==================================================
23. FEATURED IMAGE PANEL
==================================================

Connect directly to the Phase 13 Media Library.

Allow:

- Select image
- Upload
- Replace
- Remove

Show:

Desktop preview
Mobile preview
Social preview
Pinterest preview

==================================================
24. SEO PANEL
==================================================

Connect to Phase 12.

Fields:

- SEO title
- Meta description
- Canonical
- Index/noindex
- Follow/nofollow
- Sitemap inclusion
- Schema type

Show:

SEO preview
Validation states

Do not create fake ranking scores.

==================================================
25. PINTEREST PANEL
==================================================

Fields:

- Pinterest title
- Pinterest description
- Primary Pinterest image
- Pin template
- Alternate pins
- Enable Save button

Show live visual preview.

==================================================
26. SOCIAL PANEL
==================================================

Fields:

- Social title
- Social description
- Open Graph image
- X/Twitter image

Show social preview.

==================================================
27. PUBLISHING PANEL
==================================================

Fields:

Status:

Draft
Review
Scheduled
Published
Unpublished

Actions:

Save Draft
Preview
Submit for Review
Schedule
Publish

Scheduling UI:

Date
Time
Timezone

Show confirmation before publishing.

==================================================
28. CONTENT PREVIEW
==================================================

Create a preview mode using the existing public article template.

Preview:

Desktop
Tablet
Mobile

The preview must reflect:

- Content blocks
- Images
- Ads
- Affiliate blocks
- Related content
- Author
- SEO/Pinterest settings where visually applicable

Do not create a completely separate article design.

Use the same public template.

==================================================
29. REVISION HISTORY
==================================================

Create:

Revision History

Show:

- Version
- Author/editor
- Date/time
- Changes

Actions:

View
Compare
Restore

This is a future backend UI.

Do not claim real version history exists unless connected to a backend.

==================================================
30. CONTENT VALIDATION
==================================================

Before publishing, create a pre-publish checklist.

Check:

- Title exists
- Slug exists
- Author selected
- Featured image exists
- Category selected
- Content exists
- SEO title
- Meta description
- Canonical
- Alt text
- Pinterest image
- Required taxonomy

Show:

Ready to Publish
Needs Attention

Do not prevent publishing for optional fields unless configured as required.

==================================================
31. UNSAVED CHANGES
==================================================

Create warning UI if the editor contains unsaved changes.

Options:

Save Changes
Discard
Cancel

Do not silently lose content.

==================================================
32. DUPLICATE ARTICLE
==================================================

Add:

Duplicate

When duplicated:

- New draft
- New editable slug
- Existing content blocks copied
- SEO canonical cleared/updated
- Pinterest metadata copied but editable
- Publishing status reset to Draft

==================================================
33. RESPONSIVE EDITOR
==================================================

Test:

320px
375px
390px
414px
768px
834px
1024px
1280px
1440px

Mobile editor:

- Full-width inputs
- Collapsible settings
- Touch-friendly controls
- Block controls remain accessible
- No accidental horizontal overflow

==================================================
34. ACCESSIBILITY
==================================================

Support:

- Keyboard navigation
- Focus states
- Accessible labels
- Semantic buttons
- Screen-reader-friendly controls
- Accessible dialogs
- Accessible image selection
- Accessible drag/reorder alternatives

Do not make drag-and-drop the only way to reorder blocks.

Provide alternative controls:

Move Up
Move Down

==================================================
35. PERFORMANCE
==================================================

The editor should be designed for long articles.

Avoid rendering unnecessary heavy components.

Use:

- Lazy media previews
- Lightweight block previews
- Efficient lists
- Pagination where appropriate

==================================================
36. DATA MODEL
==================================================

Create a reusable conceptual structure:

ContentItem
{
  id,
  type,
  title,
  slug,
  excerpt,
  blocks[],
  featuredImage,
  author,
  taxonomy,
  publishing,
  seo,
  pinterest,
  social,
  relatedContent[]
}

Block:

{
  id,
  type,
  data,
  order
}

Do not hard-code article-specific fields into individual page components.

==================================================
37. UNIVERSAL CONTENT SUPPORT
==================================================

The editor architecture must eventually support:

Articles
Recipes
DIY
Listicles
Guides
Product Guides

Specialized editors can extend this universal editor later.

Do not create an architecture that only works for blog articles.

==================================================
38. DO NOT BREAK EXISTING SYSTEMS
==================================================

Preserve:

- Public website
- Homepage
- Category pages
- Article pages
- Recipe pages
- DIY pages
- Author pages
- Search
- CMS dashboard
- SEO
- Media Library
- Ads
- Pinterest
- Social
- Responsive system
- Existing routes

Add the Advanced Content Editor alongside these systems.

==================================================
FINAL GOAL
==================================================

Create a professional, scalable, block-based editorial CMS editor capable of producing thousands of rich lifestyle articles.

An editor should be able to create a complete article without touching code.

The editor must connect conceptually to:

Media
Authors
Taxonomy
SEO
Pinterest
Social
Advertisements
Affiliate Products
Sponsored Content
Related Content
Publishing

The public website should render the same content through the existing universal templates.

Build the UI, reusable components and data architecture now.

Real database persistence, authentication, file storage, autosave, revision storage, scheduling, publishing and external API integrations will be connected during production/backend implementation.

Run type checking/build validation after implementation.