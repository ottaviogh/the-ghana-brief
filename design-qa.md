# Design QA — The Ghana Brief

**Source visual truth**

- Selected ideation result: Option 2, “The Global Dispatch”.
- Local source path: `/workspace/scratch/b441720dd8dd/generated_images/exec-4904f144-ffe3-442e-9783-2e878ac53d12.png`
- Source pixels: 1536 × 1024. The board contains a 1440 × 1024 desktop concept and a 390 × 844 mobile concept, scaled into one presentation image.

**Implementation evidence**

- URL: `http://terminal.local:4173/`
- Browser-rendered screenshot: Cloud Browser tab 2 homepage viewport capture, observed in the final QA pass. The browser integration supplied image evidence directly and did not expose a local screenshot path.
- Browser viewport: 1363 × 936 CSS px; document width 1348 CSS px; device scale factor 1.
- State: homepage, newsletter form empty, menu closed, search closed.
- Density normalization: both source board and implementation capture were reviewed at 1×. Layout proportions were compared against the desktop frame within the board rather than the board canvas.

**Full-view comparison evidence**

- The final browser capture preserves the source hierarchy: compact dark masthead; asymmetric forest-green hero; large ivory serif headline at left; dominant Ghanaian editorial photograph at right; gold primary action; immediate ivory newsletter band.
- The hero and newsletter remain above the fold at the tested desktop viewport, matching the source's information density and visual rhythm.
- The implementation expands the concept into a longer publication homepage below the source viewport while preserving the selected visual system.

**Focused-region comparison evidence**

- Header: gold GB raster mark, uppercase serif wordmark, tagline, editorial navigation, search and gold Subscribe control match the selected direction.
- Hero: generated Accra creative-business photography matches the source art direction, focal grouping and warm green/gold palette. Crop remains sharp and balanced.
- Newsletter band: title, supporting text, email input, consent control and gold action preserve the source anatomy and spacing.
- Focused regions were readable in the full browser capture; no further crop was required.

**Required fidelity surfaces**

- Fonts and typography: DM Serif Display provides the high-contrast editorial character; DM Sans provides clean navigation and body copy. Weights, line height and desktop headline wrapping closely match the selected direction.
- Spacing and layout rhythm: desktop grid, hero depth, section gutters and newsletter spacing match the visual target. Responsive breakpoints at 1000 px and 650 px provide the requested tablet and mobile reflow.
- Colors and tokens: exact requested tokens are used: forest `#102C25`, champagne `#D6BB79`, ivory `#F8F6F0`, charcoal `#222B28`.
- Image quality and asset fidelity: hero and diaspora images are full-resolution generated raster assets with consistent editorial art direction. The GB mark is a raster asset derived from the selected design concept. No visible asset was replaced with CSS art or a placeholder.
- Copy and content: the target headline, tagline, navigation and newsletter proposition are preserved. All demonstration reporting is explicitly marked “Sample” or “Concept content.”

**Interaction and accessibility verification**

- Tested primary navigation from homepage to Business & Money and back.
- Tested site search with “diaspora” and confirmed the matching sample feature.
- Tested consent-gated newsletter flow with a valid local sample address and confirmed the success state.
- Tested article opening and confirmed the sample-content disclosure and sources section.
- Tested advertising enquiry form and its confirmation state.
- Tested the dedicated privacy page.
- Checked browser console: no application errors. One Chrome extension metadata error was excluded because it does not originate from the site.
- Semantic headings, button labels, form labels, focusable controls, alt text and reduced-motion handling are present.

**Findings**

- No actionable P0, P1 or P2 differences remain.

**Comparison history**

1. Initial browser pass found two P2 scope gaps outside the homepage visual: the Privacy route reused About content, and Advertise lacked a working enquiry form.
2. Fixed by adding a dedicated concept privacy policy, CMS/editorial workflow copy, and an accessible advertising enquiry form with confirmation state.
3. Post-fix browser evidence confirmed both routes and the form success state with no application console errors.

**Follow-up polish**

- P3: connect a real beehiiv publication and replace concept-domain contact addresses before launch.
- P3: replace sample stories with sourced editorial work through the chosen CMS.

**Final result: passed**
