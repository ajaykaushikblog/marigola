PHASE 15 — CREATE SPECIALIZED RECIPE + DIY CMS EDITORS

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
- Advanced Universal Content Editor
- Advertisement System
- Pinterest System
- Social Sharing
- Responsive layouts
- Existing routes
- Existing components
- Existing data structures

This phase creates specialized CMS editors for Recipes and DIY/Tutorials.

The specialized editors must extend the Universal Content Editor created in Phase 14 rather than becoming separate disconnected systems.

==================================================
1. SPECIALIZED CONTENT ARCHITECTURE
==================================================

Create two specialized editors:

/admin/content/new/recipe

/admin/content/new/diy

And edit routes:

/admin/content/:id/edit/recipe

/admin/content/:id/edit/diy

Both editors must inherit common functionality from the Universal Content Editor:

- Title
- Slug
- Excerpt
- Featured image
- Author
- Taxonomy
- Content blocks
- SEO
- Pinterest
- Social
- Publishing
- Preview
- Media
- Related content
- Monetization

Then add specialized fields.

==================================================
2. RECIPE CMS EDITOR
==================================================

Create a professional Recipe Editor.

Desktop layout:

Main editor
+
Recipe settings sidebar

Top actions:

- Save Draft
- Preview
- Schedule
- Publish

Recipe-specific sections:

- Recipe Information
- Timing
- Servings
- Ingredients
- Instructions
- Equipment
- Nutrition
- Notes
- Tips
- Gallery
- Affiliate Products
- Recipe SEO

==================================================
3. RECIPE BASIC INFORMATION
==================================================

Fields:

- Recipe name
- Short description
- Featured image
- Author
- Recipe category
- Cuisine
- Course
- Difficulty
- Keywords/tags

Examples:

Cuisine:
Italian

Course:
Dinner

Difficulty:
Easy

Keep these fields configurable rather than hard-coded.

==================================================
4. RECIPE TIMING
==================================================

Fields:

- Prep time
- Cook time
- Total time

Use a clear time input interface.

Support:

Minutes
Hours + minutes

Automatically calculate total time conceptually when appropriate.

Allow manual override.

==================================================
5. SERVINGS
==================================================

Create:

Servings

Allow:

- Default servings
- Minimum
- Maximum

Create a serving adjustment UI.

Example:

Servings:
4

[-] 4 [+]

The future public recipe page can use this value to scale ingredient quantities.

==================================================
6. INGREDIENT BUILDER
==================================================

Create a structured ingredient editor.

Each ingredient row:

- Quantity
- Unit
- Ingredient name
- Optional preparation note
- Optional group

Example:

1
cup
all-purpose flour
sifted

Allow:

- Add ingredient
- Delete ingredient
- Reorder
- Duplicate

==================================================
7. INGREDIENT GROUPS
==================================================

Allow grouped ingredients.

Examples:

For the Dough
For the Filling
For the Sauce
For the Topping

Each group can contain multiple ingredients.

Allow:

- Add group
- Rename group
- Reorder group
- Delete group

Do not require every recipe to use groups.

==================================================
8. INSTRUCTIONS BUILDER
==================================================

Create structured recipe instructions.

Each step:

- Step number
- Instruction text
- Optional image
- Optional timing
- Optional tip

Actions:

- Add step
- Delete step
- Reorder
- Duplicate

Support optional step images from the Media Library.

==================================================
9. EQUIPMENT
==================================================

Create structured equipment list.

Fields:

- Equipment name
- Optional quantity
- Optional affiliate product

Examples:

Stand mixer
9-inch cake pan
Dutch oven

Allow:

- Add
- Delete
- Reorder

==================================================
10. NUTRITION
==================================================

Create optional nutrition fields:

- Calories
- Protein
- Carbohydrates
- Fat
- Fiber
- Sugar
- Sodium

Allow:

- Per serving
- Per recipe

Clearly indicate when nutrition data is not available.

Do not generate fake nutrition values.

==================================================
11. RECIPE NOTES
==================================================

Create:

Recipe Notes

Allow rich text.

Examples:

- Storage
- Make ahead
- Substitutions
- Serving suggestions

==================================================
12. RECIPE TIPS
==================================================

Create a reusable Tips section.

Allow multiple tips.

Each tip:

- Title
- Description

Actions:

Add
Edit
Delete
Reorder

==================================================
13. RECIPE GALLERY
==================================================

Connect to Phase 13 Media Library.

Allow:

- Multiple images
- Reorder
- Captions
- Alt text
- Set primary image

Preview:

- Desktop
- Mobile

==================================================
14. RECIPE AFFILIATE PRODUCTS
==================================================

Connect to the existing Phase 8 monetization system.

Allow editors to associate products such as:

- Cookware
- Kitchen tools
- Appliances
- Ingredients/products where appropriate

Fields:

- Product
- Image
- Price
- Merchant
- Affiliate URL
- CTA
- Disclosure

Do not hard-code one affiliate provider.

==================================================
15. RECIPE SEO
==================================================

Connect to Phase 12 SEO.

Fields:

- SEO title
- Meta description
- Canonical
- Index/noindex
- Sitemap inclusion

Recipe structured data preview must include appropriate fields:

- Name
- Image
- Author
- Description
- Prep time
- Cook time
- Total time
- Recipe yield
- Ingredients
- Instructions
- Nutrition when available

Rating/review fields must only appear when genuine rating/review data exists.

Do not create fake ratings.

==================================================
16. RECIPE PINTEREST
==================================================

Connect to Phase 9 Pinterest.

Fields:

- Pinterest title
- Pinterest description
- Primary Pinterest image
- Pin template
- Alternate pins

Create Pinterest preview.

Support multiple pins per recipe.

==================================================
17. RECIPE PREVIEW
==================================================

Use the existing Universal Recipe Page.

Preview modes:

Desktop
Tablet
Mobile

Preview must reflect:

- Recipe title
- Image
- Timing
- Servings
- Ingredients
- Instructions
- Nutrition
- Tips
- Notes
- Affiliate products
- Ads
- Related recipes
- Author

Do not create a separate visual design disconnected from the public Recipe Page.

==================================================
18. RECIPE PRINT PREVIEW
==================================================

Create a print-preview concept.

Show a clean printable recipe layout:

- Recipe title
- Image
- Description
- Ingredients
- Instructions
- Timing
- Servings
- Notes

Do not include unnecessary navigation or advertisements in the printable recipe.

==================================================
19. RECIPE PDF PREVIEW
==================================================

Create a future PDF/download configuration.

Fields:

- Enable PDF download
- PDF title
- Cover image
- Include nutrition
- Include notes
- Include author

Show PDF preview.

Actual PDF generation will be connected later.

==================================================
20. DIY CMS EDITOR
==================================================

Create:

/admin/content/new/diy

Build a specialized DIY/Tutorial editor using the Universal Content Editor.

DIY-specific sections:

- Project Information
- Difficulty
- Time
- Cost
- Materials
- Tools
- Steps
- Step Images
- Tips
- Variations
- Gallery
- Affiliate Products
- DIY SEO
- Pinterest

==================================================
21. DIY PROJECT INFORMATION
==================================================

Fields:

- Project title
- Description
- Featured image
- Author
- Category
- Occasion
- Season
- Difficulty

Difficulty options:

Easy
Intermediate
Advanced

Do not hard-code these values into the public template.

==================================================
22. DIY TIME + COST
==================================================

Fields:

- Preparation time
- Project time
- Total time
- Estimated cost
- Currency

Show a clear summary.

Allow "Cost not specified".

Do not invent cost data.

==================================================
23. MATERIALS BUILDER
==================================================

Create structured materials.

Each item:

- Quantity
- Unit
- Material name
- Optional note
- Optional affiliate product

Actions:

Add
Delete
Duplicate
Reorder

==================================================
24. TOOLS BUILDER
==================================================

Create structured tools list.

Fields:

- Tool name
- Optional quantity
- Optional affiliate product
- Optional note

Actions:

Add
Delete
Reorder

==================================================
25. DIY STEP BUILDER
==================================================

Create structured tutorial steps.

Each step:

- Step number
- Step title
- Instruction
- Step image
- Optional tip

Actions:

- Add step
- Delete
- Duplicate
- Reorder

Use the Media Library for step images.

==================================================
26. DIY TIPS
==================================================

Create:

Tips

Each tip:

- Title
- Description

Allow multiple tips.

==================================================
27. DIY VARIATIONS
==================================================

Create a Variations section.

Each variation:

- Variation title
- Description
- Optional image

Examples:

Color variation
Size variation
Seasonal variation
Material variation

Do not require variations for every project.

==================================================
28. DIY GALLERY
==================================================

Connect to the Media Library.

Support:

- Finished project images
- Process images
- Detail images

Allow:

- Reorder
- Captions
- Alt text
- Primary image

==================================================
29. DIY AFFILIATE PRODUCTS
==================================================

Allow editors to associate:

- Tools
- Materials
- Supplies
- Equipment

Use the existing Affiliate Product system.

Include appropriate disclosure.

==================================================
30. DIY SEO
==================================================

Connect to Phase 12.

Fields:

- SEO title
- Meta description
- Canonical
- Robots
- Sitemap inclusion
- Structured data where appropriate

Show SEO preview.

Do not create fake SEO scores.

==================================================
31. DIY PINTEREST
==================================================

Connect to Phase 9.

Fields:

- Pinterest title
- Pinterest description
- Primary pin image
- Pin template
- Alternate pins

Support multiple Pinterest assets.

==================================================
32. DIY PREVIEW
==================================================

Use the existing Universal DIY Page.

Preview:

Desktop
Tablet
Mobile

Show:

- Project information
- Materials
- Tools
- Steps
- Images
- Tips
- Variations
- Affiliate products
- Author
- Related projects
- Ads

==================================================
33. SPECIALIZED VALIDATION
==================================================

Recipe pre-publish checklist:

- Recipe title
- Description
- Featured image
- Author
- Ingredients
- Instructions
- Prep time
- Cook time
- Servings
- SEO
- Pinterest

DIY pre-publish checklist:

- Project title
- Description
- Featured image
- Author
- Difficulty
- Materials
- Tools
- Instructions
- SEO
- Pinterest

Clearly distinguish:

Required
Recommended
Optional

Do not force optional fields.

==================================================
34. UNIVERSAL CONTENT COMPATIBILITY
==================================================

Recipes and DIY projects must still support:

- Standard content blocks
- Images
- Galleries
- Videos
- Quotes
- Tables
- Callouts
- Affiliate blocks
- Sponsored blocks
- Advertisements
- Newsletter
- Related content
- Pinterest content

The specialized fields extend the Universal Content Editor.

They do not replace it.

==================================================
35. CONTENT TYPE CONVERSION
==================================================

Create a future-ready concept for converting content types where appropriate.

Example:

Article
→ Recipe

Article
→ DIY

Show a warning that specialized fields may need to be completed.

Do not automatically discard content.

==================================================
36. RESPONSIVE ADMIN EDITORS
==================================================

Test at:

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

- Single-column
- Collapsible settings
- Touch-friendly controls
- Easy ingredient editing
- Easy step editing
- No accidental horizontal scrolling

==================================================
37. ACCESSIBILITY
==================================================

Support:

- Keyboard navigation
- Focus states
- Accessible labels
- Screen-reader-friendly controls
- Accessible dialogs
- Move Up / Move Down alternatives to drag-and-drop

Do not make drag-and-drop the only way to reorder ingredients, steps, materials or gallery images.

==================================================
38. DATA ARCHITECTURE
==================================================

Conceptually extend:

ContentItem

with:

recipeData:
{
  prepTime,
  cookTime,
  totalTime,
  servings,
  ingredients[],
  instructions[],
  equipment[],
  nutrition,
  notes,
  tips[],
  gallery[]
}

and:

diyData:
{
  difficulty,
  prepTime,
  projectTime,
  totalTime,
  estimatedCost,
  materials[],
  tools[],
  steps[],
  tips[],
  variations[],
  gallery[]
}

Keep these specialized structures separate from the universal content fields.

==================================================
39. DO NOT BREAK EXISTING SYSTEMS
==================================================

Preserve:

- Public Recipe Page
- Public DIY Page
- Universal Article Page
- Universal Content Editor
- Media Library
- SEO Control Center
- Pinterest System
- Monetization
- Authors
- Search
- CMS Dashboard
- Responsive system
- Existing routes

==================================================
FINAL GOAL
==================================================

Create professional specialized CMS editors for Recipes and DIY/Tutorials while keeping them part of the same Universal Lifestyle CMS.

Editors should be able to create structured recipe and DIY content without writing code.

The specialized content must render through the existing public universal templates.

Build the UI, reusable components and data architecture now.

Actual database persistence, image processing, PDF generation, recipe calculations, authentication, storage and external integrations will be connected during production/backend implementation.

Run type checking/build validation after implementation.