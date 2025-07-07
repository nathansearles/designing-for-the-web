# Designing for the Web

### _A Shared Language for Designers and Developers_

---

## Welcome

When designers and developers speak the same language, great things happen.

This guide shares the principles that help create consistent, scalable UI designs — making it easier to collaborate, build faster, and deliver better experiences for users.

Use it as a reference, revisit it often, and most importantly, adapt it to fit your team's needs.

---

## Table of Contents

- [Cool, so what’s this about?](#cool-so-whats-this-about)
- [TL;DR](#tldr)
- [UI Design System](#ui-design-system)
  - [Why Use a Design System?](#why-use-a-design-system)
  - [Core Elements of the System](#core-elements-of-the-system)
- [Grids](#grids)
  - [Why Use a Grid?](#why-use-a-grid)
  - [Grid Basics](#grid-basics)
- [Responsive](#responsive)
  - [Key Principles of Responsive Design](#key-principles-of-responsive-design)
- [Containers](#containers)
  - [Why Containers Matter](#why-containers-matter)
  - [Example](#example)
- [Typography](#typography)
  - [Key Principles of Typography](#key-principles-of-typography)
  - [Best Practices for Readability](#best-practices-for-readability)
- [Spacing](#spacing)
  - [Key Principles of Spacing](#key-principles-of-spacing)
- [Color](#color)
  - [Key Principles of Color](#key-principles-of-color)
- [Designing for CMS-Powdered Websites](#designing-for-cms-powdered-websites)
- [Things Not to Do](#things-not-to-do)
- [Tools and Resources](#tools-and-resources)
  - [Design Tools](#design-tools)
  - [Further Reading and Inspiration](#further-reading-and-inspiration)
- [Wrapping Up](#wrapping-up)

---

## Cool, so what’s this about?

This guide is a collection of principles designed to create a shared language between design and development, fostering consistent, scalable UI designs that enhance user experience and brand engagement.

## TL;DR

- **Fonts and Spacing:**  
  Most browsers start with **16px** as the default font size. Base your sizing on simple multiples of 16 to keep designs consistent and scalable.

- **REM Units:**  
  Use REM units for all fonts and spacing.  
  1rem equals **16px** by default in most browsers — the same base size you’re already designing with.  
  Using REMs keeps your sizing flexible, scalable, and accessible, because it adjusts automatically if a user changes their browser settings.

- **Fluid Scaling:**  
  Fonts and spacing should **scale fluidly** with the container, not stay fixed.

- **Breakpoints:**  
  Use **manual breakpoints only when necessary** — content should define when layout changes, not screen size alone.

- **12-Column Grid:**  
  A **12-column grid** offers flexible layout options (2, 3, 4, or 6 columns) without feeling locked in.

- **Grid Alignment:**  
  **Not everything must snap to the grid.** Some elements should stay fixed, others should flex based on content.

## UI Design System

Building a design system creates a shared foundation for consistency, scalability, and better collaboration between design and development.

### Why Use a Design System?

A design system improves consistency, speeds up workflows, scales across teams, boosts quality, simplifies maintenance, and ensures accessibility.

#### **Core Elements of the System**

- **Type Scale:**  
  Set up a system of type tokens that define the minimum and maximum font sizes based on the container.

- **Space Scale:**  
   Establish a predefined set of spacing values that scale fluidly within a container.

- **Container:**  
  Define a maximum content width; below that width, let the layout adjust fluidly to the viewport.

- **Grid:**  
  Use a 12-column grid as a guide — but don't feel locked in. Creativity and user experience come first.

- **Colors:**  
  Use an accessible color palette with lighter and darker shades for flexibility and clarity.

- **Components:**  
  Create reusable UI building blocks designed to work seamlessly together and form intuitive user patterns.

- **Design Tokens:**  
  Design tokens store core values like color, spacing, and typography as data, keeping your system scalable and consistent.

## Grids

A grid system provides a foundation for layout consistency between design and development — but knowing when (and how) to break the rules is just as important as following them.

### Why Use a Grid?

- **Consistency and Alignment:**  
  Grids keep layouts aligned and consistent across pages and components.

- **Visual Hierarchy:**  
  Grids help users easily scan and understand content by creating a clear hierarchy.

- **Efficiency:**  
  Designing within a grid speeds up decision-making and layout creation.

- **Responsiveness:**  
  A structured grid makes it easier to design layouts that adapt across screen sizes.

- **User Experience:**  
  Organized layouts improve usability and make interfaces feel intentional.

- **Collaboration:**  
  A shared grid system gives designers and developers a common language to work from.

### Grid Basics

- **Core Elements:**  
  A grid consists of a **container**, **columns**, **gutters**, and **margins**. Define these globally to create a solid, flexible foundation.

- **Starting Point:**  
  Begin with a **1440px container**, **12 columns**, and **32px gutters and margins**. Tweak these values as needed for your project.

- **Content-Based Alignment:**  
  Don’t force text to snap to the grid. Align based on content instead — aim for **45–75 characters per line** for optimal readability.

- **Flexibility over Rigidity:**  
  Overemphasizing strict grid alignment can make designs feel stiff or generic. It’s okay to break the grid when it improves creativity, functionality, or user experience.

## Responsive

Responsive design ensures your website adjusts fluidly across different screen sizes and devices — creating a seamless, consistent experience for everyone.

### Key Principles of Responsive Design

- **Content-First Approach:**  
   Viewports come in all shapes and sizes. Design based on **content needs**, not fixed device sizes.

- **Consistent Experience:**  
  Users expect a consistent experience across phones, tablets, laptops, and desktops. Responsive design makes sure they get it.

- **Modular Scale:**  
  Use a **modular scale** to size fonts and design elements proportionally. A consistent ratio creates visual harmony across devices.

- **Media Queries:**  
  **Media queries** let you fine-tune styles based on characteristics like screen width, height, or orientation — but they should support, not drive, the design.

- **Remember:**  
  Design for flexibility, not perfection. Real-world users don't browse in perfect screen sizes.

## Containers

Containers set the boundaries for your content — defining how wide your layouts are and keeping designs consistent and fluid across different screen sizes.

### Why Containers Matter

- **Consistency:**  
  Containers create a consistent layout structure from page to page and component to component. They also define the width of columns, gutters, and margins.

- **Fluid Width:**  
  Set a **maximum container width**. When the viewport is wider than this max, content stays centered. When it’s smaller, the container fluidly adjusts to the viewport size.

- **Internal Grid:**  
  Use a 12-column internal grid inside the container to manage layout, spacing, and alignment — including inset blocks of content.

- **Tip:**  
  Think of the container as the frame for your artwork — it keeps everything clean, balanced, and focused.

### Example

If your max width is **1440px** with **32px margins** on the left and right:

- The maximum content width inside the container would be **1376px**.
- (1376px \+ 32px \+ 32px \= 1440px)

## Typography

Good typography is the backbone of good design — it drives readability, accessibility, and the overall feel of your product.

### Key Principles of Typography

- **REM Units:**  
  Use **REM** units for all fonts and spacing.

  - 1rem \= 16px (default browser setting).

  - Example: 48px font size → **3rem** (48 ÷ 16 \= 3).

- **Accessibility First:**  
  REM units make designs more accessible by allowing users to adjust their browser’s base font size — making sure your site scales naturally to user preferences.

- **Type System:**  
  Create a defined type system (e.g., headings, body, captions) to promote visual consistency and simplify design decisions.

- **Fluid Type Scale:**  
  Set minimum and maximum font sizes based on container width.

  - This makes type **fluid** and adaptive across devices.

  - Tools like [Utopia](https://utopia.fyi) can help generate your type scales.

- **Design Tokens:**  
  Capture font sizes, line heights, and spacing as **design tokens**. This keeps your typography scalable and easy to maintain across both design and code.

### Best Practices for Readability

- **Line Length:**  
   Keep paragraphs between **45–75 characters per line** for optimal reading comfort.

- **Line Height:**

  - Larger headlines → \~100% line height.

  - Smaller body text → \~150% line height.

- **Letter Spacing:**  
   As font size increases, **slightly reduce letter spacing** to maintain readability.

- **Alignment:**

  - **Left-align** text for readability.

  - Center-align short blocks of text only (2–3 lines max).  
    Avoid centering long paragraphs.

- **Tip:**  
  Good typography should feel invisible — users should notice the content, not the font choices.

## Spacing

Thoughtful spacing gives designs structure, balance, and rhythm — and makes interfaces easier to scan and use.

### Key Principles of Spacing

- **REM Units for Spacing:**  
  Use **REM** units to define all spacing values, just like with typography.

  - 1rem \= 16px (default browser font size).

  - Using REMs ensures spacing scales properly for accessibility.

- **Spacing System:**  
  Define a **system of spacing values** (small, medium, large, etc.) to create consistency across layouts.  
   Fewer spacing choices \= faster, cleaner designs.

- **Accessibility:**  
  REM-based spacing ensures that when users adjust their font size settings, **spacing scales too** — preserving layout and readability.

- **Grouping and Proximity:**  
  According to the **[Gestalt principle of proximity](https://en.wikipedia.org/wiki/Principles_of_grouping)**, items placed close together are perceived as related. Use spacing intentionally to guide users through content.

- **Design Tokens:**  
  Store your spacing values as **design tokens** to sync design and development, keeping everything scalable and consistent.

- **Tip:**  
  When in doubt, add a little more space. Crowded designs feel overwhelming — generous spacing feels intentional.

## Color

Color sets the mood, guides attention, and strengthens brand identity — but it needs to be used thoughtfully to stay accessible and effective.

### Key Principles of Color

- **Accessibility:**  
  Follow the **WCAG guidelines** for contrast:

  - Normal text (\~18px or smaller): **4.5:1 contrast ratio** minimum.

  - Large text (18px+ bold or 24px+ regular): **3:1 contrast ratio** minimum.  
     Learn more: [WebAIM Color Accessibility Guide](https://webaim.org/articles/contrast/)

- **The 60/30/10 Rule:**  
  Use **60%** primary color, **30%** secondary color, and **10%** accent color to create a balanced, visually appealing design. [Watch: 60/30/10 Rule Explained (YouTube)](https://www.youtube.com/watch?v=nrN2axSSOKg)

- **Using Shades:**  
  You'll need **more shades than you think** — plan for:

  - **8–10 shades of gray** (backgrounds, borders, disabled states).

  - **5–10 shades** for each primary and accent color (hover states, active states, dark mode, etc.)

- **Tip:**  
  Design for real use, not just the perfect moodboard. Your colors need to look good in buttons, backgrounds, error states — everywhere.

## Designing for CMS-Powdered Websites

CMS-powered sites are dynamic by nature. Your design needs to be just as flexible — ready to adapt without losing its integrity.

Modern websites are often built on a CMS (Content Management System), which means content isn’t hard-coded onto a page — it’s made up of reusable components that can be rearranged by editors.

When designing for a CMS-powdered site, think about layouts as flexible systems — not rigid page templates.

**Key Principles:**

- **Design for Modularity:**
  Treat each section or block as a standalone component. Assume it might appear before or after other components in different contexts.
- **Plan for Reordering:**
  Make sure the design doesn’t fall apart if someone moves components around. The layout and style should stay strong and coherent, even when content order changes.
- **Define Clear Relationships:**
  Use consistent spacing, typography, and visual cues to show how components relate to each other — without relying on fixed positioning or static page designs.
- **Flexibility Without Losing Intent:**
  Good modular design maintains the original design intent — visual rhythm, hierarchy, and storytelling — even when the order of content shifts.

## Things Not to Do

Even with the best intentions, there are a few practices that can hurt user experience if not handled carefully. Here’s what to watch out for:

### Scrolljacking

Scrolljacking takes control away from the user — and usually not in a good way. By overriding a user's natural scrolling behavior, you introduce friction and frustration into an otherwise smooth experience.

We encourage healthy uses of sticky content, but advise against parallel scrolljacking (where vertical scrolling snaps or hijacks content on the same vertical axis). However, there are more pleasant experiences with perpendicular scrolljacking ([example](https://rivian.com/): horizontal scrolling triggered by vertical movement) when done thoughtfully.

**Responsiveness is key:**
If content doesn’t match the user’s scroll velocity, the page can feel slow, clunky, and non-performant.

### Opacity as Indicators

Be intentional when choosing colors and treatments for disabled elements. When a button is tinted gray, users generally expect it to be inactive. Problems arise when low-opacity elements unintentionally look disabled even though they are still interactive.

This often happens when reducing opacity to make something look "less important" — but visually, it reads as disabled.

**Quick rule of thumb:**
- Elements feel **active** when contrast **increases**.
- Elements feel **inactive** when contrast **decreases**.

If users can’t tell whether something is clickable, they hesitate — or worse, they miss it entirely.

## Tools and Resources

Here are some tools and references to level up your designs and help you build systems that scale.

### Design Tools

- [**Fluid Type Scale Calculator**](https://utopia.fyi/type/calculator/?c=320,16,1.2,1536,18,1.25,7,2,&s=0.75%7C0.5%7C0.25,1.5%7C2%7C3%7C4%7C6,s-l&g=s,l,xl,12)**:**  
   Create fluid font size values that adapt across screen sizes.

- [**Fluid Space Calculator**](https://utopia.fyi/space/calculator/?c=320,16,1.2,1536,32,1.25,5,2,&s=0.75%7C0.5%7C0.25,1.5%7C2%7C3%7C4%7C6,s-l&g=s,l,xl,12)**:**  
   Set up fluid spacing values to maintain consistent, flexible layouts.

- [**Fluid Grid Calculator**](https://utopia.fyi/grid/calculator/?c=320,16,1.2,1536,32,1.25,5,2,&s=0.75%7C0.5%7C0.25,1.5%7C2%7C3%7C4%7C6,s-l&g=s,s,xl,12)**:**  
   Generate grid settings and visualize how your layout scales.

- [**Utopia Figma Plugin**](https://utopia.fyi/blog/figma-plugin-v2/)**:**  
   Quickly create named type styles and spacing components directly inside Figma.

- [**WebAIM Contrast Checker**](https://webaim.org/resources/contrastchecker/)**:**  
   Test color contrast ratios to make sure your designs are accessible.

### **Further Reading and Inspiration**

- [**Refactoring UI**](https://www.refactoringui.com/)**:**  
  Practical design advice explained from a developer’s perspective.

- [**New Responsive**](https://web.dev/articles/new-responsive)**:**  
  Rethink responsive design in a component-driven, modern web.

- [**Understanding Flexbox and CSS Grid**](https://uxdesign.cc/why-ui-designers-should-understand-flexbox-and-css-grid-e236a9dec37a?gi=8050e9970067)**:**  
  Bridge the mental model gap between designers and developers around layout systems.

- [**What Are Design Tokens?**](https://piccalil.li/blog/what-are-design-tokens/)**:**  
  Learn how tokens translate design decisions into scalable systems.

- [**Uber Base Design System**](https://base.uber.com/6d2425e9f/p/785d5f-layout-grids)**:**  
  See how Uber structures their grids and layout principles.

- [**The Secret Science of Perfect Spacing**](https://www.youtube.com/watch?v=9ElrcTtAxzA)**:**  
  How smart spacing gives interfaces that "oddly satisfying" feeling.

- [**The Component Gallery**](https://component.gallery/)**:**  
  A visual reference of real-world components from design systems across the web.

- [**Viewports.fyi**](https://viewports.fyi/)**:**  
  Explore real-world viewport sizes to design beyond arbitrary breakpoints.

## Wrapping Up

Design systems aren’t built in a day. Stay flexible, collaborate often, and always design with real users in mind.

Focus on building consistency and scalability — but never lose sight of creativity, adaptability, and the real people you’re designing for.
