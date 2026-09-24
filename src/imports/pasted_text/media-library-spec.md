PHASE 13 — CREATE THE ADVANCED MEDIA LIBRARY & IMAGE MANAGEMENT SYSTEM

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
- Advertisement System
- Pinterest System
- Social Sharing
- Responsive layouts
- Existing routes
- Existing data structures

Build a professional, scalable Media Library for the Universal Lifestyle CMS.

The website is highly image-focused and Pinterest-first, so media management must be designed to handle thousands of images efficiently.

This is a front-end/UI and architecture prototype for the future production backend.

==================================================
1. MEDIA LIBRARY
==================================================

Create:

/admin/media

Build a professional media management interface.

Support two viewing modes:

- Grid
- List

Grid view should show:

- Thumbnail
- Filename
- Image type
- Dimensions
- Usage count
- Upload date

List view should show:

- File
- Type
- Dimensions
- Size
- Used in
- Uploaded
- Modified
- Status
- Actions

==================================================
2. MEDIA SEARCH
==================================================

Create a powerful media search.

Search by:

- Filename
- Title
- Alt text
- Caption
- Description
- Tags
- Content usage

Add filters:

- Image
- Video
- PDF
- Document
- Pinterest asset
- Unused
- Used
- Recently uploaded

Include sorting:

- Newest
- Oldest
- Name
- File size
- Dimensions
- Most used
- Least used

==================================================
3. MEDIA UPLOAD
==================================================

Create a reusable upload interface.

Support:

- Drag and drop
- Browse files
- Multiple upload
- Upload progress
- Success state
- Error state
- Cancel upload

Create an upload queue.

Each item should show:

- Filename
- Thumbnail
- Progress
- Status
- Error message where applicable

Do not implement fake backend uploads.

This is a production-ready UI concept for future storage integration.

==================================================
4. MEDIA DETAILS PANEL
==================================================

When an image is selected, open a detailed media panel.

Show:

- Large preview
- Filename
- File type
- File size
- Width
- Height
- Aspect ratio
- Uploaded date
- Modified date
- URL

Editable fields:

- Title
- Alt text
- Caption
- Description
- Filename
- Media tags

Add:

Save Changes
Replace Image
Delete

==================================================
5. ALT TEXT MANAGEMENT
==================================================

Make accessibility and image SEO first-class features.

Each image should have:

- Alt text
- Decorative image toggle

Show validation:

- Missing alt text
- Very short alt text
- Good descriptive alt text

Do not force alt text on genuinely decorative images.

Provide an editor-friendly explanation:

Alt text should describe the meaningful visual content and purpose of the image.

==================================================
6. IMAGE SEO
==================================================

Add image SEO fields:

- SEO-friendly filename
- Alt text
- Image title
- Caption
- Description

Show:

Image SEO status

Checks:

- Filename
- Alt text
- Dimensions
- File format
- File size

Connect these fields conceptually to the existing Phase 12 SEO system.

==================================================
7. IMAGE DIMENSIONS
==================================================

Display:

Width
Height
Aspect ratio

Detect common formats:

1:1
4:3
16:9
2:3
3:2

Highlight Pinterest format:

1000 × 1500
2:3

Clearly distinguish Pinterest assets from normal editorial images.

==================================================
8. PINTEREST MEDIA MANAGEMENT
==================================================

Create a dedicated media filter:

Pinterest Assets

Allow editors to identify:

- Standard images
- Pinterest images
- Alternate Pinterest pins

For Pinterest assets show:

- Pin title
- Pin description
- Template
- Dimensions
- Destination content

Support:

Create Pinterest Asset
Edit Pinterest Asset
Duplicate Pinterest Asset
Set as Primary Pin

Connect this to the existing Phase 9 Pinterest system.

==================================================
9. IMAGE VARIANTS
==================================================

Create a future-ready concept for image variants.

For an original image, show:

Original
Thumbnail
Small
Medium
Large
Mobile
Pinterest
Social

Example:

Original:
3000 × 4500

Pinterest:
1000 × 1500

Mobile:
768 × 1152

Do not actually generate files unless the existing environment supports it.

Represent the architecture and UI only.

==================================================
10. RESPONSIVE IMAGE MANAGEMENT
==================================================

Create a responsive image configuration UI.

Support conceptual fields:

- Source image
- Desktop image
- Tablet image
- Mobile image
- Retina image

Show how the future CMS could select appropriate images.

The public website should remain capable of using responsive image sources.

==================================================
11. IMAGE COMPRESSION
==================================================

Create a future image optimization section.

Show:

Original size
Optimized size
Estimated savings
Format

Support future formats:

- WebP
- AVIF
- JPEG
- PNG

Use UI states such as:

Optimized
Needs Optimization
Processing

Do not claim actual compression has occurred in this prototype.

==================================================
12. IMAGE USAGE TRACKING
==================================================

For every media item show:

"Used in"

Example:

Used in:
- 3 Articles
- 1 Recipe
- 2 Pinterest Pins
- 1 Category

Allow clicking a usage item to open the corresponding content.

Create:

View Usage

This is important so editors do not accidentally delete images still being used.

==================================================
13. UNUSED MEDIA
==================================================

Create:

/admin/media/unused

Show media files that are not currently referenced by content.

Columns/cards:

- Image
- Filename
- Uploaded
- Size
- Dimensions
- Last used
- Status

Actions:

Review
Delete
Keep

Do not automatically delete unused media.

==================================================
14. DUPLICATE MEDIA DETECTION
==================================================

Create a future-ready duplicate detection interface.

Show:

Possible duplicates

For each group:

- Images
- Dimensions
- File sizes
- Upload dates

Actions:

Compare
Keep
Delete Duplicate

Do not claim two images are duplicates unless connected to a real duplicate detection system.

Use placeholder/example states.

==================================================
15. MEDIA TAGGING
==================================================

Allow editors to add media tags.

Examples:

Christmas
Halloween
Wedding
Recipe
Nails
DIY
Home Decor
Food
Pinterest
Hero Image
Product

Tags should be reusable and searchable.

Do not create separate media databases for each category.

==================================================
16. MEDIA COLLECTIONS
==================================================

Create optional collections.

Examples:

Christmas 2026
Halloween Campaign
Wedding Inspiration
Pinterest Assets
Recipe Photography
Homepage Images

A media item can belong to multiple collections.

Collections are organizational tools and should not automatically become public URLs.

==================================================
17. MEDIA BULK ACTIONS
==================================================

Allow selecting multiple media items.

Bulk actions:

- Add tags
- Remove tags
- Move to collection
- Update metadata
- Optimize
- Delete

For destructive actions:

Show confirmation.

==================================================
18. MEDIA REPLACEMENT
==================================================

Create a "Replace Media" workflow.

When replacing an image:

- Keep existing media references where technically possible
- Show current image
- Show replacement image
- Confirm replacement
- Warn about affected content

Do not silently break existing image URLs.

==================================================
19. MEDIA DELETE SAFETY
==================================================

Before deletion show:

Image is used in X locations.

List affected content.

Options:

Cancel
Delete Anyway

If the image is heavily used, show a stronger warning.

The UI should encourage editors to replace/remove references before deleting.

==================================================
20. GALLERY MANAGEMENT
==================================================

Create a reusable gallery editor.

Support:

- Add images
- Remove images
- Reorder images
- Set cover image
- Add captions
- Edit alt text
- Preview gallery

Gallery should support:

Articles
Recipes
DIY
Guides
Product Guides

==================================================
21. ARTICLE IMAGE SELECTOR
==================================================

Create a reusable media picker.

When an editor selects:

"Insert Image"

open:

Media Library

Allow:

Search
Filter
Select
Upload
Edit metadata

Then:

Insert Image

The same media picker should work across:

Article editor
Recipe editor
DIY editor
Category editor
Homepage editor

==================================================
22. FEATURED IMAGE SELECTOR
==================================================

Create a reusable featured image selector.

Support:

- Select existing image
- Upload new image
- Crop/preview
- Replace
- Remove

Show preview for:

Desktop
Mobile
Social
Pinterest

==================================================
23. CROPPING / FOCAL POINT
==================================================

Create a future-ready image editing interface.

Support conceptual controls:

- Crop
- Aspect ratio
- Focal point
- Position
- Rotation

Preserve original image.

Create presets:

1:1
4:3
16:9
2:3
3:2

Pinterest:

2:3

Do not permanently destroy the original image.

==================================================
24. MEDIA INFORMATION FOR SEO
==================================================

Connect media to the existing SEO system.

Show:

- Alt text status
- Filename status
- Image dimensions
- Optimization status
- Usage
- Pinterest status

Create an overall:

Image SEO Health

This should be an interface indicator, not a guaranteed ranking score.

==================================================
25. MEDIA IMPORT / EXPORT
==================================================

Create a future UI for:

Import Media
Export Media

Support conceptual formats:

CSV
JSON

Show:

- Import progress
- Success
- Warnings
- Errors

Do not implement fake backend processing.

==================================================
26. MEDIA STORAGE SETTINGS
==================================================

Create:

/admin/media/settings

Future configuration sections:

Storage
Image Processing
CDN
Compression
Responsive Images
Pinterest Assets
Upload Limits

Possible future storage:

Local
Object Storage
CDN

Do not assume a specific provider.

==================================================
27. MEDIA LIBRARY DASHBOARD
==================================================

Create summary cards:

- Total Media
- Images
- Videos
- Documents
- Pinterest Assets
- Unused Media
- Needs Optimization
- Missing Alt Text

Again, these are UI/dashboard fields until connected to real data.

==================================================
28. MEDIA ACTIVITY
==================================================

Create media activity history.

Show:

- Uploaded
- Edited
- Replaced
- Deleted
- Used in content
- Metadata changed

Fields:

User
Action
Media
Date/time

==================================================
29. RESPONSIVE ADMIN EXPERIENCE
==================================================

Test the Media Library at:

320px
375px
390px
414px
768px
834px
1024px
1280px
1440px

Mobile:

- Grid becomes appropriate number of columns
- Detail panel becomes full-screen or bottom sheet
- Upload interface remains usable
- Filters become collapsible
- Tables become responsive
- Touch controls remain accessible

Avoid accidental horizontal page scrolling.

==================================================
30. PERFORMANCE
==================================================

Design the system for thousands of media files.

Use:

- Pagination
- Lazy-loaded thumbnails
- Lightweight previews
- Search/filter controls
- Virtualized lists conceptually where appropriate

Do not attempt to render thousands of full-resolution images at once.

==================================================
31. ACCESSIBILITY
==================================================

Media management must support:

- Keyboard navigation
- Focus states
- Accessible labels
- Screen reader descriptions
- Clear upload status
- Accessible dialogs
- Accessible confirmation dialogs

==================================================
32. DO NOT BREAK EXISTING SYSTEMS
==================================================

Preserve all existing:

- Public website
- CMS Dashboard
- SEO Control Center
- Pinterest system
- Ads
- Social sharing
- Content editors
- Authors
- Search
- Responsive system
- Routes
- Components

Add this Media Library as a reusable CMS module.

==================================================
FINAL GOAL
==================================================

Create a professional media management system capable of supporting a large image-heavy lifestyle website with thousands of articles and Pinterest assets.

The Media Library should become the central source for:

- Editorial images
- Recipe images
- DIY images
- Author images
- Product images
- Pinterest images
- Social images
- Gallery images

The system must be scalable, searchable, SEO-friendly, Pinterest-friendly, responsive and safe for large-scale content management.

Build the reusable UI, components and data architecture now.

Actual file storage, image processing, CDN, image transformation and database integrations will be connected during production/backend implementation.

Run type checking/build validation after implementation.