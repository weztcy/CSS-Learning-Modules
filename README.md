# CSS Learning Modules

[![CSS Standard](https://img.shields.io/badge/CSS3-Living%20Standard-1572B6?logo=css3&logoColor=white)](https://www.w3.org/Style/CSS/) [![Curriculum Modules](https://img.shields.io/badge/Modules-18%20Pedagogical%20Modules-2ea44f)](#learning-roadmap) [![Interactive Lessons](https://img.shields.io/badge/Lessons-300%20CSS%20Modules-blue)](#learning-modules--subtopics) [![Rendered Captures](https://img.shields.io/badge/Output%20Captures-300%20Verified%20Outputs-8a2be2)](#learning-modules--subtopics) [![W3C Validation & Standards](https://img.shields.io/badge/Standards-W3C%20CSS%20Specs-success)](#tech-stack--tools) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE)

![CSS Learning Modules Banner](./screenshots/banner.png)

## Project Description

**CSS Learning Modules** is an exhaustive, production-grade educational curriculum designed to guide learners from fundamental styling syntax through advanced layout engines, responsive web architectures, modern CSS features, and complete production web applications.

Structured across **18 pedagogical modules** containing **300 fully standalone CSS stylesheets and HTML previews**, this repository bridges declarative theory and live browser execution. Each lesson pairs an isolated `.css` stylesheet with an interactive `.html` preview document and a verified browser rendering capture (`output/`) recorded directly from modern rendering engines. Built entirely with pure, vanilla CSS without third-party frameworks or preprocessors, this curriculum serves as an authoritative, code-first reference for mastering the web's design foundation.

## Learning Objectives

Learners engaging with this curriculum will develop concrete, industry-standard frontend styling and design skills across every core domain of modern web development:

- **Core Syntax & Ruleset Anatomy**: Master selector syntax, declaration blocks, properties, values, units, and integration methods (inline, internal, external).
- **Selectors & Combinators**: Leverage universal, type, class, ID, attribute selectors (exact, substring, prefix, suffix), and structural combinators (child, descendant, adjacent/general sibling).
- **Cascade, Specificity, & Inheritance**: Understand browser cascade algorithms, specificity weighting calculation (inline > ID > class > type), inheritance behavior, value keywords (`inherit`, `initial`, `unset`, `revert`), and cascade layers (`@layer`).
- **Box Model & Sizing Mechanics**: Dissect content, padding, border, and margin layers, `box-sizing` (`content-box` vs. `border-box`), margin collapse, intrinsic sizing (`min-content`, `max-content`, `fit-content`), and modern aspect-ratio controls.
- **Typography & Text Formatting**: Architect responsive typography using system font stacks, `@font-face` web fonts, optical sizing, fluid sizing via `clamp()`, and text manipulation properties.
- **Colors, Gradients, & Backgrounds**: Implement modern color models (HEX, RGB, HSL), opacity channels, multi-layer backgrounds, linear/radial/conic gradients, and blend modes (`background-blend-mode`).
- **Borders, Shadows, & Visual Effects**: Construct modern elevation shadows (`box-shadow`), accessible outline rings (`outline-offset`), glassmorphic frosted glass (`backdrop-filter`), graphic filters, and geometric `clip-path` shapes.
- **Display & Positioning Systems**: Control normal flow and out-of-flow elements using `block`, `inline`, `inline-block`, `position` (`relative`, `absolute`, `fixed`, `sticky`), and stacking contexts (`z-index`).
- **Flexbox 1-Dimensional Layouts**: Master flexible layouts, main/cross axes, alignment (`justify-content`, `align-items`), flexible sizing (`flex-grow`, `flex-shrink`, `flex-basis`), gap spacing, and fluid UI patterns.
- **CSS Grid 2-Dimensional Layouts**: Architect two-dimensional grid systems using `grid-template-columns`/`rows`, named template areas, flexible fractional units (`fr`), `minmax()`, `repeat()`, and auto-placement (`auto-fill`/`auto-fit`).
- **Responsive Web Design & Adaptability**: Engineer mobile-first and desktop-first layouts using `@media` range syntax, orientation queries, hover/pointer capabilities, dark/light color schemes (`prefers-color-scheme`), reduced motion, and container queries (`@container`).
- **Pseudo-classes & Pseudo-elements**: Enhance user interaction with dynamic pseudo-classes (`:hover`, `:focus-visible`, `:has()`, `:is()`, `:where()`, `:not()`, `:nth-child()`) and generated pseudo-elements (`::before`, `::after`, `::marker`).
- **Transforms, Transitions, & Animations**: Create GPU-accelerated 2D/3D transformations, smooth state transitions, and keyframe-driven timeline animations (`@keyframes`) with easing curves.
- **Custom Properties & Calculations**: Design scalable design systems using CSS Variables (`--custom-property`), scoped tokens, mathematical expressions (`calc()`, `min()`, `max()`, `clamp()`), modern color functions (`color-mix()`, `light-dark()`), and CSS counters.
- **Modern Living Standard Features**: Utilize emerging CSS specifications including native CSS Nesting, `@scope` style encapsulation, `@property` typed Houdini variables, and native scroll snap behaviors.
- **Accessible Form & Component Styling**: Craft custom accessible form controls, input focus rings, validation indicators (`:valid`, `:invalid`), responsive data tables, custom scrollbars, and native disclosure widgets (`details`/`summary`).
- **Architecture, Clean Code, & Best Practices**: Adopt scalable styling methodologies including CSS Reset, CSS Normalize, BEM naming conventions, utility classes, and modular file organization.
- **Full-Scale Capstone Projects**: Synthesize frontend competencies into 5 complete real-world projects: User Profile Card, Responsive Portfolio, Grid Dashboard, E-Commerce Storefront, and Full Modern Landing Page.

## Learning Roadmap

The curriculum follows a structured pedagogical trajectory progressing from foundational syntax to advanced web engineering architectures:

| Module | Title | Level | Topics | Primary Focus |
| :--- | :--- | :--- | :---: | :--- |
| [01. Introduction to CSS and Basic Syntax](#module-01-introduction-to-css-and-basic-syntax) | Introduction to CSS and Basic Syntax | `Fundamental` | 15 (1–15) | Covers foundational CSS syntax, rulesets, declarations, inline/internal/external integration, comments, whitespace, units, color values, and user-agent stylesheets. |
| [02. CSS Selectors](#module-02-css-selectors) | CSS Selectors | `Fundamental` | 20 (16–35) | Explores universal, type, class, and ID selectors, combinators (child, descendant, adjacent/general sibling), attribute matching, selector combinations, and selector lists. |
| [03. Cascade, Specificity, and Inheritance](#module-03-cascade-specificity-and-inheritance) | Cascade, Specificity, and Inheritance | `Fundamental to Intermediate` | 15 (36–50) | Examines cascade algorithms, specificity weighting calculation, source order, inheritance behavior, value keywords (`inherit`, `initial`, `unset`, `revert`), `!important`, and cascade layers (`@layer`). |
| [04. CSS Box Model](#module-04-css-box-model) | CSS Box Model | `Fundamental to Intermediate` | 20 (51–70) | Dissects concentric box layers (content, padding, border, margin), `box-sizing` (`content-box` vs `border-box`), min/max constraints, margin collapsing, centering with `margin: auto`, logical properties, intrinsic sizing, and aspect ratios. |
| [05. Typography and Text Formatting](#module-05-typography-and-text-formatting) | Typography and Text Formatting | `Fundamental to Intermediate` | 20 (71–90) | Covers font families, fallback stacks, font sizes, weights, styles, line heights, text alignments, decorations, transforms, spacing, shadows, overflow ellipsis truncation, and web fonts with `@font-face`. |
| [06. Colors and Backgrounds](#module-06-colors-and-backgrounds) | Colors and Backgrounds | `Fundamental to Intermediate` | 20 (91–110) | Examines named colors, hexadecimal, `rgb()`, `hsl()`, alpha channels, background images, repeat, positioning, sizing (`cover`/`contain`), multi-backgrounds, linear/radial/conic gradients, blend modes, clipping, and origins. |
| [07. Borders, Outlines, Shadows, and Visual Effects](#module-07-borders-outlines-shadows-and-visual-effects) | Borders, Outlines, Shadows, and Visual Effects | `Intermediate` | 15 (111–125) | Explores border properties, widths, styles, rounded corners (`border-radius`), outlines, outline offsets, elevation drop shadows (`box-shadow`), opacity, graphical filters, backdrop filters (glassmorphism), and clip paths. |
| [08. Display, Positioning, and Overflow](#module-08-display-positioning-and-overflow) | Display, Positioning, and Overflow | `Intermediate` | 20 (126–145) | Covers display modes (`block`, `inline`, `inline-block`, `none`), visibility, positioning schemes (`static`, `relative`, `absolute`, `fixed`, `sticky`), physical and logical insets, `z-index` stacking contexts, overflow modes, and `object-fit`. |
| [09. Flexbox Layout](#module-09-flexbox-layout) | Flexbox Layout | `Intermediate` | 20 (146–165) | Explores one-dimensional flex containers, flex direction, wrapping, flow, main-axis distribution (`justify-content`), cross-axis alignment (`align-items`), flexible sizing (`grow`, `shrink`, `basis`), ordering, gap, and responsive patterns. |
| [10. CSS Grid Layout](#module-10-css-grid-layout) | CSS Grid Layout | `Intermediate to Advanced` | 20 (166–185) | Dissects two-dimensional grid containers, column/row track definition, named grid areas, line placement, gap, implicit flow, auto-fit/auto-fill, `minmax()`, `repeat()`, fractional units (`fr`), alignments, and dashboard layouts. |
| [11. Responsive Web Design](#module-11-responsive-web-design) | Responsive Web Design | `Intermediate to Advanced` | 20 (186–205) | Examines `@media` queries, mobile-first and desktop-first strategies, fluid layouts, fluid typography with `clamp()`, responsive images/navigation, orientation, hover/pointer capabilities, dark mode, reduced motion, and container queries (`@container`). |
| [12. Pseudo-classes and Pseudo-elements](#module-12-pseudo-classes-and-pseudo-elements) | Pseudo-classes and Pseudo-elements | `Intermediate to Advanced` | 20 (206–225) | Covers interaction states (`:hover`, `:active`, `:focus`, `:focus-visible`, `:focus-within`), tree-structural selectors (`:nth-child`, `:nth-of-type`), logical selectors (`:not`, `:is`, `:where`, `:has`), form states, and generated content (`::before`, `::after`, `::marker`). |
| [13. Transforms, Transitions, and Animations](#module-13-transforms-transitions-and-animations) | Transforms, Transitions, and Animations | `Intermediate to Advanced` | 20 (226–245) | Explores 2D geometric transforms (`translate`, `rotate`, `scale`, `skew`), 3D transforms, perspective, `preserve-3d`, backface visibility, smooth state transitions (timing, delays, easing curves), and `@keyframes` timeline animations. |
| [14. CSS Variables, Functions, and Calculations](#module-14-css-variables-functions-and-calculations) | CSS Variables, Functions, and Calculations | `Advanced` | 20 (246–265) | Covers CSS custom properties, global/local scoping, `var()`, arithmetic with `calc()`, `min()`, `max()`, `clamp()`, `color-mix()`, relative color syntax, `light-dark()`, CSS counters, design tokens, and modular theming systems. |
| [15. At-Rules and Modern CSS Features](#module-15-at-rules-and-modern-css-features) | At-Rules and Modern CSS Features | `Advanced` | 15 (266–280) | Examines `@media`, `@supports` feature queries, `@import`, `@font-face`, `@keyframes`, `@layer` cascades, `@container` queries, `@scope` style boundaries, Houdini `@property`, native CSS Nesting, and scroll snap mechanics. |
| [16. Forms, Tables, and Component Styling](#module-16-forms-tables-and-component-styling) | Forms, Tables, and Component Styling | `Advanced` | 10 (281–290) | Covers form input styling, accessible focus states, visual validation (`:valid`/`:invalid`), custom checkboxes/radios, button component variants, data table styling, zebra striping, responsive tables, custom scrollbars, and native accordions. |
| [17. CSS Architecture, Debugging, and Best Practices](#module-17-css-architecture-debugging-and-best-practices) | CSS Architecture, Debugging, and Best Practices | `Advanced` | 5 (291–295) | Explores universal CSS reset strategies, cross-browser normalization, BEM naming methodology, utility-first atomic classes, and modular directory architectures (ITCSS and 7-1 pattern). |
| [18. Practical Capstone CSS Projects](#module-18-practical-capstone-css-projects) | Practical Capstone CSS Projects | `Capstone / Practical` | 5 (296–300) | Synthesizes curriculum concepts into 5 complete real-world projects: User Profile Card, Responsive Developer Portfolio, Interactive Dashboard, E-Commerce Storefront, and Full Corporate Landing Page. |

## Prerequisites

Before starting with the curriculum, ensure your local development environment meets the following baseline requirements:

- **Prior Knowledge**: Basic familiarity with HTML document structure and web browser navigation is recommended. The curriculum starts with fundamental styling syntax and progressively advances to professional architectures.
- **Modern Web Browser**: Any modern web browser with full support for CSS3 and contemporary Web Standards:
  - **Google Chrome** (v90 or higher)
  - **Mozilla Firefox** (v88 or higher)
  - **Microsoft Edge** (v90 or higher)
  - **Apple Safari** (v15 or higher)
- **Text Editor or IDE**: Any code editor supporting CSS syntax highlighting, linting, and formatting (e.g., [Visual Studio Code](https://code.visualstudio.com/), [Sublime Text](https://www.sublimetext.com/), or [WebStorm](https://www.jetbrains.com/webstorm/)).
- **Local HTTP Server (Recommended)**: While HTML and CSS files can be previewed directly via the filesystem (`file://`), serving them over HTTP is strongly recommended for testing web fonts (`@font-face`), modular imports (`@import`), and modern features. Options include the VS Code Live Server extension, Node.js (`npx serve`), or Python (`python -m http.server`).

## Tech Stack & Tools

- **Core Styling Technology**: CSS3 / W3C & WHATWG CSS Living Standard
- **Core Markup Language**: HTML5 (W3C Recommendation)
- **Layout Specifications**: CSS Box Model Module Level 4, CSS Flexible Box Layout Module Level 1, CSS Grid Layout Module Level 2
- **Responsive & Adaptive Standards**: Media Queries Level 5, CSS Container Queries Level 1
- **Visual Effects & Motion**: CSS Transforms Module Level 2, CSS Transitions Module Level 2, CSS Animations Level 1, Filter Effects Module Level 1
- **Programmable & Modern CSS**: CSS Custom Properties for Cascading Variables Module Level 1, CSS Values and Units Module Level 4 (`calc()`, `min()`, `max()`, `clamp()`), CSS Houdini Properties & Values API Level 1 (`@property`), CSS Cascading and Inheritance Level 5 (`@layer`)
- **Inspection & Development Tools**: Browser Developer Tools (Elements inspector, Computed styles panel, Box Model visualizer, Flexbox/Grid layout overlays, Animation timelines)
- **Local Development Servers**: Python `http.server`, Node.js `serve`, VS Code Live Server

## Getting Started

Follow these steps to clone the repository and explore the learning modules locally:

### 1. Clone the Repository

```bash
git clone https://github.com/weztcy/CSS-Learning-Modules.git
cd CSS-Learning-Modules
```

### 2. Previewing Lessons in Your Browser

You can inspect and execute any lesson using one of the following methods:

#### Method A: Direct File Execution

Open any lesson preview HTML file directly from your terminal or file manager:

```bash
# Windows
start "" "module-01-pengenalan-css-dan-sintaks-dasar/01_css_basic_syntax.html"

# macOS
open module-01-pengenalan-css-dan-sintaks-dasar/01_css_basic_syntax.html

# Linux
xdg-open module-01-pengenalan-css-dan-sintaks-dasar/01_css_basic_syntax.html
```

#### Method B: VS Code Live Server Extension (Recommended)

1. Open the cloned `CSS Learning Modules` folder in Visual Studio Code.
2. Install the **Live Server** extension (`ritwickdey.liveserver`).
3. Right-click on any `.html` preview file and select **Open with Live Server** to view the live rendering with instant reload upon modifying the paired `.css` stylesheet.

#### Method C: Python Built-In HTTP Server

If you have Python installed, launch a local web server from the repository root:

```bash
python -m http.server 8080
```

Then navigate to `http://localhost:8080` in your web browser.

#### Method D: Node.js Serve

If Node.js is installed, spin up a lightweight local server via npx:

```bash
npx serve .
```

## How to Use This Repository

To maximize your learning effectiveness, follow this structured study workflow:

1. **Select a Module**: Review the [Learning Roadmap](#learning-roadmap) and choose a topic aligned with your current learning objectives.
2. **Study the Architecture**: Read the module overview and subtopic descriptions to grasp the underlying browser layout engine mechanics, cascade rules, and rendering behaviors.
3. **Inspect the Stylesheet Source**: Open the linked `.css` file in your code editor to examine selector specificity, property declarations, and architectural commenting. Inspect the paired `.html` file to see how markup is structured.
4. **Render in Browser**: Launch the `.html` file in your browser to observe the visual styling in action.
5. **Compare with Output Captures**: Compare your browser's rendered display against the verified output screenshot located in that subtopic's `output/` directory.
6. **Experiment and Modify**: Experiment by altering properties, modifying values, testing layout edge cases in Developer Tools, and completing the capstone projects in Module 18.

## Learning Modules & Subtopics

Below is the structured overview of all learning modules and their respective subtopics with direct repository links. Detailed explanations, run instructions, and execution captures are documented within the dedicated `README.md` in each module directory.

### Module 01: Introduction to CSS and Basic Syntax

**Curriculum Path**: [`module-01-pengenalan-css-dan-sintaks-dasar`](./module-01-pengenalan-css-dan-sintaks-dasar) | **Level**: `Fundamental` | **Scope**: 15 Lessons

#### Overview & Concepts Covered

Covers foundational Cascading Style Sheets (CSS) principles, including basic syntax structure, ruleset anatomy, declaration blocks, properties and values, the three CSS implementation methods (inline, internal, and external stylesheets), educational code commenting, whitespace handling, case sensitivity rules, value units (px, rem, em, %), color notation systems, and the default user-agent styles applied by web browsers.

#### Subtopics

- [`01_css_basic_syntax.css`](./module-01-pengenalan-css-dan-sintaks-dasar/01_css_basic_syntax.css) — Basic CSS Syntax ([Preview HTML](./module-01-pengenalan-css-dan-sintaks-dasar/01_css_basic_syntax.html))
- [`02_css_ruleset.css`](./module-01-pengenalan-css-dan-sintaks-dasar/02_css_ruleset.css) — CSS Ruleset Anatomy ([Preview HTML](./module-01-pengenalan-css-dan-sintaks-dasar/02_css_ruleset.html))
- [`03_css_selectors_intro.css`](./module-01-pengenalan-css-dan-sintaks-dasar/03_css_selectors_intro.css) — Introduction to Selectors ([Preview HTML](./module-01-pengenalan-css-dan-sintaks-dasar/03_css_selectors_intro.html))
- [`04_css_declarations.css`](./module-01-pengenalan-css-dan-sintaks-dasar/04_css_declarations.css) — CSS Declarations ([Preview HTML](./module-01-pengenalan-css-dan-sintaks-dasar/04_css_declarations.html))
- [`05_css_properties_values.css`](./module-01-pengenalan-css-dan-sintaks-dasar/05_css_properties_values.css) — Properties and Values ([Preview HTML](./module-01-pengenalan-css-dan-sintaks-dasar/05_css_properties_values.html))
- [`06_inline_css.css`](./module-01-pengenalan-css-dan-sintaks-dasar/06_inline_css.css) — Inline CSS Styling ([Preview HTML](./module-01-pengenalan-css-dan-sintaks-dasar/06_inline_css.html))
- [`07_internal_css.css`](./module-01-pengenalan-css-dan-sintaks-dasar/07_internal_css.css) — Internal CSS Stylesheets ([Preview HTML](./module-01-pengenalan-css-dan-sintaks-dasar/07_internal_css.html))
- [`08_external_css.css`](./module-01-pengenalan-css-dan-sintaks-dasar/08_external_css.css) — External CSS Stylesheets ([Preview HTML](./module-01-pengenalan-css-dan-sintaks-dasar/08_external_css.html))
- [`09_css_comments.css`](./module-01-pengenalan-css-dan-sintaks-dasar/09_css_comments.css) — CSS Comments ([Preview HTML](./module-01-pengenalan-css-dan-sintaks-dasar/09_css_comments.html))
- [`10_css_multiple_declarations.css`](./module-01-pengenalan-css-dan-sintaks-dasar/10_css_multiple_declarations.css) — Multiple Declarations ([Preview HTML](./module-01-pengenalan-css-dan-sintaks-dasar/10_css_multiple_declarations.html))
- [`11_css_whitespace.css`](./module-01-pengenalan-css-dan-sintaks-dasar/11_css_whitespace.css) — Whitespace in CSS ([Preview HTML](./module-01-pengenalan-css-dan-sintaks-dasar/11_css_whitespace.html))
- [`12_css_case_sensitivity.css`](./module-01-pengenalan-css-dan-sintaks-dasar/12_css_case_sensitivity.css) — CSS Case Sensitivity ([Preview HTML](./module-01-pengenalan-css-dan-sintaks-dasar/12_css_case_sensitivity.html))
- [`13_css_property_units.css`](./module-01-pengenalan-css-dan-sintaks-dasar/13_css_property_units.css) — CSS Units and Values ([Preview HTML](./module-01-pengenalan-css-dan-sintaks-dasar/13_css_property_units.html))
- [`14_css_color_values.css`](./module-01-pengenalan-css-dan-sintaks-dasar/14_css_color_values.css) — Color Value Formats ([Preview HTML](./module-01-pengenalan-css-dan-sintaks-dasar/14_css_color_values.html))
- [`15_css_browser_defaults.css`](./module-01-pengenalan-css-dan-sintaks-dasar/15_css_browser_defaults.css) — Browser Default User-Agent Styles ([Preview HTML](./module-01-pengenalan-css-dan-sintaks-dasar/15_css_browser_defaults.html))

### Module 02: CSS Selectors

**Curriculum Path**: [`module-02-css-selectors`](./module-02-css-selectors) | **Level**: `Fundamental` | **Scope**: 20 Lessons

#### Overview & Concepts Covered

Provides a comprehensive examination of CSS selectors and combinators: the universal selector (`*`), type/element selectors, class selectors, ID selectors, grouping selectors, combinators (descendant, child `>`, adjacent sibling `+`, general sibling `~`), the attribute selector family (presence `[attr]`, exact match `=`, substring `*=`, prefix `^=`, suffix `$=`, space-separated word `~=`, hyphenated `|=`), selector combinations, complex compound selectors, and selector list patterns.

#### Subtopics

- [`16_universal_selector.css`](./module-02-css-selectors/16_universal_selector.css) — Universal Selector ([Preview HTML](./module-02-css-selectors/16_universal_selector.html))
- [`17_element_selector.css`](./module-02-css-selectors/17_element_selector.css) — Element / Type Selector ([Preview HTML](./module-02-css-selectors/17_element_selector.html))
- [`18_class_selector.css`](./module-02-css-selectors/18_class_selector.css) — Class Selector ([Preview HTML](./module-02-css-selectors/18_class_selector.html))
- [`19_id_selector.css`](./module-02-css-selectors/19_id_selector.css) — ID Selector ([Preview HTML](./module-02-css-selectors/19_id_selector.html))
- [`20_grouping_selector.css`](./module-02-css-selectors/20_grouping_selector.css) — Grouping Selector ([Preview HTML](./module-02-css-selectors/20_grouping_selector.html))
- [`21_descendant_selector.css`](./module-02-css-selectors/21_descendant_selector.css) — Descendant Combinator ([Preview HTML](./module-02-css-selectors/21_descendant_selector.html))
- [`22_child_selector.css`](./module-02-css-selectors/22_child_selector.css) — Child Combinator ([Preview HTML](./module-02-css-selectors/22_child_selector.html))
- [`23_adjacent_sibling_selector.css`](./module-02-css-selectors/23_adjacent_sibling_selector.css) — Adjacent Sibling Combinator ([Preview HTML](./module-02-css-selectors/23_adjacent_sibling_selector.html))
- [`24_general_sibling_selector.css`](./module-02-css-selectors/24_general_sibling_selector.css) — General Sibling Combinator ([Preview HTML](./module-02-css-selectors/24_general_sibling_selector.html))
- [`25_attribute_selector.css`](./module-02-css-selectors/25_attribute_selector.css) — Attribute Presence Selector ([Preview HTML](./module-02-css-selectors/25_attribute_selector.html))
- [`26_attribute_exact_match.css`](./module-02-css-selectors/26_attribute_exact_match.css) — Exact Attribute Matching ([Preview HTML](./module-02-css-selectors/26_attribute_exact_match.html))
- [`27_attribute_contains.css`](./module-02-css-selectors/27_attribute_contains.css) — Attribute Substring Matching ([Preview HTML](./module-02-css-selectors/27_attribute_contains.html))
- [`28_attribute_prefix.css`](./module-02-css-selectors/28_attribute_prefix.css) — Attribute Prefix Matching ([Preview HTML](./module-02-css-selectors/28_attribute_prefix.html))
- [`29_attribute_suffix.css`](./module-02-css-selectors/29_attribute_suffix.css) — Attribute Suffix Matching ([Preview HTML](./module-02-css-selectors/29_attribute_suffix.html))
- [`30_attribute_word_match.css`](./module-02-css-selectors/30_attribute_word_match.css) — Attribute Word Matching ([Preview HTML](./module-02-css-selectors/30_attribute_word_match.html))
- [`31_attribute_hyphen_match.css`](./module-02-css-selectors/31_attribute_hyphen_match.css) — Attribute Hyphen Matching ([Preview HTML](./module-02-css-selectors/31_attribute_hyphen_match.html))
- [`32_selector_combinations.css`](./module-02-css-selectors/32_selector_combinations.css) — Selector Combinations ([Preview HTML](./module-02-css-selectors/32_selector_combinations.html))
- [`33_multiple_class_selectors.css`](./module-02-css-selectors/33_multiple_class_selectors.css) — Multiple Class Selectors ([Preview HTML](./module-02-css-selectors/33_multiple_class_selectors.html))
- [`34_complex_selectors.css`](./module-02-css-selectors/34_complex_selectors.css) — Complex Selectors ([Preview HTML](./module-02-css-selectors/34_complex_selectors.html))
- [`35_selector_list_patterns.css`](./module-02-css-selectors/35_selector_list_patterns.css) — Selector List Patterns ([Preview HTML](./module-02-css-selectors/35_selector_list_patterns.html))

### Module 03: Cascade, Specificity, and Inheritance

**Curriculum Path**: [`module-03-cascade-specificity-dan-inheritance`](./module-03-cascade-specificity-dan-inheritance) | **Level**: `Fundamental to Intermediate` | **Scope**: 15 Lessons

#### Overview & Concepts Covered

Explores the core rendering engine algorithms governing CSS: the Cascade (rule precedence and conflict resolution), Specificity calculations (inline styles > IDs > classes/attributes/pseudo-classes > type selectors), source order determination, CSS Inheritance (property propagation from parent to child), inherited versus non-inherited properties, universal value keywords (`initial`, `inherit`, `unset`, `revert`, `revert-layer`), safe usage and architectural risks of `!important`, and modern Cascade Layers (`@layer`).

#### Subtopics

- [`36_css_cascade.css`](./module-03-cascade-specificity-dan-inheritance/36_css_cascade.css) — The CSS Cascade Algorithm ([Preview HTML](./module-03-cascade-specificity-dan-inheritance/36_css_cascade.html))
- [`37_selector_specificity.css`](./module-03-cascade-specificity-dan-inheritance/37_selector_specificity.css) — Selector Specificity ([Preview HTML](./module-03-cascade-specificity-dan-inheritance/37_selector_specificity.html))
- [`38_specificity_comparison.css`](./module-03-cascade-specificity-dan-inheritance/38_specificity_comparison.css) — Specificity Comparison and Weighting ([Preview HTML](./module-03-cascade-specificity-dan-inheritance/38_specificity_comparison.html))
- [`39_source_order.css`](./module-03-cascade-specificity-dan-inheritance/39_source_order.css) — Source Order and Rule Precedence ([Preview HTML](./module-03-cascade-specificity-dan-inheritance/39_source_order.html))
- [`40_css_inheritance.css`](./module-03-cascade-specificity-dan-inheritance/40_css_inheritance.css) — CSS Inheritance ([Preview HTML](./module-03-cascade-specificity-dan-inheritance/40_css_inheritance.html))
- [`41_inherited_properties.css`](./module-03-cascade-specificity-dan-inheritance/41_inherited_properties.css) — Inherited Properties ([Preview HTML](./module-03-cascade-specificity-dan-inheritance/41_inherited_properties.html))
- [`42_non_inherited_properties.css`](./module-03-cascade-specificity-dan-inheritance/42_non_inherited_properties.css) — Non-Inherited Properties ([Preview HTML](./module-03-cascade-specificity-dan-inheritance/42_non_inherited_properties.html))
- [`43_initial_value.css`](./module-03-cascade-specificity-dan-inheritance/43_initial_value.css) — The `initial` Keyword ([Preview HTML](./module-03-cascade-specificity-dan-inheritance/43_initial_value.html))
- [`44_inherit_keyword.css`](./module-03-cascade-specificity-dan-inheritance/44_inherit_keyword.css) — The `inherit` Keyword ([Preview HTML](./module-03-cascade-specificity-dan-inheritance/44_inherit_keyword.html))
- [`45_unset_keyword.css`](./module-03-cascade-specificity-dan-inheritance/45_unset_keyword.css) — The `unset` Keyword ([Preview HTML](./module-03-cascade-specificity-dan-inheritance/45_unset_keyword.html))
- [`46_revert_keyword.css`](./module-03-cascade-specificity-dan-inheritance/46_revert_keyword.css) — The `revert` Keyword ([Preview HTML](./module-03-cascade-specificity-dan-inheritance/46_revert_keyword.html))
- [`47_revert_layer.css`](./module-03-cascade-specificity-dan-inheritance/47_revert_layer.css) — The `revert-layer` Keyword ([Preview HTML](./module-03-cascade-specificity-dan-inheritance/47_revert_layer.html))
- [`48_important_declaration.css`](./module-03-cascade-specificity-dan-inheritance/48_important_declaration.css) — The `!important` Declaration ([Preview HTML](./module-03-cascade-specificity-dan-inheritance/48_important_declaration.html))
- [`49_cascade_layers_intro.css`](./module-03-cascade-specificity-dan-inheritance/49_cascade_layers_intro.css) — Introduction to Cascade Layers (`@layer`) ([Preview HTML](./module-03-cascade-specificity-dan-inheritance/49_cascade_layers_intro.html))
- [`50_cascade_conflict_resolution.css`](./module-03-cascade-specificity-dan-inheritance/50_cascade_conflict_resolution.css) — CSS Cascade Conflict Resolution ([Preview HTML](./module-03-cascade-specificity-dan-inheritance/50_cascade_conflict_resolution.html))

### Module 04: CSS Box Model

**Curriculum Path**: [`module-04-css-box-model`](./module-04-css-box-model) | **Level**: `Fundamental to Intermediate` | **Scope**: 20 Lessons

#### Overview & Concepts Covered

Dissects the core structural layout model of CSS: the Box Model. Topics include the four concentric box layers (content, padding, border, and margin), fundamental differences between `content-box` and `border-box`, explicit dimensions and bounding constraints (`min-width`, `max-width`, `min-height`, `max-height`), margin collapsing mechanics, horizontal centering via `margin: auto`, modern logical properties (`margin-inline`, `padding-block`), global box-sizing resets, intrinsic sizing keywords (`min-content`, `max-content`, `fit-content()`), and the `aspect-ratio` property.

#### Subtopics

- [`51_box_model_basic.css`](./module-04-css-box-model/51_box_model_basic.css) — CSS Box Model Fundamentals ([Preview HTML](./module-04-css-box-model/51_box_model_basic.html))
- [`52_content_box.css`](./module-04-css-box-model/52_content_box.css) — `box-sizing: content-box` ([Preview HTML](./module-04-css-box-model/52_content_box.html))
- [`53_border_box.css`](./module-04-css-box-model/53_border_box.css) — `box-sizing: border-box` ([Preview HTML](./module-04-css-box-model/53_border_box.html))
- [`54_width_property.css`](./module-04-css-box-model/54_width_property.css) — The `width` Property ([Preview HTML](./module-04-css-box-model/54_width_property.html))
- [`55_height_property.css`](./module-04-css-box-model/55_height_property.css) — The `height` Property ([Preview HTML](./module-04-css-box-model/55_height_property.html))
- [`56_min_width.css`](./module-04-css-box-model/56_min_width.css) — The `min-width` Property ([Preview HTML](./module-04-css-box-model/56_min_width.html))
- [`57_max_width.css`](./module-04-css-box-model/57_max_width.css) — The `max-width` Property ([Preview HTML](./module-04-css-box-model/57_max_width.html))
- [`58_min_height.css`](./module-04-css-box-model/58_min_height.css) — The `min-height` Property ([Preview HTML](./module-04-css-box-model/58_min_height.html))
- [`59_max_height.css`](./module-04-css-box-model/59_max_height.css) — The `max-height` Property ([Preview HTML](./module-04-css-box-model/59_max_height.html))
- [`60_margin_property.css`](./module-04-css-box-model/60_margin_property.css) — The `margin` Property ([Preview HTML](./module-04-css-box-model/60_margin_property.html))
- [`61_margin_collapse.css`](./module-04-css-box-model/61_margin_collapse.css) — Margin Collapsing Mechanics ([Preview HTML](./module-04-css-box-model/61_margin_collapse.html))
- [`62_padding_property.css`](./module-04-css-box-model/62_padding_property.css) — The `padding` Property ([Preview HTML](./module-04-css-box-model/62_padding_property.html))
- [`63_margin_auto.css`](./module-04-css-box-model/63_margin_auto.css) — Centering Elements with `margin: auto` ([Preview HTML](./module-04-css-box-model/63_margin_auto.html))
- [`64_logical_margin.css`](./module-04-css-box-model/64_logical_margin.css) — Logical Margin Properties ([Preview HTML](./module-04-css-box-model/64_logical_margin.html))
- [`65_logical_padding.css`](./module-04-css-box-model/65_logical_padding.css) — Logical Padding Properties ([Preview HTML](./module-04-css-box-model/65_logical_padding.html))
- [`66_box_sizing_global.css`](./module-04-css-box-model/66_box_sizing_global.css) — Global Box-Sizing Reset ([Preview HTML](./module-04-css-box-model/66_box_sizing_global.html))
- [`67_intrinsic_sizing.css`](./module-04-css-box-model/67_intrinsic_sizing.css) — Intrinsic Sizing Keywords ([Preview HTML](./module-04-css-box-model/67_intrinsic_sizing.html))
- [`68_min_content_max_content.css`](./module-04-css-box-model/68_min_content_max_content.css) — `min-content` and `max-content` ([Preview HTML](./module-04-css-box-model/68_min_content_max_content.html))
- [`69_fit_content.css`](./module-04-css-box-model/69_fit_content.css) — The `fit-content()` Function ([Preview HTML](./module-04-css-box-model/69_fit_content.html))
- [`70_aspect_ratio.css`](./module-04-css-box-model/70_aspect_ratio.css) — The `aspect-ratio` Property ([Preview HTML](./module-04-css-box-model/70_aspect_ratio.html))

### Module 05: Typography and Text Formatting

**Curriculum Path**: [`module-05-typography-dan-pemformatan-teks`](./module-05-typography-dan-pemformatan-teks) | **Level**: `Fundamental to Intermediate` | **Scope**: 20 Lessons

#### Overview & Concepts Covered

Delves into modern web typography principles and text styling: font family definitions with resilient fallback stacks, scalable font size scaling (`rem`, `em`, `%`), numeric and keyword font weights, font styles, small-caps font variants, font stretch, the `font` shorthand, comfortable line height ratios (`line-height`), alignment controls (`text-align`), modern text decoration suites (underline offset, thickness, styling), case transformations (`text-transform`), paragraph indentation, letter and word spacing kerning, graphical text shadows, ellipsis truncation (`text-overflow`), whitespace management, and custom self-hosted web fonts via `@font-face`.

#### Subtopics

- [`71_font_family.css`](./module-05-typography-dan-pemformatan-teks/71_font_family.css) — The `font-family` Property and Fallbacks ([Preview HTML](./module-05-typography-dan-pemformatan-teks/71_font_family.html))
- [`72_font_size.css`](./module-05-typography-dan-pemformatan-teks/72_font_size.css) — The `font-size` Property and Scalable Units ([Preview HTML](./module-05-typography-dan-pemformatan-teks/72_font_size.html))
- [`73_font_weight.css`](./module-05-typography-dan-pemformatan-teks/73_font_weight.css) — The `font-weight` Property ([Preview HTML](./module-05-typography-dan-pemformatan-teks/73_font_weight.html))
- [`74_font_style.css`](./module-05-typography-dan-pemformatan-teks/74_font_style.css) — The `font-style` Property ([Preview HTML](./module-05-typography-dan-pemformatan-teks/74_font_style.html))
- [`75_font_variant.css`](./module-05-typography-dan-pemformatan-teks/75_font_variant.css) — The `font-variant` Property ([Preview HTML](./module-05-typography-dan-pemformatan-teks/75_font_variant.html))
- [`76_font_stretch.css`](./module-05-typography-dan-pemformatan-teks/76_font_stretch.css) — The `font-stretch` Property ([Preview HTML](./module-05-typography-dan-pemformatan-teks/76_font_stretch.html))
- [`77_font_shorthand.css`](./module-05-typography-dan-pemformatan-teks/77_font_shorthand.css) — The `font` Shorthand Property ([Preview HTML](./module-05-typography-dan-pemformatan-teks/77_font_shorthand.html))
- [`78_line_height.css`](./module-05-typography-dan-pemformatan-teks/78_line_height.css) — The `line-height` Property ([Preview HTML](./module-05-typography-dan-pemformatan-teks/78_line_height.html))
- [`79_text_align.css`](./module-05-typography-dan-pemformatan-teks/79_text_align.css) — The `text-align` Property ([Preview HTML](./module-05-typography-dan-pemformatan-teks/79_text_align.html))
- [`80_text_decoration.css`](./module-05-typography-dan-pemformatan-teks/80_text_decoration.css) — The `text-decoration` Property Suite ([Preview HTML](./module-05-typography-dan-pemformatan-teks/80_text_decoration.html))
- [`81_text_transform.css`](./module-05-typography-dan-pemformatan-teks/81_text_transform.css) — The `text-transform` Property ([Preview HTML](./module-05-typography-dan-pemformatan-teks/81_text_transform.html))
- [`82_text_indent.css`](./module-05-typography-dan-pemformatan-teks/82_text_indent.css) — The `text-indent` Property ([Preview HTML](./module-05-typography-dan-pemformatan-teks/82_text_indent.html))
- [`83_letter_spacing.css`](./module-05-typography-dan-pemformatan-teks/83_letter_spacing.css) — The `letter-spacing` Property ([Preview HTML](./module-05-typography-dan-pemformatan-teks/83_letter_spacing.html))
- [`84_word_spacing.css`](./module-05-typography-dan-pemformatan-teks/84_word_spacing.css) — The `word-spacing` Property ([Preview HTML](./module-05-typography-dan-pemformatan-teks/84_word_spacing.html))
- [`85_text_shadow.css`](./module-05-typography-dan-pemformatan-teks/85_text_shadow.css) — The `text-shadow` Property ([Preview HTML](./module-05-typography-dan-pemformatan-teks/85_text_shadow.html))
- [`86_text_overflow.css`](./module-05-typography-dan-pemformatan-teks/86_text_overflow.css) — The `text-overflow` Property and Ellipsis Truncation ([Preview HTML](./module-05-typography-dan-pemformatan-teks/86_text_overflow.html))
- [`87_white_space.css`](./module-05-typography-dan-pemformatan-teks/87_white_space.css) — The `white-space` Property ([Preview HTML](./module-05-typography-dan-pemformatan-teks/87_white_space.html))
- [`88_word_break.css`](./module-05-typography-dan-pemformatan-teks/88_word_break.css) — The `word-break` Property ([Preview HTML](./module-05-typography-dan-pemformatan-teks/88_word_break.html))
- [`89_overflow_wrap.css`](./module-05-typography-dan-pemformatan-teks/89_overflow_wrap.css) — The `overflow-wrap` Property ([Preview HTML](./module-05-typography-dan-pemformatan-teks/89_overflow_wrap.html))
- [`90_web_fonts.css`](./module-05-typography-dan-pemformatan-teks/90_web_fonts.css) — Custom Web Fonts with `@font-face` ([Preview HTML](./module-05-typography-dan-pemformatan-teks/90_web_fonts.html))

### Module 06: Colors and Backgrounds

**Curriculum Path**: [`module-06-warna-dan-background`](./module-06-warna-dan-background) | **Level**: `Fundamental to Intermediate` | **Scope**: 20 Lessons

#### Overview & Concepts Covered

Presents an in-depth guide to color theory, notations, and background rendering in CSS: official named color keywords, 3/6/8-digit hexadecimal notations, modern comma-free `rgb()` and `hsl()` functional syntax, alpha transparency management, foreground text and background colors, background image handling (`image`, `repeat`, `position`, `size: cover/contain`, `attachment: fixed/scroll`), shorthand definitions, multi-layer composite backgrounds, CSS gradients (linear, radial, and conic gradients with color stops), layer blending modes (`background-blend-mode`), and background clipping (`background-clip`) and positioning origin (`background-origin`).

#### Subtopics

- [`91_named_colors.css`](./module-06-warna-dan-background/91_named_colors.css) — CSS Named Colors ([Preview HTML](./module-06-warna-dan-background/91_named_colors.html))
- [`92_hex_colors.css`](./module-06-warna-dan-background/92_hex_colors.css) — Hexadecimal Color Notation ([Preview HTML](./module-06-warna-dan-background/92_hex_colors.html))
- [`93_rgb_colors.css`](./module-06-warna-dan-background/93_rgb_colors.css) — The `rgb()` Functional Notation ([Preview HTML](./module-06-warna-dan-background/93_rgb_colors.html))
- [`94_hsl_colors.css`](./module-06-warna-dan-background/94_hsl_colors.css) — The `hsl()` Functional Notation ([Preview HTML](./module-06-warna-dan-background/94_hsl_colors.html))
- [`95_alpha_colors.css`](./module-06-warna-dan-background/95_alpha_colors.css) — Color Alpha Channels and Transparency ([Preview HTML](./module-06-warna-dan-background/95_alpha_colors.html))
- [`96_color_property.css`](./module-06-warna-dan-background/96_color_property.css) — The `color` Property ([Preview HTML](./module-06-warna-dan-background/96_color_property.html))
- [`97_background_color.css`](./module-06-warna-dan-background/97_background_color.css) — The `background-color` Property ([Preview HTML](./module-06-warna-dan-background/97_background_color.html))
- [`98_background_image.css`](./module-06-warna-dan-background/98_background_image.css) — The `background-image` Property ([Preview HTML](./module-06-warna-dan-background/98_background_image.html))
- [`99_background_repeat.css`](./module-06-warna-dan-background/99_background_repeat.css) — The `background-repeat` Property ([Preview HTML](./module-06-warna-dan-background/99_background_repeat.html))
- [`100_background_position.css`](./module-06-warna-dan-background/100_background_position.css) — The `background-position` Property ([Preview HTML](./module-06-warna-dan-background/100_background_position.html))
- [`101_background_size.css`](./module-06-warna-dan-background/101_background_size.css) — The `background-size` Property (`cover` & `contain`) ([Preview HTML](./module-06-warna-dan-background/101_background_size.html))
- [`102_background_attachment.css`](./module-06-warna-dan-background/102_background_attachment.css) — The `background-attachment` Property ([Preview HTML](./module-06-warna-dan-background/102_background_attachment.html))
- [`103_background_shorthand.css`](./module-06-warna-dan-background/103_background_shorthand.css) — The `background` Shorthand Property ([Preview HTML](./module-06-warna-dan-background/103_background_shorthand.html))
- [`104_multiple_backgrounds.css`](./module-06-warna-dan-background/104_multiple_backgrounds.css) — Multiple Background Layers ([Preview HTML](./module-06-warna-dan-background/104_multiple_backgrounds.html))
- [`105_background_gradients.css`](./module-06-warna-dan-background/105_background_gradients.css) — Linear Gradients (`linear-gradient`) ([Preview HTML](./module-06-warna-dan-background/105_background_gradients.html))
- [`106_radial_gradient.css`](./module-06-warna-dan-background/106_radial_gradient.css) — Radial Gradients (`radial-gradient`) ([Preview HTML](./module-06-warna-dan-background/106_radial_gradient.html))
- [`107_conic_gradient.css`](./module-06-warna-dan-background/107_conic_gradient.css) — Conic Gradients (`conic-gradient`) ([Preview HTML](./module-06-warna-dan-background/107_conic_gradient.html))
- [`108_gradient_color_stops.css`](./module-06-warna-dan-background/108_gradient_color_stops.css) — Gradient Color Stops and Positioning ([Preview HTML](./module-06-warna-dan-background/108_gradient_color_stops.html))
- [`109_background_blend_mode.css`](./module-06-warna-dan-background/109_background_blend_mode.css) — The `background-blend-mode` Property ([Preview HTML](./module-06-warna-dan-background/109_background_blend_mode.html))
- [`110_background_clip_origin.css`](./module-06-warna-dan-background/110_background_clip_origin.css) — `background-clip` and `background-origin` ([Preview HTML](./module-06-warna-dan-background/110_background_clip_origin.html))

### Module 07: Borders, Outlines, Shadows, and Visual Effects

**Curriculum Path**: [`module-07-border-outline-shadow-dan-efek-visual`](./module-07-border-outline-shadow-dan-efek-visual) | **Level**: `Intermediate` | **Scope**: 15 Lessons

#### Overview & Concepts Covered

Explores element boundary styling, elevation depth, and visual graphic effects: the `border` shorthand and individual side configurations (width, styles, color, and curved corners with `border-radius`), vital distinctions between borders and accessible focus outlines (`outline` and `outline-offset`), layered realistic drop shadows (`box-shadow`), element opacity levels, CSS graphical filters (`blur`, `grayscale`, `brightness`, `drop-shadow`), glassmorphic frosted glass aesthetics using `backdrop-filter`, layer blending with `mix-blend-mode`, and geometric masking shapes via `clip-path`.

#### Subtopics

- [`111_border_property.css`](./module-07-border-outline-shadow-dan-efek-visual/111_border_property.css) — The `border` Shorthand Property ([Preview HTML](./module-07-border-outline-shadow-dan-efek-visual/111_border_property.html))
- [`112_border_width.css`](./module-07-border-outline-shadow-dan-efek-visual/112_border_width.css) — The `border-width` Property ([Preview HTML](./module-07-border-outline-shadow-dan-efek-visual/112_border_width.html))
- [`113_border_style.css`](./module-07-border-outline-shadow-dan-efek-visual/113_border_style.css) — The `border-style` Property ([Preview HTML](./module-07-border-outline-shadow-dan-efek-visual/113_border_style.html))
- [`114_border_color.css`](./module-07-border-outline-shadow-dan-efek-visual/114_border_color.css) — The `border-color` Property ([Preview HTML](./module-07-border-outline-shadow-dan-efek-visual/114_border_color.html))
- [`115_border_radius.css`](./module-07-border-outline-shadow-dan-efek-visual/115_border_radius.css) — The `border-radius` Property and Rounded Corners ([Preview HTML](./module-07-border-outline-shadow-dan-efek-visual/115_border_radius.html))
- [`116_individual_borders.css`](./module-07-border-outline-shadow-dan-efek-visual/116_individual_borders.css) — Individual Side Border Properties ([Preview HTML](./module-07-border-outline-shadow-dan-efek-visual/116_individual_borders.html))
- [`117_outline_property.css`](./module-07-border-outline-shadow-dan-efek-visual/117_outline_property.css) — The `outline` Property ([Preview HTML](./module-07-border-outline-shadow-dan-efek-visual/117_outline_property.html))
- [`118_outline_offset.css`](./module-07-border-outline-shadow-dan-efek-visual/118_outline_offset.css) — The `outline-offset` Property ([Preview HTML](./module-07-border-outline-shadow-dan-efek-visual/118_outline_offset.html))
- [`119_box_shadow.css`](./module-07-border-outline-shadow-dan-efek-visual/119_box_shadow.css) — The `box-shadow` Property and Elevation ([Preview HTML](./module-07-border-outline-shadow-dan-efek-visual/119_box_shadow.html))
- [`120_multiple_box_shadows.css`](./module-07-border-outline-shadow-dan-efek-visual/120_multiple_box_shadows.css) — Multiple Layered Box Shadows ([Preview HTML](./module-07-border-outline-shadow-dan-efek-visual/120_multiple_box_shadows.html))
- [`121_opacity_property.css`](./module-07-border-outline-shadow-dan-efek-visual/121_opacity_property.css) — The `opacity` Property ([Preview HTML](./module-07-border-outline-shadow-dan-efek-visual/121_opacity_property.html))
- [`122_filter_property.css`](./module-07-border-outline-shadow-dan-efek-visual/122_filter_property.css) — The `filter` Property and Graphical Effects ([Preview HTML](./module-07-border-outline-shadow-dan-efek-visual/122_filter_property.html))
- [`123_backdrop_filter.css`](./module-07-border-outline-shadow-dan-efek-visual/123_backdrop_filter.css) — The `backdrop-filter` Property (Glassmorphism) ([Preview HTML](./module-07-border-outline-shadow-dan-efek-visual/123_backdrop_filter.html))
- [`124_mix_blend_mode.css`](./module-07-border-outline-shadow-dan-efek-visual/124_mix_blend_mode.css) — The `mix-blend-mode` Property ([Preview HTML](./module-07-border-outline-shadow-dan-efek-visual/124_mix_blend_mode.html))
- [`125_clip_path.css`](./module-07-border-outline-shadow-dan-efek-visual/125_clip_path.css) — The `clip-path` Property and Geometric Masking ([Preview HTML](./module-07-border-outline-shadow-dan-efek-visual/125_clip_path.html))

### Module 08: Display, Positioning, and Overflow

**Curriculum Path**: [`module-08-display-positioning-dan-overflow`](./module-08-display-positioning-dan-overflow) | **Level**: `Intermediate` | **Scope**: 20 Lessons

#### Overview & Concepts Covered

Covers document normal flow control, element rendering types, and coordinates: standard display modes (`block`, `inline`, `inline-block`, `none`), element visibility states (`visibility: hidden` vs `display: none`), the CSS positioning scheme (`static`, `relative`, `absolute`, `fixed`, `sticky`), physical versus modern logical inset properties, the 3D stacking axis (`z-index`) and stacking context creation, container overflow management (`overflow: hidden`, `auto`, `scroll`, and directional `overflow-x`/`y`), and image scaling behavior via `object-fit` and `object-position`.

#### Subtopics

- [`126_display_block.css`](./module-08-display-positioning-dan-overflow/126_display_block.css) — `display: block` ([Preview HTML](./module-08-display-positioning-dan-overflow/126_display_block.html))
- [`127_display_inline.css`](./module-08-display-positioning-dan-overflow/127_display_inline.css) — `display: inline` ([Preview HTML](./module-08-display-positioning-dan-overflow/127_display_inline.html))
- [`128_display_inline_block.css`](./module-08-display-positioning-dan-overflow/128_display_inline_block.css) — `display: inline-block` ([Preview HTML](./module-08-display-positioning-dan-overflow/128_display_inline_block.html))
- [`129_display_none.css`](./module-08-display-positioning-dan-overflow/129_display_none.css) — `display: none` ([Preview HTML](./module-08-display-positioning-dan-overflow/129_display_none.html))
- [`130_visibility_property.css`](./module-08-display-positioning-dan-overflow/130_visibility_property.css) — The `visibility` Property (`visible` vs `hidden`) ([Preview HTML](./module-08-display-positioning-dan-overflow/130_visibility_property.html))
- [`131_position_static.css`](./module-08-display-positioning-dan-overflow/131_position_static.css) — `position: static` (Normal Flow) ([Preview HTML](./module-08-display-positioning-dan-overflow/131_position_static.html))
- [`132_position_relative.css`](./module-08-display-positioning-dan-overflow/132_position_relative.css) — `position: relative` ([Preview HTML](./module-08-display-positioning-dan-overflow/132_position_relative.html))
- [`133_position_absolute.css`](./module-08-display-positioning-dan-overflow/133_position_absolute.css) — `position: absolute` ([Preview HTML](./module-08-display-positioning-dan-overflow/133_position_absolute.html))
- [`134_position_fixed.css`](./module-08-display-positioning-dan-overflow/134_position_fixed.css) — `position: fixed` ([Preview HTML](./module-08-display-positioning-dan-overflow/134_position_fixed.html))
- [`135_position_sticky.css`](./module-08-display-positioning-dan-overflow/135_position_sticky.css) — `position: sticky` ([Preview HTML](./module-08-display-positioning-dan-overflow/135_position_sticky.html))
- [`136_top_right_bottom_left.css`](./module-08-display-positioning-dan-overflow/136_top_right_bottom_left.css) — Physical Inset Properties (`top`, `right`, `bottom`, `left`) ([Preview HTML](./module-08-display-positioning-dan-overflow/136_top_right_bottom_left.html))
- [`137_inset_logical_properties.css`](./module-08-display-positioning-dan-overflow/137_inset_logical_properties.css) — Logical Inset Properties (`inset`, `inset-block`, `inset-inline`) ([Preview HTML](./module-08-display-positioning-dan-overflow/137_inset_logical_properties.html))
- [`138_z_index.css`](./module-08-display-positioning-dan-overflow/138_z_index.css) — The `z-index` Property ([Preview HTML](./module-08-display-positioning-dan-overflow/138_z_index.html))
- [`139_stacking_context.css`](./module-08-display-positioning-dan-overflow/139_stacking_context.css) — CSS Stacking Context Creation and Layering ([Preview HTML](./module-08-display-positioning-dan-overflow/139_stacking_context.html))
- [`140_overflow_hidden.css`](./module-08-display-positioning-dan-overflow/140_overflow_hidden.css) — `overflow: hidden` and Clipping ([Preview HTML](./module-08-display-positioning-dan-overflow/140_overflow_hidden.html))
- [`141_overflow_auto.css`](./module-08-display-positioning-dan-overflow/141_overflow_auto.css) — `overflow: auto` and Scrollbars ([Preview HTML](./module-08-display-positioning-dan-overflow/141_overflow_auto.html))
- [`142_overflow_scroll.css`](./module-08-display-positioning-dan-overflow/142_overflow_scroll.css) — `overflow: scroll` ([Preview HTML](./module-08-display-positioning-dan-overflow/142_overflow_scroll.html))
- [`143_overflow_x_y.css`](./module-08-display-positioning-dan-overflow/143_overflow_x_y.css) — Independent Overflow (`overflow-x` and `overflow-y`) ([Preview HTML](./module-08-display-positioning-dan-overflow/143_overflow_x_y.html))
- [`144_object_fit.css`](./module-08-display-positioning-dan-overflow/144_object_fit.css) — The `object-fit` Property for Replaced Elements ([Preview HTML](./module-08-display-positioning-dan-overflow/144_object_fit.html))
- [`145_object_position.css`](./module-08-display-positioning-dan-overflow/145_object_position.css) — The `object-position` Property ([Preview HTML](./module-08-display-positioning-dan-overflow/145_object_position.html))

### Module 09: Flexbox Layout

**Curriculum Path**: [`module-09-flexbox-layout`](./module-09-flexbox-layout) | **Level**: `Intermediate` | **Scope**: 20 Lessons

#### Overview & Concepts Covered

Examines the one-dimensional Flexible Box Layout module: converting elements into flex containers (`display: flex`), main axis direction (`flex-direction`), multi-line wrapping (`flex-wrap`), the `flex-flow` shorthand, main-axis distribution (`justify-content`), cross-axis alignment (`align-items`, `align-content`, `align-self`), flexible growth, shrinkage, and base sizing (`flex-grow`, `flex-shrink`, `flex-basis`), structural reordering (`order`), gap spacing (`gap`), and practical UI patterns including responsive navigation bars, equal-height card grids, absolute centering, and adaptive sidebars.

#### Subtopics

- [`146_flexbox_basic.css`](./module-09-flexbox-layout/146_flexbox_basic.css) — Introduction to Flexbox Architecture ([Preview HTML](./module-09-flexbox-layout/146_flexbox_basic.html))
- [`147_display_flex.css`](./module-09-flexbox-layout/147_display_flex.css) — `display: flex` and Flex Container Initialization ([Preview HTML](./module-09-flexbox-layout/147_display_flex.html))
- [`148_flex_direction.css`](./module-09-flexbox-layout/148_flex_direction.css) — The `flex-direction` Property (Main Axis) ([Preview HTML](./module-09-flexbox-layout/148_flex_direction.html))
- [`149_flex_wrap.css`](./module-09-flexbox-layout/149_flex_wrap.css) — The `flex-wrap` Property and Multi-Line Flex ([Preview HTML](./module-09-flexbox-layout/149_flex_wrap.html))
- [`150_flex_flow.css`](./module-09-flexbox-layout/150_flex_flow.css) — The `flex-flow` Shorthand Property ([Preview HTML](./module-09-flexbox-layout/150_flex_flow.html))
- [`151_justify_content.css`](./module-09-flexbox-layout/151_justify_content.css) — The `justify-content` Property (Main Axis Alignment) ([Preview HTML](./module-09-flexbox-layout/151_justify_content.html))
- [`152_align_items.css`](./module-09-flexbox-layout/152_align_items.css) — The `align-items` Property (Cross Axis Alignment) ([Preview HTML](./module-09-flexbox-layout/152_align_items.html))
- [`153_align_content.css`](./module-09-flexbox-layout/153_align_content.css) — The `align-content` Property (Multi-Line Alignment) ([Preview HTML](./module-09-flexbox-layout/153_align_content.html))
- [`154_align_self.css`](./module-09-flexbox-layout/154_align_self.css) — The `align-self` Property (Individual Item Alignment) ([Preview HTML](./module-09-flexbox-layout/154_align_self.html))
- [`155_flex_grow.css`](./module-09-flexbox-layout/155_flex_grow.css) — The `flex-grow` Property (Space Distribution) ([Preview HTML](./module-09-flexbox-layout/155_flex_grow.html))
- [`156_flex_shrink.css`](./module-09-flexbox-layout/156_flex_shrink.css) — The `flex-shrink` Property (Item Contraction) ([Preview HTML](./module-09-flexbox-layout/156_flex_shrink.html))
- [`157_flex_basis.css`](./module-09-flexbox-layout/157_flex_basis.css) — The `flex-basis` Property (Initial Item Size) ([Preview HTML](./module-09-flexbox-layout/157_flex_basis.html))
- [`158_flex_shorthand.css`](./module-09-flexbox-layout/158_flex_shorthand.css) — The `flex` Shorthand Property ([Preview HTML](./module-09-flexbox-layout/158_flex_shorthand.html))
- [`159_order_property.css`](./module-09-flexbox-layout/159_order_property.css) — The `order` Property and Visual Reordering ([Preview HTML](./module-09-flexbox-layout/159_order_property.html))
- [`160_gap_flexbox.css`](./module-09-flexbox-layout/160_gap_flexbox.css) — The `gap` Property in Flexbox ([Preview HTML](./module-09-flexbox-layout/160_gap_flexbox.html))
- [`161_flexbox_navigation.css`](./module-09-flexbox-layout/161_flexbox_navigation.css) — Flexbox Navigation Bar Architecture ([Preview HTML](./module-09-flexbox-layout/161_flexbox_navigation.html))
- [`162_flexbox_cards.css`](./module-09-flexbox-layout/162_flexbox_cards.css) — Equal-Height Card Grid with Flexbox ([Preview HTML](./module-09-flexbox-layout/162_flexbox_cards.html))
- [`163_flexbox_centering.css`](./module-09-flexbox-layout/163_flexbox_centering.css) — Centering Elements with Flexbox ([Preview HTML](./module-09-flexbox-layout/163_flexbox_centering.html))
- [`164_flexbox_sidebar.css`](./module-09-flexbox-layout/164_flexbox_sidebar.css) — Sidebar with Flexbox ([Preview HTML](./module-09-flexbox-layout/164_flexbox_sidebar.html))
- [`165_flexbox_responsive_layout.css`](./module-09-flexbox-layout/165_flexbox_responsive_layout.css) — Adaptive Multi-Column Layouts with Flexbox ([Preview HTML](./module-09-flexbox-layout/165_flexbox_responsive_layout.html))

### Module 10: CSS Grid Layout

**Curriculum Path**: [`module-10-css-grid-layout`](./module-10-css-grid-layout) | **Level**: `Intermediate to Advanced` | **Scope**: 20 Lessons

#### Overview & Concepts Covered

Master the two-dimensional CSS Grid Layout engine: initializing grid containers (`display: grid`), explicit column and row definitions (`grid-template-columns`, `grid-template-rows`), visual layout mapping with named template areas (`grid-template-areas`), item placement coordinates (`grid-column`, `grid-row`, `grid-area`), grid gap spacing, implicit grid flow and auto track sizing (`grid-auto-flow`, `grid-auto-columns`/`rows`), responsive auto-placement keywords (`auto-fill`, `auto-fit`), flexible fractional units (`fr`), responsive track formulas (`minmax()`, `repeat()`), grid alignment properties (`justify-items`, `align-items`), and full multi-column card and dashboard architectures.

#### Subtopics

- [`166_grid_basic.css`](./module-10-css-grid-layout/166_grid_basic.css) — Introduction to 2D CSS Grid Layout ([Preview HTML](./module-10-css-grid-layout/166_grid_basic.html))
- [`167_display_grid.css`](./module-10-css-grid-layout/167_display_grid.css) — `display: grid` and Grid Container Initialization ([Preview HTML](./module-10-css-grid-layout/167_display_grid.html))
- [`168_grid_template_columns.css`](./module-10-css-grid-layout/168_grid_template_columns.css) — The `grid-template-columns` Property ([Preview HTML](./module-10-css-grid-layout/168_grid_template_columns.html))
- [`169_grid_template_rows.css`](./module-10-css-grid-layout/169_grid_template_rows.css) — The `grid-template-rows` Property ([Preview HTML](./module-10-css-grid-layout/169_grid_template_rows.html))
- [`170_grid_template_areas.css`](./module-10-css-grid-layout/170_grid_template_areas.css) — Named Grid Areas (`grid-template-areas`) ([Preview HTML](./module-10-css-grid-layout/170_grid_template_areas.html))
- [`171_grid_column.css`](./module-10-css-grid-layout/171_grid_column.css) — Column Placement with `grid-column` ([Preview HTML](./module-10-css-grid-layout/171_grid_column.html))
- [`172_grid_row.css`](./module-10-css-grid-layout/172_grid_row.css) — Row Placement with `grid-row` ([Preview HTML](./module-10-css-grid-layout/172_grid_row.html))
- [`173_grid_area.css`](./module-10-css-grid-layout/173_grid_area.css) — The `grid-area` Placement Property ([Preview HTML](./module-10-css-grid-layout/173_grid_area.html))
- [`174_grid_gap.css`](./module-10-css-grid-layout/174_grid_gap.css) — Grid Gap Spacing (`row-gap`, `column-gap`, `gap`) ([Preview HTML](./module-10-css-grid-layout/174_grid_gap.html))
- [`175_grid_auto_flow.css`](./module-10-css-grid-layout/175_grid_auto_flow.css) — Implicit Grid Flow (`grid-auto-flow`) ([Preview HTML](./module-10-css-grid-layout/175_grid_auto_flow.html))
- [`176_grid_auto_columns_rows.css`](./module-10-css-grid-layout/176_grid_auto_columns_rows.css) — Implicit Track Sizing (`grid-auto-columns` / `grid-auto-rows`) ([Preview HTML](./module-10-css-grid-layout/176_grid_auto_columns_rows.html))
- [`177_grid_auto_fit.css`](./module-10-css-grid-layout/177_grid_auto_fit.css) — Responsive Column Wrapping with `auto-fit` ([Preview HTML](./module-10-css-grid-layout/177_grid_auto_fit.html))
- [`178_grid_auto_fill.css`](./module-10-css-grid-layout/178_grid_auto_fill.css) — Empty Slot Reservation with `auto-fill` ([Preview HTML](./module-10-css-grid-layout/178_grid_auto_fill.html))
- [`179_minmax_function.css`](./module-10-css-grid-layout/179_minmax_function.css) — The `minmax()` Track Sizing Function ([Preview HTML](./module-10-css-grid-layout/179_minmax_function.html))
- [`180_repeat_function.css`](./module-10-css-grid-layout/180_repeat_function.css) — The `repeat()` Pattern Function ([Preview HTML](./module-10-css-grid-layout/180_repeat_function.html))
- [`181_fractional_units.css`](./module-10-css-grid-layout/181_fractional_units.css) — Fractional Unit (`fr`) Distribution ([Preview HTML](./module-10-css-grid-layout/181_fractional_units.html))
- [`182_justify_items_grid.css`](./module-10-css-grid-layout/182_justify_items_grid.css) — Inline Alignment with `justify-items` and `justify-self` ([Preview HTML](./module-10-css-grid-layout/182_justify_items_grid.html))
- [`183_align_items_grid.css`](./module-10-css-grid-layout/183_align_items_grid.css) — Block Alignment with `align-items` and `align-self` ([Preview HTML](./module-10-css-grid-layout/183_align_items_grid.html))
- [`184_grid_card_layout.css`](./module-10-css-grid-layout/184_grid_card_layout.css) — Responsive Card Layout with CSS Grid ([Preview HTML](./module-10-css-grid-layout/184_grid_card_layout.html))
- [`185_grid_dashboard_layout.css`](./module-10-css-grid-layout/185_grid_dashboard_layout.css) — Complex Dashboard Architecture with CSS Grid ([Preview HTML](./module-10-css-grid-layout/185_grid_dashboard_layout.html))

### Module 11: Responsive Web Design

**Curriculum Path**: [`module-11-responsive-web-design`](./module-11-responsive-web-design) | **Level**: `Intermediate to Advanced` | **Scope**: 20 Lessons

#### Overview & Concepts Covered

Focuses on responsive design paradigms, adaptive layouts, and media query specifications: core `@media` syntax, breakpoint architectures with `min-width` (mobile-first) and `max-width` (desktop-first), fluid layouts and percentage dimensions, responsive typography with mathematical bounds via `clamp()`, flexible images, adaptive navigation bars, responsive Flexbox and Grid patterns, orientation queries (`portrait`/`landscape`), user input hardware detection (`hover`, `pointer`), user preference media queries (`prefers-color-scheme`, `prefers-reduced-motion`), print media stylesheets, and next-generation Container Queries (`@container`).

#### Subtopics

- [`186_media_queries_basic.css`](./module-11-responsive-web-design/186_media_queries_basic.css) — Media Queries Syntax and Mechanics ([Preview HTML](./module-11-responsive-web-design/186_media_queries_basic.html))
- [`187_media_min_width.css`](./module-11-responsive-web-design/187_media_min_width.css) — Mobile-First Breakpoints with `min-width` ([Preview HTML](./module-11-responsive-web-design/187_media_min_width.html))
- [`188_media_max_width.css`](./module-11-responsive-web-design/188_media_max_width.css) — Desktop-First Breakpoints with `max-width` ([Preview HTML](./module-11-responsive-web-design/188_media_max_width.html))
- [`189_mobile_first.css`](./module-11-responsive-web-design/189_mobile_first.css) — Mobile-First Progressive Enhancement Strategy ([Preview HTML](./module-11-responsive-web-design/189_mobile_first.html))
- [`190_desktop_first.css`](./module-11-responsive-web-design/190_desktop_first.css) — Desktop-First Graceful Degradation Strategy ([Preview HTML](./module-11-responsive-web-design/190_desktop_first.html))
- [`191_responsive_typography.css`](./module-11-responsive-web-design/191_responsive_typography.css) — Responsive Typography and Fluid Font Scaling ([Preview HTML](./module-11-responsive-web-design/191_responsive_typography.html))
- [`192_fluid_layout.css`](./module-11-responsive-web-design/192_fluid_layout.css) — Fluid Percentage-Based Layouts ([Preview HTML](./module-11-responsive-web-design/192_fluid_layout.html))
- [`193_fluid_typography_clamp.css`](./module-11-responsive-web-design/193_fluid_typography_clamp.css) — Modern Fluid Typography with `clamp()` ([Preview HTML](./module-11-responsive-web-design/193_fluid_typography_clamp.html))
- [`194_responsive_images.css`](./module-11-responsive-web-design/194_responsive_images.css) — Responsive Images and Aspect-Ratio Preservation ([Preview HTML](./module-11-responsive-web-design/194_responsive_images.html))
- [`195_responsive_navigation.css`](./module-11-responsive-web-design/195_responsive_navigation.css) — Responsive Navigation and Mobile Toggle Menus ([Preview HTML](./module-11-responsive-web-design/195_responsive_navigation.html))
- [`196_responsive_flexbox.css`](./module-11-responsive-web-design/196_responsive_flexbox.css) — Adaptive Flexbox Breakpoints ([Preview HTML](./module-11-responsive-web-design/196_responsive_flexbox.html))
- [`197_responsive_grid.css`](./module-11-responsive-web-design/197_responsive_grid.css) — Adaptive CSS Grid Breakpoints ([Preview HTML](./module-11-responsive-web-design/197_responsive_grid.html))
- [`198_orientation_queries.css`](./module-11-responsive-web-design/198_orientation_queries.css) — Device Orientation Media Queries (`portrait` vs `landscape`) ([Preview HTML](./module-11-responsive-web-design/198_orientation_queries.html))
- [`199_hover_capability_queries.css`](./module-11-responsive-web-design/199_hover_capability_queries.css) — Hover Capability Media Queries (`hover: hover` vs `none`) ([Preview HTML](./module-11-responsive-web-design/199_hover_capability_queries.html))
- [`200_pointer_media_queries.css`](./module-11-responsive-web-design/200_pointer_media_queries.css) — Pointer Accuracy Media Queries (`pointer: fine` vs `coarse`) ([Preview HTML](./module-11-responsive-web-design/200_pointer_media_queries.html))
- [`201_prefers_color_scheme.css`](./module-11-responsive-web-design/201_prefers_color_scheme.css) — Dark Mode Adaptation with `prefers-color-scheme` ([Preview HTML](./module-11-responsive-web-design/201_prefers_color_scheme.html))
- [`202_prefers_reduced_motion.css`](./module-11-responsive-web-design/202_prefers_reduced_motion.css) — Accessibility Adaptation with `prefers-reduced-motion` ([Preview HTML](./module-11-responsive-web-design/202_prefers_reduced_motion.html))
- [`203_media_print_screen.css`](./module-11-responsive-web-design/203_media_print_screen.css) — Media Types (`print` vs `screen` Media Styles) ([Preview HTML](./module-11-responsive-web-design/203_media_print_screen.html))
- [`204_container_queries.css`](./module-11-responsive-web-design/204_container_queries.css) — Container Queries with `@container` ([Preview HTML](./module-11-responsive-web-design/204_container_queries.html))
- [`205_responsive_design_system.css`](./module-11-responsive-web-design/205_responsive_design_system.css) — Architecting a Complete Responsive Design System ([Preview HTML](./module-11-responsive-web-design/205_responsive_design_system.html))

### Module 12: Pseudo-classes and Pseudo-elements

**Curriculum Path**: [`module-12-pseudo-class-dan-pseudo-element`](./module-12-pseudo-class-dan-pseudo-element) | **Level**: `Intermediate to Advanced` | **Scope**: 20 Lessons

#### Overview & Concepts Covered

Details state-based selection and virtual element rendering: interactive user action states (`:hover`, `:active`), accessible focus management (`:focus`, `:focus-visible`, `:focus-within`), tree-structural selectors (`:first-child`, `:last-child`, `:first-of-type`, `:last-of-type`), functional pattern matchers (`:nth-child(An+B)`, `:nth-of-type()`), modern relational and grouping pseudo-classes (`:not()`, `:is()`, `:where()`, `:has()`), form control states (`:checked`, `:disabled`, `:enabled`), and generated/virtual pseudo-elements (`::before`, `::after`, `::marker`, `::selection`, `::placeholder`).

#### Subtopics

- [`206_hover_pseudo_class.css`](./module-12-pseudo-class-dan-pseudo-element/206_hover_pseudo_class.css) — The `:hover` User Action Pseudo-Class ([Preview HTML](./module-12-pseudo-class-dan-pseudo-element/206_hover_pseudo_class.html))
- [`207_active_pseudo_class.css`](./module-12-pseudo-class-dan-pseudo-element/207_active_pseudo_class.css) — The `:active` State Pseudo-Class ([Preview HTML](./module-12-pseudo-class-dan-pseudo-element/207_active_pseudo_class.html))
- [`208_focus_pseudo_class.css`](./module-12-pseudo-class-dan-pseudo-element/208_focus_pseudo_class.css) — The `:focus` Form and Element State ([Preview HTML](./module-12-pseudo-class-dan-pseudo-element/208_focus_pseudo_class.html))
- [`209_focus_visible.css`](./module-12-pseudo-class-dan-pseudo-element/209_focus_visible.css) — Accessible Focus Rings with `:focus-visible` ([Preview HTML](./module-12-pseudo-class-dan-pseudo-element/209_focus_visible.html))
- [`210_focus_within.css`](./module-12-pseudo-class-dan-pseudo-element/210_focus_within.css) — Parent Focus Detection with `:focus-within` ([Preview HTML](./module-12-pseudo-class-dan-pseudo-element/210_focus_within.html))
- [`211_first_child.css`](./module-12-pseudo-class-dan-pseudo-element/211_first_child.css) — Structural `:first-child` Pseudo-Class ([Preview HTML](./module-12-pseudo-class-dan-pseudo-element/211_first_child.html))
- [`212_last_child.css`](./module-12-pseudo-class-dan-pseudo-element/212_last_child.css) — Structural `:last-child` Pseudo-Class ([Preview HTML](./module-12-pseudo-class-dan-pseudo-element/212_last_child.html))
- [`213_nth_child.css`](./module-12-pseudo-class-dan-pseudo-element/213_nth_child.css) — Formulaic Selection with `:nth-child(An+B)` ([Preview HTML](./module-12-pseudo-class-dan-pseudo-element/213_nth_child.html))
- [`214_nth_of_type.css`](./module-12-pseudo-class-dan-pseudo-element/214_nth_of_type.css) — Type-Restricted Selection with `:nth-of-type()` ([Preview HTML](./module-12-pseudo-class-dan-pseudo-element/214_nth_of_type.html))
- [`215_first_of_type.css`](./module-12-pseudo-class-dan-pseudo-element/215_first_of_type.css) — The `:first-of-type` Pseudo-Class ([Preview HTML](./module-12-pseudo-class-dan-pseudo-element/215_first_of_type.html))
- [`216_last_of_type.css`](./module-12-pseudo-class-dan-pseudo-element/216_last_of_type.css) — The `:last-of-type` Pseudo-Class ([Preview HTML](./module-12-pseudo-class-dan-pseudo-element/216_last_of_type.html))
- [`217_not_pseudo_class.css`](./module-12-pseudo-class-dan-pseudo-element/217_not_pseudo_class.css) — Negation Matching with `:not()` ([Preview HTML](./module-12-pseudo-class-dan-pseudo-element/217_not_pseudo_class.html))
- [`218_is_pseudo_class.css`](./module-12-pseudo-class-dan-pseudo-element/218_is_pseudo_class.css) — Forgiving Selector Grouping with `:is()` ([Preview HTML](./module-12-pseudo-class-dan-pseudo-element/218_is_pseudo_class.html))
- [`219_where_pseudo_class.css`](./module-12-pseudo-class-dan-pseudo-element/219_where_pseudo_class.css) — Zero-Specificity Selector Grouping with `:where()` ([Preview HTML](./module-12-pseudo-class-dan-pseudo-element/219_where_pseudo_class.html))
- [`220_has_pseudo_class.css`](./module-12-pseudo-class-dan-pseudo-element/220_has_pseudo_class.css) — The Parent / Relational Selector `:has()` ([Preview HTML](./module-12-pseudo-class-dan-pseudo-element/220_has_pseudo_class.html))
- [`221_checked_pseudo_class.css`](./module-12-pseudo-class-dan-pseudo-element/221_checked_pseudo_class.css) — Input State Selection with `:checked` ([Preview HTML](./module-12-pseudo-class-dan-pseudo-element/221_checked_pseudo_class.html))
- [`222_disabled_enabled.css`](./module-12-pseudo-class-dan-pseudo-element/222_disabled_enabled.css) — State-Based Selection with `:disabled` and `:enabled` ([Preview HTML](./module-12-pseudo-class-dan-pseudo-element/222_disabled_enabled.html))
- [`223_before_pseudo_element.css`](./module-12-pseudo-class-dan-pseudo-element/223_before_pseudo_element.css) — Generated Content with `::before` ([Preview HTML](./module-12-pseudo-class-dan-pseudo-element/223_before_pseudo_element.html))
- [`224_after_pseudo_element.css`](./module-12-pseudo-class-dan-pseudo-element/224_after_pseudo_element.css) — Decorative Content with `::after` ([Preview HTML](./module-12-pseudo-class-dan-pseudo-element/224_after_pseudo_element.html))
- [`225_marker_selection_placeholder.css`](./module-12-pseudo-class-dan-pseudo-element/225_marker_selection_placeholder.css) — Specialized Pseudo-Elements (`::marker`, `::selection`, `::placeholder`) ([Preview HTML](./module-12-pseudo-class-dan-pseudo-element/225_marker_selection_placeholder.html))

### Module 13: Transforms, Transitions, and Animations

**Curriculum Path**: [`module-13-transform-transition-dan-animation`](./module-13-transform-transition-dan-animation) | **Level**: `Intermediate to Advanced` | **Scope**: 20 Lessons

#### Overview & Concepts Covered

Covers motion design, hardware-accelerated transformations, and CSS animation engines: 2D geometric manipulations (`translate`, `rotate`, `scale`, `skew`, `transform-origin`), 3D coordinate space (`translate3d`, `rotateX/Y/Z`, `perspective`, `transform-style: preserve-3d`, `backface-visibility`), smooth state transitions (`transition-property`, `duration`, `timing-function`, cubic-bezier curves, `delay`, `transition` shorthand), and keyframe timeline animation via `@keyframes` (`animation-duration`, `iteration-count`, `direction`, `fill-mode`, `play-state`, and multi-animation composition).

#### Subtopics

- [`226_transform_translate.css`](./module-13-transform-transition-dan-animation/226_transform_translate.css) — 2D Translation with `transform: translate()` ([Preview HTML](./module-13-transform-transition-dan-animation/226_transform_translate.html))
- [`227_transform_rotate.css`](./module-13-transform-transition-dan-animation/227_transform_rotate.css) — 2D Rotation with `transform: rotate()` ([Preview HTML](./module-13-transform-transition-dan-animation/227_transform_rotate.html))
- [`228_transform_scale.css`](./module-13-transform-transition-dan-animation/228_transform_scale.css) — 2D Scaling with `transform: scale()` ([Preview HTML](./module-13-transform-transition-dan-animation/228_transform_scale.html))
- [`229_transform_skew.css`](./module-13-transform-transition-dan-animation/229_transform_skew.css) — 2D Skewing with `transform: skew()` ([Preview HTML](./module-13-transform-transition-dan-animation/229_transform_skew.html))
- [`230_transform_origin.css`](./module-13-transform-transition-dan-animation/230_transform_origin.css) — Pivot Point Configuration with `transform-origin` ([Preview HTML](./module-13-transform-transition-dan-animation/230_transform_origin.html))
- [`231_transform_3d.css`](./module-13-transform-transition-dan-animation/231_transform_3d.css) — 3D Transformations (`translate3d`, `rotateX`, `rotateY`) ([Preview HTML](./module-13-transform-transition-dan-animation/231_transform_3d.html))
- [`232_perspective_property.css`](./module-13-transform-transition-dan-animation/232_perspective_property.css) — 3D Depth and the `perspective` Property ([Preview HTML](./module-13-transform-transition-dan-animation/232_perspective_property.html))
- [`233_transform_style.css`](./module-13-transform-transition-dan-animation/233_transform_style.css) — Nested 3D Scene Preservation with `transform-style: preserve-3d` ([Preview HTML](./module-13-transform-transition-dan-animation/233_transform_style.html))
- [`234_backface_visibility.css`](./module-13-transform-transition-dan-animation/234_backface_visibility.css) — 3D Card Flip Effects with `backface-visibility` ([Preview HTML](./module-13-transform-transition-dan-animation/234_backface_visibility.html))
- [`235_transition_property.css`](./module-13-transform-transition-dan-animation/235_transition_property.css) — The `transition-property` Configuration ([Preview HTML](./module-13-transform-transition-dan-animation/235_transition_property.html))
- [`236_transition_duration.css`](./module-13-transform-transition-dan-animation/236_transition_duration.css) — The `transition-duration` Timing Property ([Preview HTML](./module-13-transform-transition-dan-animation/236_transition_duration.html))
- [`237_transition_timing_function.css`](./module-13-transform-transition-dan-animation/237_transition_timing_function.css) — Easing Functions and Cubic Bezier Curves ([Preview HTML](./module-13-transform-transition-dan-animation/237_transition_timing_function.html))
- [`238_transition_delay.css`](./module-13-transform-transition-dan-animation/238_transition_delay.css) — Staggered Transitions with `transition-delay` ([Preview HTML](./module-13-transform-transition-dan-animation/238_transition_delay.html))
- [`239_transition_shorthand.css`](./module-13-transform-transition-dan-animation/239_transition_shorthand.css) — The `transition` Shorthand Property ([Preview HTML](./module-13-transform-transition-dan-animation/239_transition_shorthand.html))
- [`240_keyframes_animation.css`](./module-13-transform-transition-dan-animation/240_keyframes_animation.css) — Keyframe Timeline Architecture with `@keyframes` ([Preview HTML](./module-13-transform-transition-dan-animation/240_keyframes_animation.html))
- [`241_animation_duration.css`](./module-13-transform-transition-dan-animation/241_animation_duration.css) — The `animation-duration` Property ([Preview HTML](./module-13-transform-transition-dan-animation/241_animation_duration.html))
- [`242_animation_iteration_count.css`](./module-13-transform-transition-dan-animation/242_animation_iteration_count.css) — Loop Control with `animation-iteration-count` ([Preview HTML](./module-13-transform-transition-dan-animation/242_animation_iteration_count.html))
- [`243_animation_direction_fill_mode.css`](./module-13-transform-transition-dan-animation/243_animation_direction_fill_mode.css) — Animation Direction and Fill Modes (`animation-direction`, `animation-fill-mode`) ([Preview HTML](./module-13-transform-transition-dan-animation/243_animation_direction_fill_mode.html))
- [`244_animation_play_state.css`](./module-13-transform-transition-dan-animation/244_animation_play_state.css) — Interactive Playback with `animation-play-state` ([Preview HTML](./module-13-transform-transition-dan-animation/244_animation_play_state.html))
- [`245_animation_composition.css`](./module-13-transform-transition-dan-animation/245_animation_composition.css) — Chained and Multi-Animation Composition ([Preview HTML](./module-13-transform-transition-dan-animation/245_animation_composition.html))

### Module 14: CSS Variables, Functions, and Calculations

**Curriculum Path**: [`module-14-css-variables-functions-dan-perhitungan`](./module-14-css-variables-functions-dan-perhitungan) | **Level**: `Advanced` | **Scope**: 20 Lessons

#### Overview & Concepts Covered

Explores declarative programming and mathematical capabilities in modern CSS: CSS Custom Properties (CSS Variables) with `--` naming conventions, global (`:root`) versus local component scoping, retrieval and fallback handling via `var()`, dynamic arithmetic calculations with mixed units via `calc()`, bound-clamping functions (`min()`, `max()`, `clamp()`), modern color manipulation functions (`color-mix()`, relative color syntax), automatic light/dark theme adaptation via `light-dark()`, native document counters (`counter-reset`, `counter-increment`, `counter()`), design tokens architecture, dynamic spacing systems, and comprehensive application theming.

#### Subtopics

- [`246_css_custom_properties.css`](./module-14-css-variables-functions-dan-perhitungan/246_css_custom_properties.css) — CSS Custom Properties (Variables) Foundations ([Preview HTML](./module-14-css-variables-functions-dan-perhitungan/246_css_custom_properties.html))
- [`247_css_variable_declaration.css`](./module-14-css-variables-functions-dan-perhitungan/247_css_variable_declaration.css) — Declaring CSS Variables (`--property-name`) ([Preview HTML](./module-14-css-variables-functions-dan-perhitungan/247_css_variable_declaration.html))
- [`248_css_variable_scope.css`](./module-14-css-variables-functions-dan-perhitungan/248_css_variable_scope.css) — CSS Variable Scoping (Global vs Local) ([Preview HTML](./module-14-css-variables-functions-dan-perhitungan/248_css_variable_scope.html))
- [`249_root_selector_variables.css`](./module-14-css-variables-functions-dan-perhitungan/249_root_selector_variables.css) — Global Design Tokens on `:root` ([Preview HTML](./module-14-css-variables-functions-dan-perhitungan/249_root_selector_variables.html))
- [`250_var_function.css`](./module-14-css-variables-functions-dan-perhitungan/250_var_function.css) — Variable Retrieval and Fallbacks with `var()` ([Preview HTML](./module-14-css-variables-functions-dan-perhitungan/250_var_function.html))
- [`251_calc_function.css`](./module-14-css-variables-functions-dan-perhitungan/251_calc_function.css) — Dynamic Calculations with `calc()` ([Preview HTML](./module-14-css-variables-functions-dan-perhitungan/251_calc_function.html))
- [`252_min_function.css`](./module-14-css-variables-functions-dan-perhitungan/252_min_function.css) — Lower-Bound Restraints with `min()` ([Preview HTML](./module-14-css-variables-functions-dan-perhitungan/252_min_function.html))
- [`253_max_function.css`](./module-14-css-variables-functions-dan-perhitungan/253_max_function.css) — Upper-Bound Restraints with `max()` ([Preview HTML](./module-14-css-variables-functions-dan-perhitungan/253_max_function.html))
- [`254_clamp_function.css`](./module-14-css-variables-functions-dan-perhitungan/254_clamp_function.css) — Fluid Range Boundaries with `clamp()` ([Preview HTML](./module-14-css-variables-functions-dan-perhitungan/254_clamp_function.html))
- [`255_color_mix_function.css`](./module-14-css-variables-functions-dan-perhitungan/255_color_mix_function.css) — Modern Color Blending with `color-mix()` ([Preview HTML](./module-14-css-variables-functions-dan-perhitungan/255_color_mix_function.html))
- [`256_relative_color_syntax.css`](./module-14-css-variables-functions-dan-perhitungan/256_relative_color_syntax.css) — Relative Color Syntax Transformations ([Preview HTML](./module-14-css-variables-functions-dan-perhitungan/256_relative_color_syntax.html))
- [`257_light_dark_function.css`](./module-14-css-variables-functions-dan-perhitungan/257_light_dark_function.css) — Automatic Theme Switching with `light-dark()` ([Preview HTML](./module-14-css-variables-functions-dan-perhitungan/257_light_dark_function.html))
- [`258_css_counters.css`](./module-14-css-variables-functions-dan-perhitungan/258_css_counters.css) — Automatic Counter Foundations ([Preview HTML](./module-14-css-variables-functions-dan-perhitungan/258_css_counters.html))
- [`259_counter_reset_increment.css`](./module-14-css-variables-functions-dan-perhitungan/259_counter_reset_increment.css) — Manipulating Counters with `counter-reset` and `counter-increment` ([Preview HTML](./module-14-css-variables-functions-dan-perhitungan/259_counter_reset_increment.html))
- [`260_counter_function.css`](./module-14-css-variables-functions-dan-perhitungan/260_counter_function.css) — Displaying Numeric Counters with `counter()` and `counters()` ([Preview HTML](./module-14-css-variables-functions-dan-perhitungan/260_counter_function.html))
- [`261_custom_property_fallback.css`](./module-14-css-variables-functions-dan-perhitungan/261_custom_property_fallback.css) — Multi-Tiered Custom Property Fallbacks ([Preview HTML](./module-14-css-variables-functions-dan-perhitungan/261_custom_property_fallback.html))
- [`262_design_tokens.css`](./module-14-css-variables-functions-dan-perhitungan/262_design_tokens.css) — Architecting Design Tokens with CSS Variables ([Preview HTML](./module-14-css-variables-functions-dan-perhitungan/262_design_tokens.html))
- [`263_dynamic_spacing_system.css`](./module-14-css-variables-functions-dan-perhitungan/263_dynamic_spacing_system.css) — Dynamic Modular Spacing Scale Systems ([Preview HTML](./module-14-css-variables-functions-dan-perhitungan/263_dynamic_spacing_system.html))
- [`264_dynamic_color_system.css`](./module-14-css-variables-functions-dan-perhitungan/264_dynamic_color_system.css) — Dynamic Color Systems and Semantic Tokens ([Preview HTML](./module-14-css-variables-functions-dan-perhitungan/264_dynamic_color_system.html))
- [`265_theme_variables.css`](./module-14-css-variables-functions-dan-perhitungan/265_theme_variables.css) — Application Theming and Dynamic Mode Switching ([Preview HTML](./module-14-css-variables-functions-dan-perhitungan/265_theme_variables.html))

### Module 15: At-Rules and Modern CSS Features

**Curriculum Path**: [`module-15-at-rules-dan-fitur-css-modern`](./module-15-at-rules-dan-fitur-css-modern) | **Level**: `Advanced` | **Scope**: 15 Lessons

#### Overview & Concepts Covered

Investigates the advanced at-rule (`@`) ecosystem and cutting-edge Living Standard CSS features: modern `@media` range queries, feature detection with `@supports` (testing selectors and font formats), modular file imports via `@import`, self-hosted typography with `@font-face`, animation timelines with `@keyframes`, explicit specificity management with `@layer`, container-driven responsive design via `@container`, scoped component encapsulation using `@scope`, registered animatable typed CSS properties via Houdini `@property`, native CSS Nesting syntax (`&`), and smooth scroll snap mechanisms (`scroll-snap-type`, `scroll-snap-align`, `scroll-behavior: smooth`).

#### Subtopics

- [`266_media_at_rule.css`](./module-15-at-rules-dan-fitur-css-modern/266_media_at_rule.css) — Modern Range Syntax in `@media` ([Preview HTML](./module-15-at-rules-dan-fitur-css-modern/266_media_at_rule.html))
- [`267_supports_at_rule.css`](./module-15-at-rules-dan-fitur-css-modern/267_supports_at_rule.css) — Feature Detection with `@supports` ([Preview HTML](./module-15-at-rules-dan-fitur-css-modern/267_supports_at_rule.html))
- [`268_import_at_rule.css`](./module-15-at-rules-dan-fitur-css-modern/268_import_at_rule.css) — Modular Stylesheet Ingestion with `@import` ([Preview HTML](./module-15-at-rules-dan-fitur-css-modern/268_import_at_rule.html))
- [`269_font_face_at_rule.css`](./module-15-at-rules-dan-fitur-css-modern/269_font_face_at_rule.css) — Self-Hosted Typography with `@font-face` ([Preview HTML](./module-15-at-rules-dan-fitur-css-modern/269_font_face_at_rule.html))
- [`270_keyframes_at_rule.css`](./module-15-at-rules-dan-fitur-css-modern/270_keyframes_at_rule.css) — Animation Timeline Definition with `@keyframes` ([Preview HTML](./module-15-at-rules-dan-fitur-css-modern/270_keyframes_at_rule.html))
- [`271_layer_at_rule.css`](./module-15-at-rules-dan-fitur-css-modern/271_layer_at_rule.css) — Cascade Layer Architecture with `@layer` ([Preview HTML](./module-15-at-rules-dan-fitur-css-modern/271_layer_at_rule.html))
- [`272_container_at_rule.css`](./module-15-at-rules-dan-fitur-css-modern/272_container_at_rule.css) — Component-Level Responsive Containers with `@container` ([Preview HTML](./module-15-at-rules-dan-fitur-css-modern/272_container_at_rule.html))
- [`273_scope_at_rule.css`](./module-15-at-rules-dan-fitur-css-modern/273_scope_at_rule.css) — Scoped Styling and Boundary Encapsulation with `@scope` ([Preview HTML](./module-15-at-rules-dan-fitur-css-modern/273_scope_at_rule.html))
- [`274_property_at_rule.css`](./module-15-at-rules-dan-fitur-css-modern/274_property_at_rule.css) — Typed Houdini CSS Variables with `@property` ([Preview HTML](./module-15-at-rules-dan-fitur-css-modern/274_property_at_rule.html))
- [`275_css_nesting.css`](./module-15-at-rules-dan-fitur-css-modern/275_css_nesting.css) — Native CSS Nesting and Parent Selector (`&`) ([Preview HTML](./module-15-at-rules-dan-fitur-css-modern/275_css_nesting.html))
- [`276_cascade_layer_order.css`](./module-15-at-rules-dan-fitur-css-modern/276_cascade_layer_order.css) — Managing Cascade Layer Priority and Precedence ([Preview HTML](./module-15-at-rules-dan-fitur-css-modern/276_cascade_layer_order.html))
- [`277_css_feature_detection.css`](./module-15-at-rules-dan-fitur-css-modern/277_css_feature_detection.css) — Advanced Feature Detection with `@supports` (`selector()`, `font-tech()`) ([Preview HTML](./module-15-at-rules-dan-fitur-css-modern/277_css_feature_detection.html))
- [`278_scroll_snap_type.css`](./module-15-at-rules-dan-fitur-css-modern/278_scroll_snap_type.css) — CSS Scroll Snapping Containers with `scroll-snap-type` ([Preview HTML](./module-15-at-rules-dan-fitur-css-modern/278_scroll_snap_type.html))
- [`279_scroll_snap_align.css`](./module-15-at-rules-dan-fitur-css-modern/279_scroll_snap_align.css) — Scroll Alignment Points with `scroll-snap-align` ([Preview HTML](./module-15-at-rules-dan-fitur-css-modern/279_scroll_snap_align.html))
- [`280_scroll_behavior.css`](./module-15-at-rules-dan-fitur-css-modern/280_scroll_behavior.css) — Native Smooth Scrolling with `scroll-behavior: smooth` ([Preview HTML](./module-15-at-rules-dan-fitur-css-modern/280_scroll_behavior.html))

### Module 16: Forms, Tables, and Component Styling

**Curriculum Path**: [`module-16-form-tabel-dan-styling-komponen`](./module-16-form-tabel-dan-styling-komponen) | **Level**: `Advanced` | **Scope**: 10 Lessons

#### Overview & Concepts Covered

Focuses on practical UI component styling, form interface design, and data presentation: modern form input normalization, accessible focus indicators (`:focus`, `:focus-visible`), visual validation feedback (`:valid`, `:invalid`, `:user-invalid`), custom accessible checkboxes and radio buttons, multi-variant button component architecture, structured data table styling, zebra striping and row hover effects, responsive overflow tables for mobile viewports, cross-browser custom scrollbar styling, and native accordion disclosure widgets built on HTML5 `<details>` and `<summary>`.

#### Subtopics

- [`281_form_input_styling.css`](./module-16-form-tabel-dan-styling-komponen/281_form_input_styling.css) — Form Input Styling and Normalization ([Preview HTML](./module-16-form-tabel-dan-styling-komponen/281_form_input_styling.html))
- [`282_form_focus_states.css`](./module-16-form-tabel-dan-styling-komponen/282_form_focus_states.css) — Accessible Form Focus and Hover States ([Preview HTML](./module-16-form-tabel-dan-styling-komponen/282_form_focus_states.html))
- [`283_form_validation_states.css`](./module-16-form-tabel-dan-styling-komponen/283_form_validation_states.css) — Visual Form Validation Feedback with `:valid` and `:invalid` ([Preview HTML](./module-16-form-tabel-dan-styling-komponen/283_form_validation_states.html))
- [`284_checkbox_radio_styling.css`](./module-16-form-tabel-dan-styling-komponen/284_checkbox_radio_styling.css) — Custom Accessible Checkboxes and Radio Controls ([Preview HTML](./module-16-form-tabel-dan-styling-komponen/284_checkbox_radio_styling.html))
- [`285_button_component.css`](./module-16-form-tabel-dan-styling-komponen/285_button_component.css) — Multi-Variant Button Component System ([Preview HTML](./module-16-form-tabel-dan-styling-komponen/285_button_component.html))
- [`286_table_styling.css`](./module-16-form-tabel-dan-styling-komponen/286_table_styling.css) — Data Table Styling and Typography ([Preview HTML](./module-16-form-tabel-dan-styling-komponen/286_table_styling.html))
- [`287_table_zebra_stripes.css`](./module-16-form-tabel-dan-styling-komponen/287_table_zebra_stripes.css) — Zebra Striping and Row Hover Highlighting ([Preview HTML](./module-16-form-tabel-dan-styling-komponen/287_table_zebra_stripes.html))
- [`288_table_responsive.css`](./module-16-form-tabel-dan-styling-komponen/288_table_responsive.css) — Responsive Table Architectures and Horizontal Scrolling ([Preview HTML](./module-16-form-tabel-dan-styling-komponen/288_table_responsive.html))
- [`289_custom_scrollbar.css`](./module-16-form-tabel-dan-styling-komponen/289_custom_scrollbar.css) — Custom Scrollbar Styling (W3C Standard & WebKit) ([Preview HTML](./module-16-form-tabel-dan-styling-komponen/289_custom_scrollbar.html))
- [`290_details_summary_styling.css`](./module-16-form-tabel-dan-styling-komponen/290_details_summary_styling.css) — Custom Disclosure Accordion Styling (`details` and `summary`) ([Preview HTML](./module-16-form-tabel-dan-styling-komponen/290_details_summary_styling.html))

### Module 17: CSS Architecture, Debugging, and Best Practices

**Curriculum Path**: [`module-17-arsitektur-css-debugging-dan-best-practices`](./module-17-arsitektur-css-debugging-dan-best-practices) | **Level**: `Advanced` | **Scope**: 5 Lessons

#### Overview & Concepts Covered

Covers enterprise-grade stylesheet architecture, code maintainability standards, and debugging methodologies: CSS Reset strategies for removing browser styling inconsistencies, CSS Normalize approaches for preserving useful semantic defaults, BEM (Block, Element, Modifier) naming conventions to eliminate specificity collisions, utility-first (Atomic CSS) design patterns for rapid UI composition, and industry-standard modular file organization architectures (including ITCSS and the 7-1 pattern).

#### Subtopics

- [`291_css_reset.css`](./module-17-arsitektur-css-debugging-dan-best-practices/291_css_reset.css) — Modern Universal CSS Reset ([Preview HTML](./module-17-arsitektur-css-debugging-dan-best-practices/291_css_reset.html))
- [`292_css_normalize.css`](./module-17-arsitektur-css-debugging-dan-best-practices/292_css_normalize.css) — Cross-Browser Normalization with CSS Normalize ([Preview HTML](./module-17-arsitektur-css-debugging-dan-best-practices/292_css_normalize.html))
- [`293_bem_naming.css`](./module-17-arsitektur-css-debugging-dan-best-practices/293_bem_naming.css) — BEM (Block Element Modifier) Methodology ([Preview HTML](./module-17-arsitektur-css-debugging-dan-best-practices/293_bem_naming.html))
- [`294_css_utility_classes.css`](./module-17-arsitektur-css-debugging-dan-best-practices/294_css_utility_classes.css) — Utility-First CSS Classes and Atomic Styling ([Preview HTML](./module-17-arsitektur-css-debugging-dan-best-practices/294_css_utility_classes.html))
- [`295_css_organization.css`](./module-17-arsitektur-css-debugging-dan-best-practices/295_css_organization.css) — Modular CSS Architecture and Directory Structuring (ITCSS & 7-1) ([Preview HTML](./module-17-arsitektur-css-debugging-dan-best-practices/295_css_organization.html))

### Module 18: Practical Capstone CSS Projects

**Curriculum Path**: [`module-18-proyek-praktik-css`](./module-18-proyek-praktik-css) | **Level**: `Capstone / Practical` | **Scope**: 5 Projects

#### Overview & Concepts Covered

Synthesizes all foundational, intermediate, and advanced competencies developed throughout Modules 01 through 17 into 5 comprehensive, production-grade web projects: a modern User Profile Card component with avatars and statistical indicators (296), a Responsive Developer Portfolio page with an adaptive multi-column showcase gallery (297), an Interactive Analytics Dashboard layout leveraging CSS Grid with navigation sidebars and KPI metric cards (298), an E-Commerce Product Catalog layout with commercial badges and responsive cards (299), and a Full Modern Corporate Landing Page featuring a sticky navigation header, hero call-to-action, feature grid, and comprehensive footer (300).

#### Subtopics

- [`296_profile_card_project.css`](./module-18-proyek-praktik-css/296_profile_card_project.css) — User Profile Card Component ([Preview HTML](./module-18-proyek-praktik-css/296_profile_card_project.html))
- [`297_responsive_portfolio_project.css`](./module-18-proyek-praktik-css/297_responsive_portfolio_project.css) — Responsive Developer Portfolio Page ([Preview HTML](./module-18-proyek-praktik-css/297_responsive_portfolio_project.html))
- [`298_dashboard_layout_project.css`](./module-18-proyek-praktik-css/298_dashboard_layout_project.css) — Interactive Analytics Dashboard Layout ([Preview HTML](./module-18-proyek-praktik-css/298_dashboard_layout_project.html))
- [`299_ecommerce_layout_project.css`](./module-18-proyek-praktik-css/299_ecommerce_layout_project.css) — E-Commerce Storefront and Product Catalog ([Preview HTML](./module-18-proyek-praktik-css/299_ecommerce_layout_project.html))
- [`300_full_website_design_project.css`](./module-18-proyek-praktik-css/300_full_website_design_project.css) — Comprehensive Modern Corporate Landing Page ([Preview HTML](./module-18-proyek-praktik-css/300_full_website_design_project.html))

## Exercises & Practice

The curriculum emphasizes hands-on deliberate practice across every module, culminating in the complete web projects in Module 18. Learners are encouraged to test and solidify their understanding through the following project-based challenges:

1. **Card Component Refactoring (Modules 01–04)**: Convert hardcoded pixel widths and physical margins to modern logical properties (`margin-inline`, `padding-block`) and verify container integrity using `box-sizing: border-box`.
2. **Typography Scale System (Module 05)**: Replace static heading font sizes with a responsive fluid typography curve using `clamp()` and integrate a custom self-hosted `@font-face` font stack.
3. **Glassmorphism Elevation UI (Modules 06–07)**: Design a translucent floating control panel combining multi-layer drop shadows (`box-shadow`), translucent background fills, and background blur (`backdrop-filter: blur()`).
4. **Interactive Navigation Bar (Modules 08–09)**: Construct a mobile-responsive navigation bar using Flexbox that transitions smoothly from an expanded desktop layout to a compact drawer using clean CSS transforms and transitions.
5. **Auto-Responsive Card Grid (Module 10)**: Create a multi-column card layout using `grid-template-columns: repeat(auto-fit, minmax(260px, 1fr))` without writing a single `@media` breakpoint.
6. **Dark Mode Theming System (Modules 11 & 14)**: Build a design token registry using CSS Variables on `:root`, then add a `[data-theme="dark"]` selector block that dynamically reassigns surface, border, and text tokens.
7. **3D Interactive Flipping Card (Modules 12–13)**: Construct a two-sided card using `transform-style: preserve-3d` and `backface-visibility: hidden` that flips 180 degrees on hover to reveal details on the reverse side.
8. **Container-Aware Component (Module 15)**: Implement a component card that switches between vertical and horizontal orientations based on `@container (min-width: 450px)` when placed in varying parent column widths.
9. **Accessible Form & Table Interface (Module 16)**: Format a complete registration form and audit report table with custom focus rings (`:focus-visible`), validation states (`:valid`/`:invalid`), and horizontal overflow containment.
10. **Capstone Full Landing Page (Module 18)**: Build a complete responsive corporate landing page synthesizing sticky navigation headers, hero banners, feature grids, pricing tables, and multi-column footers.

## Code Execution & Expected Output

All learning modules in this repository are browser-native and require no compilation, bundling, or build tools. To inspect and verify stylesheets:

### 1. Inspecting Live Styling with Browser Developer Tools

Modern browser developer tools provide deep visual inspection into the CSS cascade and layout engines:

1. Open any `.html` preview file in your web browser (Google Chrome, Firefox, Edge, or Safari).
2. Right-click any styled element on the page and select **Inspect** (or press `F12` / `Ctrl+Shift+I` / `Cmd+Opt+I`).
3. Open the **Elements** panel and select the **Styles** sub-pane:
   - **Active Rules**: Inspect which CSS rulesets apply to the selected DOM element.
   - **Inherited Styles**: Trace which font, line-height, and color properties inherit from parent elements.
   - **Strikethrough Declarations**: Identify overridden declarations and observe how selector specificity or cascade order caused properties to be superseded.
4. Select the **Computed** sub-pane to view the final resolved pixel values calculated by the browser's layout engine.
5. Inspect the **Box Model Visualizer** at the top of the Computed tab to examine exact padding, border, and margin dimensions.

### 2. Grid and Flexbox Layout Overlays

Modern browser engines include specialized diagnostic overlays for Flexbox and Grid layouts:

- In the **Elements** panel, click the **grid** or **flex** badge next to container elements in the DOM tree.
- The browser will project interactive line numbers, track sizes, gap gutters, and area names directly over the rendered page, allowing you to debug track alignment and auto-placement visually.

### 3. Comparing with Verified Output Captures

Every subtopic in this curriculum is paired with a verified browser execution capture stored in that module's `output/` directory:

- Path format: `./module-XX-.../output/YY_topic_name.png`
- These captures represent the reference standard rendering produced by modern standards-compliant browser engines. When modifying styles or practicing exercises, compare your live browser window against the corresponding subtopic capture to verify visual accuracy.

## Learning Resources & References

- [MDN Web Docs — CSS](https://developer.mozilla.org/en-US/docs/Web/CSS) — The definitive reference guide for CSS properties, selectors, and browser compatibility tables.
- [W3C CSS Specifications & Working Group](https://www.w3.org/Style/CSS/) — The official standards body defining CSS recommendations and candidate drafts.
- [web.dev Learn CSS](https://web.dev/learn/css) — Google's comprehensive, modern course on CSS concepts, responsive design, and performance.
- [CSS-Tricks Almanac & Guides](https://css-tricks.com/) — In-depth guides covering CSS Flexbox, CSS Grid, custom properties, and UI design patterns.
- [Can I use...](https://caniuse.com/) — Up-to-date browser feature support matrices for modern CSS specifications.

## Troubleshooting

Below are solutions to common styling bugs, specificity conflicts, and rendering anomalies encountered in frontend web development:

| Issue | Cause | Solution |
| :--- | :--- | :--- |
| **New CSS rule fails to apply to element** | Higher specificity selector or inline style already targeting the element | Inspect the element in DevTools. Check the specificity score of competing rules. Increase selector specificity (e.g. add a class or parent class), refactor rules using Cascade Layers (`@layer`), or eliminate conflicting `!important` declarations. |
| **Element exceeds declared container width** | `box-sizing` defaults to `content-box`, causing padding and borders to expand total width | Add `box-sizing: border-box` to the element, or apply the global box-sizing reset (`*, *::before, *::after { box-sizing: border-box; }`) at the top of your stylesheet. |
| **Vertical space between blocks is smaller than expected** | Vertical margins between adjacent block elements collapse into a single margin | Understand margin collapsing mechanics: adjacent top and bottom margins collapse to the larger of the two. Use `padding` on containers or flex/grid `gap` spacing instead of adjacent margins. |
| **Flex item refuses to shrink and overflows container** | Flex items have an implicit default `min-width: auto`, preventing them from shrinking smaller than content | Add `min-width: 0` to the overflowing flex item to allow it to shrink below its intrinsic content width. |
| **`z-index` has no effect on element stacking** | The element has default `position: static`, or is trapped inside a lower parent Stacking Context | Ensure the element has `position: relative`, `absolute`, `fixed`, or `sticky`. If already positioned, check parent elements for properties that create a new Stacking Context (`opacity < 1`, `transform`, `filter`). |
| **Custom web font fails to load** | Browser blocking cross-origin font files under `file://` protocol or incorrect URL path in `@font-face` | Serve files via a local HTTP server (`python -m http.server 8080` or VS Code Live Server). Verify font file paths are relative to the CSS file location and that font MIME types (`font/woff2`) are supported. |
| **Modern CSS feature (e.g., `@container` or `:has()`) not working** | Outdated browser version lacking support for newer CSS Living Standard specifications | Update your web browser to the latest stable release (Chrome 105+, Firefox 121+, Safari 16+). Wrap modern features inside `@supports` queries to provide graceful fallback styles for older engines. |

## License

Please see the [LICENSE](./LICENSE) file for the terms and conditions governing the use, modification, and distribution of this project.

## Author & Contact

**Yohanes Dimas Pratama**

- GitHub: [github.com/weztcy](https://github.com/weztcy)
- Portfolio: [dimaspratama.vercel.app](https://dimaspratama.vercel.app)
- LinkedIn: [linkedin.com/in/yohanes-dimas](https://www.linkedin.com/in/yohanes-dimas)
