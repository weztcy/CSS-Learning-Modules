# Portfolio Project Data — CSS Learning Modules

- **Category:** `code-learning` (`Code Learning`)
- **Accent Color:** `orange`
- **Target Assets Folder:** `public/images/projects/css_learning_modules/`
- **Required Local Images:** `banner.webp` ONLY

## TypeScript Data (`ProjectCaseStudy`)

```typescript
{
  "id": "css-learning-modules",
  "code": "PRO-48 // CL-04",
  "title": "CSS Learning Modules",
  "category": "code-learning",
  "categoryLabel": "Code Learning",
  "year": "2025",
  "status": "Completed",
  "accentColor": "orange",
  "repoUrl": "https://github.com/weztcy/CSS-Learning-Modules",
  "license": "MIT License",
  "banner": "/images/projects/css_learning_modules/banner.webp",
  "summary": "Structured 18-module CSS curriculum with 300 paired stylesheets, live HTML previews, and verified browser outputs from syntax to production layouts.",
  "codeLearningDescription": "A comprehensive 18-module frontend styling curriculum covering 300 standalone CSS lessons from syntax, selectors, cascade, and Box Model to Flexbox, Grid, animations, design tokens, and modern at-rules, each paired with an HTML preview and verified browser screenshot.",
  "architectureSummary": "Eighteen sequential module directories pair 300 isolated CSS stylesheets with live HTML previews, study guides, and PNG browser render captures.",
  "techStack": [
    "CSS",
    "HTML",
    "Web Browser",
    "Browser DevTools",
    "VS Code",
    "Markdown"
  ],
  "telemetryMatrix": {
    "projectType": "Web Styling Curriculum",
    "targetPlatform": "Modern Web Browsers",
    "primaryDomain": "Frontend CSS & Layout Engineering",
    "architecturePipeline": "18 Modules and 300 HTML Previews",
    "testingAndAudit": "Verified",
    "projectStatus": "Completed",
    "projectYear": "2025"
  },
  "codeLearningProjectInfo": {
    "learningCategory": "Frontend Web Styling & Layout Curriculum",
    "difficultyLevel": "Beginner to Advanced",
    "programmingLanguages": "CSS & HTML"
  },
  "codeLearningObjectives": [
    {
      "title": "Core Syntax, Selectors & Cascade Mechanics",
      "description": "Master CSS ruleset anatomy, combinators, attribute matchers, specificity scoring, property inheritance, and cascade layer conflict resolution.",
      "competencyCode": "COMP_01"
    },
    {
      "title": "Box Model, Typography & Visual Surfaces",
      "description": "Control sizing, margin collapse, logical properties, fluid typography, color spaces, layered gradients, shadows, and filter effects.",
      "competencyCode": "COMP_02"
    },
    {
      "title": "Responsive Layout Architecture",
      "description": "Build adaptive 1D and 2D interfaces using Flexbox, CSS Grid, media queries, clamp() fluid scaling, and container queries.",
      "competencyCode": "COMP_03"
    },
    {
      "title": "Interactive States, Motion & Modern CSS",
      "description": "Implement structural and relational pseudo-classes (:has, :is, :where), 2D/3D transforms, @keyframes animations, custom properties, @scope, and native nesting.",
      "competencyCode": "COMP_04"
    },
    {
      "title": "Scalable Stylesheet Architecture & UI Builds",
      "description": "Apply CSS Reset, Normalize, BEM naming, utility classes, accessible form/table styling, and complete multi-section web page builds.",
      "competencyCode": "COMP_05"
    }
  ],
  "codeLearningPrerequisites": [
    {
      "category": "Foundational Knowledge",
      "items": [
        "Basic HTML5 document structure and semantic tags",
        "Understanding of element nesting, classes, IDs, and attributes"
      ],
      "description": "Learners should be comfortable reading basic HTML markup and linking external stylesheet files inside a document head."
    },
    {
      "category": "Tooling Setup",
      "items": [
        "Modern web browser (Chrome, Edge, or Firefox)",
        "Code editor such as VS Code",
        "Optional local HTTP server or Live Server extension"
      ],
      "description": "All 300 HTML preview files run natively in any modern web browser without bundlers, compilers, or external package installations."
    }
  ],
  "codeLearningCurriculumStructure": {
    "summary": "The curriculum scales progressively across five phases from CSS fundamentals to full-page UI engineering. Early modules establish selectors, cascade mechanics, and box sizing before advancing through Flexbox, Grid, responsive queries, motion, design tokens, and five capstone builds.",
    "totalEstimatedHours": "94 Hours",
    "phases": [
      {
        "phaseNumber": "01",
        "phaseTitle": "CSS Foundations & Core Mechanics",
        "difficulty": "Beginner",
        "moduleRange": "Modules 01 - 04",
        "topics": [
          "Basic Syntax & Units",
          "Selectors & Combinators",
          "Cascade, Specificity & Inheritance",
          "Box Model & Logical Sizing"
        ]
      },
      {
        "phaseNumber": "02",
        "phaseTitle": "Typography, Color & Visual Flow",
        "difficulty": "Beginner",
        "moduleRange": "Modules 05 - 08",
        "topics": [
          "Web Typography & @font-face",
          "Colors, Gradients & Blend Modes",
          "Borders, Shadows & Backdrop Filters",
          "Display, Positioning & Overflow"
        ]
      },
      {
        "phaseNumber": "03",
        "phaseTitle": "Modern Layout & Responsive Systems",
        "difficulty": "Intermediate",
        "moduleRange": "Modules 09 - 12",
        "topics": [
          "Flexbox Layout Patterns",
          "Two-Dimensional CSS Grid",
          "Media & Container Queries",
          "Pseudo-classes (:has) & Pseudo-elements"
        ]
      },
      {
        "phaseNumber": "04",
        "phaseTitle": "Motion, Variables & Modern At-Rules",
        "difficulty": "Intermediate",
        "moduleRange": "Modules 13 - 15",
        "topics": [
          "2D/3D Transforms & @keyframes",
          "Custom Properties & Design Tokens",
          "color-mix() & light-dark() Functions",
          "@layer, @scope, @property & Nesting"
        ]
      },
      {
        "phaseNumber": "05",
        "phaseTitle": "UI Components, Architecture & Capstones",
        "difficulty": "Advanced",
        "moduleRange": "Modules 16 - 18",
        "topics": [
          "Accessible Forms & Responsive Tables",
          "Reset, Normalize, BEM & Utility Classes",
          "Profile Card & Portfolio Builds",
          "Dashboard, E-Commerce & Landing Page"
        ]
      }
    ]
  },
  "codeLearningModules": [
    {
      "id": "mod-01",
      "moduleNumber": "01",
      "title": "CSS Introduction & Basic Syntax",
      "description": "Introduces stylesheet rulesets, declarations, inline/internal/external inclusion, comments, whitespace, units, color formats, and browser defaults.",
      "submoduleCount": 15,
      "difficulty": "Beginner",
      "keyTopics": ["Ruleset Anatomy", "Inline vs Internal vs External", "CSS Units & Colors", "User-Agent Defaults"],
      "sourceFilesCount": 30,
      "estimatedHours": "4 Hours"
    },
    {
      "id": "mod-02",
      "moduleNumber": "02",
      "title": "CSS Selectors",
      "description": "Covers universal, element, class, ID, and grouping selectors alongside combinators, seven attribute matching operators, and complex selector lists.",
      "submoduleCount": 20,
      "difficulty": "Beginner",
      "keyTopics": ["Basic Selectors", "Combinators (>, +, ~)", "Attribute Matchers", "Complex Selector Lists"],
      "sourceFilesCount": 40,
      "estimatedHours": "5 Hours"
    },
    {
      "id": "mod-03",
      "moduleNumber": "03",
      "title": "Cascade, Specificity & Inheritance",
      "description": "Explains cascade ordering, specificity scoring, source order, inherited vs non-inherited properties, reset keywords, !important, and @layer.",
      "submoduleCount": 15,
      "difficulty": "Beginner",
      "keyTopics": ["Specificity Math", "Inheritance Control", "initial/inherit/unset/revert", "Cascade Layers (@layer)"],
      "sourceFilesCount": 30,
      "estimatedHours": "5 Hours"
    },
    {
      "id": "mod-04",
      "moduleNumber": "04",
      "title": "CSS Box Model",
      "description": "Examines content, padding, border, and margin layers, content-box vs border-box, min/max bounds, margin collapse, logical properties, and aspect-ratio.",
      "submoduleCount": 20,
      "difficulty": "Beginner",
      "keyTopics": ["border-box Sizing", "Margin Collapsing", "Logical Margin & Padding", "Intrinsic Sizing & aspect-ratio"],
      "sourceFilesCount": 40,
      "estimatedHours": "5 Hours"
    },
    {
      "id": "mod-05",
      "moduleNumber": "05",
      "title": "Typography & Text Formatting",
      "description": "Explores font stacks, sizing, weights, line-height, text decoration and shadows, overflow ellipsis, wrapping controls, and @font-face web fonts.",
      "submoduleCount": 20,
      "difficulty": "Beginner",
      "keyTopics": ["Font Stacks & @font-face", "Line Height & Alignment", "Text Truncation & Wrapping", "Typography Shorthand"],
      "sourceFilesCount": 40,
      "estimatedHours": "5 Hours"
    },
    {
      "id": "mod-06",
      "moduleNumber": "06",
      "title": "Colors & Backgrounds",
      "description": "Covers named, HEX, RGB, HSL, and alpha colors, background sizing and positioning, layered backgrounds, linear/radial/conic gradients, and blend modes.",
      "submoduleCount": 20,
      "difficulty": "Beginner",
      "keyTopics": ["HEX, RGB & HSL Alpha", "Multiple Backgrounds", "Linear, Radial & Conic Gradients", "background-clip & Blend Modes"],
      "sourceFilesCount": 40,
      "estimatedHours": "5 Hours"
    },
    {
      "id": "mod-07",
      "moduleNumber": "07",
      "title": "Borders, Outlines, Shadows & Visual Effects",
      "description": "Details border properties and radius, accessibility outlines and offsets, layered box shadows, opacity, graphic filters, backdrop-filter, and clip-path.",
      "submoduleCount": 15,
      "difficulty": "Intermediate",
      "keyTopics": ["Borders & border-radius", "Outline vs Border", "Layered Box Shadows", "backdrop-filter & clip-path"],
      "sourceFilesCount": 30,
      "estimatedHours": "4 Hours"
    },
    {
      "id": "mod-08",
      "moduleNumber": "08",
      "title": "Display, Positioning & Overflow",
      "description": "Covers block/inline/inline-block flow, visibility vs display: none, static/relative/absolute/fixed/sticky positioning, stacking contexts, overflow, and object-fit.",
      "submoduleCount": 20,
      "difficulty": "Intermediate",
      "keyTopics": ["Display Modes", "Positioning Schemes & Inset", "z-index & Stacking Context", "Overflow & object-fit"],
      "sourceFilesCount": 40,
      "estimatedHours": "6 Hours"
    },
    {
      "id": "mod-09",
      "moduleNumber": "09",
      "title": "Flexbox Layout",
      "description": "Teaches main and cross axis alignment, wrapping, flex-grow/shrink/basis, ordering, gap spacing, and practical navigation, card, and sidebar layouts.",
      "submoduleCount": 20,
      "difficulty": "Intermediate",
      "keyTopics": ["Flex Direction & Wrapping", "justify-content & align-items", "Flex Sizing & Gap", "Navigation & Card Patterns"],
      "sourceFilesCount": 40,
      "estimatedHours": "6 Hours"
    },
    {
      "id": "mod-10",
      "moduleNumber": "10",
      "title": "CSS Grid Layout",
      "description": "Presents two-dimensional grid tracks, template areas, column/row spanning, auto-fit/auto-fill, minmax(), fractional fr units, and dashboard layouts.",
      "submoduleCount": 20,
      "difficulty": "Intermediate",
      "keyTopics": ["Grid Tracks & Template Areas", "auto-fit vs auto-fill", "minmax() & fr Units", "Grid Dashboard Architecture"],
      "sourceFilesCount": 40,
      "estimatedHours": "6 Hours"
    },
    {
      "id": "mod-11",
      "moduleNumber": "11",
      "title": "Responsive Web Design",
      "description": "Covers media queries, mobile-first vs desktop-first breakpoints, clamp() fluid typography, preference queries, print styles, and @container queries.",
      "submoduleCount": 20,
      "difficulty": "Intermediate",
      "keyTopics": ["Mobile-First Breakpoints", "Fluid clamp() Typography", "prefers-color-scheme & Motion", "Container Queries (@container)"],
      "sourceFilesCount": 40,
      "estimatedHours": "6 Hours"
    },
    {
      "id": "mod-12",
      "moduleNumber": "12",
      "title": "Pseudo-classes & Pseudo-elements",
      "description": "Explores interaction and form states, structural nth-child selectors, modern :not/:is/:where/:has selectors, and ::before/::after/::marker/::selection styling.",
      "submoduleCount": 20,
      "difficulty": "Intermediate",
      "keyTopics": ["Focus & Form States", "Structural :nth-child() Formulas", ":is(), :where() & :has()", "::before, ::after & ::marker"],
      "sourceFilesCount": 40,
      "estimatedHours": "6 Hours"
    },
    {
      "id": "mod-13",
      "moduleNumber": "13",
      "title": "Transform, Transition & Animation",
      "description": "Demonstrates 2D/3D geometric transforms, perspective and backface-visibility, transition timing curves, @keyframes timelines, and multi-animation composition.",
      "submoduleCount": 20,
      "difficulty": "Intermediate",
      "keyTopics": ["2D & 3D Transforms", "Perspective & preserve-3d", "Transition Timing & Delay", "@keyframes Orchestration"],
      "sourceFilesCount": 40,
      "estimatedHours": "6 Hours"
    },
    {
      "id": "mod-14",
      "moduleNumber": "14",
      "title": "CSS Variables, Functions & Calculations",
      "description": "Teaches custom properties, :root vs component scope, calc/min/max/clamp math, color-mix(), relative colors, light-dark(), CSS counters, and design tokens.",
      "submoduleCount": 20,
      "difficulty": "Advanced",
      "keyTopics": ["Custom Properties & Fallbacks", "calc(), min(), max(), clamp()", "color-mix() & light-dark()", "Design Tokens & CSS Counters"],
      "sourceFilesCount": 40,
      "estimatedHours": "6 Hours"
    },
    {
      "id": "mod-15",
      "moduleNumber": "15",
      "title": "At-rules & Modern CSS Features",
      "description": "Covers @media, @supports feature detection, @layer ordering, @container, @scope isolation, Houdini @property, native CSS nesting, and scroll snapping.",
      "submoduleCount": 15,
      "difficulty": "Advanced",
      "keyTopics": ["@supports Feature Detection", "@scope & @property", "Native CSS Nesting (&)", "CSS Scroll Snap & Smooth Scroll"],
      "sourceFilesCount": 30,
      "estimatedHours": "5 Hours"
    },
    {
      "id": "mod-16",
      "moduleNumber": "16",
      "title": "Forms, Tables & Component Styling",
      "description": "Focuses on accessible form inputs, validation states, custom checkboxes/radios, button systems, zebra-striped responsive tables, scrollbars, and details/summary.",
      "submoduleCount": 10,
      "difficulty": "Advanced",
      "keyTopics": ["Form Focus & Validation States", "Custom Checkbox & Radio Controls", "Responsive Data Tables", "Custom Scrollbars & Accordions"],
      "sourceFilesCount": 20,
      "estimatedHours": "4 Hours"
    },
    {
      "id": "mod-17",
      "moduleNumber": "17",
      "title": "CSS Architecture, Debugging & Best Practices",
      "description": "Addresses large-scale stylesheet engineering with CSS Reset, Normalize.css principles, BEM naming conventions, utility classes, and modular file organization.",
      "submoduleCount": 5,
      "difficulty": "Advanced",
      "keyTopics": ["CSS Reset vs Normalize", "BEM Naming Convention", "Utility-First Classes", "Modular CSS Organization"],
      "sourceFilesCount": 10,
      "estimatedHours": "4 Hours"
    },
    {
      "id": "mod-18",
      "moduleNumber": "18",
      "title": "CSS Practical Projects",
      "description": "Synthesizes all preceding modules into five real-world frontend UI implementations spanning components, portfolios, dashboards, e-commerce, and landing pages.",
      "submoduleCount": 5,
      "difficulty": "Advanced",
      "keyTopics": ["Profile Card Component", "Responsive Portfolio", "Analytics Dashboard Grid", "E-Commerce & Full Landing Page"],
      "sourceFilesCount": 10,
      "estimatedHours": "6 Hours"
    }
  ],
  "codeLearningPracticalProjects": [
    {
      "title": "Profile Card UI Component (Submodule 296)",
      "description": "Construct a modern user profile card featuring a cover header, circular overlapping avatar, absolute online indicator, bio metadata, and profile metric counters.",
      "highlights": [
        "Flexbox vertical and horizontal alignment for identity and action controls",
        "Circular avatar framing with crisp border separation and absolute status badge",
        "Structured metric grid displaying user activity counts cleanly"
      ],
      "coreScope": "Self-contained interactive UI card component using Flexbox, positioning, and visual elevation.",
      "trackTag": "UI Component Lab",
      "tier": "Core",
      "difficulty": "Intermediate",
      "estimatedTime": "1 Hour",
      "architecturalConstraints": [
        "Pure CSS and HTML with zero JavaScript",
        "Consistent box-shadow elevation and rounded container clipping"
      ]
    },
    {
      "title": "Responsive Portfolio Page (Submodule 297)",
      "description": "Design a multi-section personal portfolio page pairing a hero introduction banner with an adaptive multi-column project gallery.",
      "highlights": [
        "Responsive grid gallery that adapts column counts across viewport widths",
        "Balanced typographic hierarchy separating hero headline from project cards",
        "Hover transition feedback across interactive project preview cards"
      ],
      "coreScope": "Multi-section personal showcase adapting fluidly between desktop and mobile viewports.",
      "trackTag": "Responsive Layout Lab",
      "tier": "Core",
      "difficulty": "Intermediate",
      "estimatedTime": "1.5 Hours",
      "architecturalConstraints": [
        "Responsive multi-column CSS Grid without external frameworks",
        "Mobile-safe spacing and readable line lengths"
      ]
    },
    {
      "title": "Analytics Dashboard Layout (Submodule 298)",
      "description": "Build a two-dimensional web application dashboard shell combining a fixed-width dark sidebar, top utility header, and a three-column KPI metrics grid.",
      "highlights": [
        "CSS Grid application shell with 200px navigation sidebar and fluid main column",
        "Three-column KPI card row using repeat(3, 1fr) with consistent gutters",
        "Active and hover navigation states with clean border and shadow separation"
      ],
      "coreScope": "Application-grade 2D layout combining CSS Grid page regions with Flexbox header and sidebar internals.",
      "trackTag": "Capstone Layout",
      "tier": "Advanced",
      "difficulty": "Advanced",
      "estimatedTime": "1.5 Hours",
      "architecturalConstraints": [
        "Two-dimensional Grid shell paired with Flexbox inner alignments",
        "Contained card styling with subtle 1px borders and elevation"
      ]
    },
    {
      "title": "E-Commerce Storefront Layout (Submodule 299)",
      "description": "Implement an online store product catalog grid featuring product cards, promotional discount badges, pricing hierarchy, and purchase action buttons.",
      "highlights": [
        "Commercial product grid displaying uniform card heights and clean image framing",
        "Positioned discount badges and clear price/discount typographic contrast",
        "Interactive button states designed for high-clarity catalog browsing"
      ],
      "coreScope": "Multi-card commercial catalog grid demonstrating visual hierarchy and component consistency.",
      "trackTag": "Commerce UI Lab",
      "tier": "Advanced",
      "difficulty": "Advanced",
      "estimatedTime": "1 Hour",
      "architecturalConstraints": [
        "Uniform card grid alignment across varying product metadata lengths",
        "Pure CSS badge positioning and button hover transitions"
      ]
    },
    {
      "title": "Full Website Landing Page (Submodule 300)",
      "description": "Deliver a complete multi-section website landing page with a sticky blurred navigation bar, centered hero CTA group, feature card grid, and footer.",
      "highlights": [
        "Sticky header navigation using translucent backdrop-filter blur",
        "Centered hero section with pill badge, typographic scale, and dual CTA layout",
        "Integrated feature grid and multi-column footer under a unified design system"
      ],
      "coreScope": "End-to-end production-style landing page synthesizing layout, typography, effects, and navigation.",
      "trackTag": "Final Capstone",
      "tier": "Advanced",
      "difficulty": "Advanced",
      "estimatedTime": "1 Hour",
      "architecturalConstraints": [
        "Zero external CSS frameworks or JavaScript dependencies",
        "Cohesive color palette, z-index sticky header, and border-box reset"
      ]
    }
  ],
  "codeLearningOutcomes": [
    {
      "pillar": "Layout & Responsive Systems",
      "skills": [
        {
          "title": "Flexbox & CSS Grid Composition",
          "description": "Combine one-dimensional Flexbox alignment with two-dimensional CSS Grid templates to construct dashboards, navigation bars, and responsive card galleries."
        },
        {
          "title": "Viewport & Container Adaptability",
          "description": "Use mobile-first media queries, clamp() fluid scaling, and @container rules so components adapt to both screen dimensions and parent containers."
        }
      ]
    },
    {
      "pillar": "Modern CSS & Design Systems",
      "skills": [
        {
          "title": "Custom Properties & Dynamic Functions",
          "description": "Architect reusable design tokens with :root variables, calc(), color-mix(), and light-dark() for consistent theming across light and dark modes."
        },
        {
          "title": "Cascade Governance & Clean Selectors",
          "description": "Resolve specificity conflicts predictably using @layer, @scope, BEM conventions, and relational pseudo-classes such as :has() and :where()."
        }
      ]
    }
  ],
  "codeLearningCurriculumSpecs": {
    "curriculumTrack": "Modern CSS Frontend Mastery",
    "primaryLanguage": "CSS and HTML",
    "executionRuntime": "Modern Web Browser",
    "testVerification": "Visual Output Screenshots"
  },
  "codeLearningSupplementaryResources": [
    {
      "title": "Module Study Guides",
      "description": "Eighteen structured module-level Markdown guides documenting scope, learning objectives, code explanations, and run instructions for every submodule.",
      "resources": [
        {
          "name": "Module 01-18 Curriculum Guides (README.md)",
          "type": "Reference Guide",
          "format": "MD"
        }
      ]
    },
    {
      "title": "Visual Execution Outputs",
      "description": "Three hundred browser-rendered PNG reference captures stored inside each module's output directory for visual self-verification.",
      "resources": [
        {
          "name": "Submodule 001-300 Browser Render Captures (output/*.png)",
          "type": "Visual Reference",
          "format": "PNG"
        }
      ]
    }
  ]
}
```
