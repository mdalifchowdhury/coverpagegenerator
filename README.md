# Assignment Cover Page Generator – Print-Ready A4 Cover Pages in Your Browser

Assignment Cover Page Generator is a lightweight, browser-based tool that turns a simple form into a clean, print-ready A4 cover page for university assignments. Fill in the details, choose a template, watch the page update live, and save it as a PDF from your browser's print dialog.

It is built for students who are tired of rebuilding the same cover page in Word for every submission. The whole app is one HTML file: no installation, no internet connection, and no account needed.

## ✨ Key Features

### 📝 Live Cover Page Builder

- Fill in the form and watch the A4 cover page update as you type.
- Fields are grouped into University Information, Assignment Information, Submitted To, Submitted By, and Optional Information.
- Required fields are marked with `*`. Optional fields left empty are dropped from the cover page automatically, so there are no blank labels or gaps.
- The assignment type becomes the main heading on the cover. Pick a suggestion (Individual Assignment, Group Assignment, Report, Case Study, Term Paper) or type your own. If left blank, it shows "Assignment".
- The submission date is shown in a long format, such as "5 November 2026".
- Group members can be listed one per line and appear as a "Group Members" list.
- Additional notes appear above the submission date, with line breaks kept.

### 🎨 Templates

Switch between three designs at any time without losing what you typed.

| Template | Style |
|---|---|
| Classic Academic (default) | Serif font, double-line navy border, centered header |
| Modern Minimalist | Sans-serif font, navy accent bar on the left edge, light panels behind the "Submitted To" and "Submitted By" sections |
| Formal Corporate | Navy bars at the top and bottom, boxed assignment type, navy section headings |

### 🖼️ University Logo

- Upload your university logo to show it at the top of the cover page.
- See a thumbnail preview and remove the logo with one click.
- Clear messages appear for unsupported file types and files over 2 MB.
- The logo is read locally in your browser and is never uploaded anywhere.

### 📄 Export Options

- **Print / Save as PDF** – prints only the cover page (the form is hidden) in A4 portrait. The PDF file name is suggested automatically as `Student Name - Course Code - Assignment Type`.
- **Download as HTML** – saves the finished cover as a standalone `cover-page.html` file with the styles and logo embedded.
- Both options check that all required fields are filled before they run.

### ✅ Layout & Usability

- A warning appears if your content is taller than one A4 page.
- The preview scales down to fit smaller screens while keeping A4 proportions.
- Responsive layout: form beside the preview on desktop, stacked on narrow screens.
- All text is HTML-escaped before rendering, so characters like `&` and `<` appear exactly as typed.
- Labeled fields, visible keyboard focus, and status messages for screen readers.

### 🧪 Sample Data & Reset

- **Load Sample Data** fills the form with an example so you can try the templates instantly. A logo you already uploaded is kept.
- **Reset Form** clears all fields, the template choice, and the logo.

## 📋 Form Fields

| Section | Required | Optional |
|---|---|---|
| University Information | University name, Department | Faculty, Campus or address |
| Assignment Information | Assignment title, Course title, Course code, Submission date | Assignment type |
| Submitted To | Teacher's full name | Designation, Department, Faculty or institution |
| Submitted By | Student's full name, Student ID, Degree / program | Department, Faculty, Academic session, Semester or year, Section or group |
| Optional Information | – | Group members and IDs, Additional notes |

## 📂 Supported Logo Formats

| Format | Support |
|---|---|
| PNG | Yes |
| JPG / JPEG | Yes |
| SVG | Yes |
| WebP | Yes |
| GIF and other formats | No |

Note: The maximum logo size is 2 MB.

## 🛠️ Technologies Used

- **HTML5** – page and form structure
- **CSS3** – responsive layout (Grid and Flexbox), the three cover templates, and the A4 print stylesheet (`@page`, `@media print`)
- **Vanilla JavaScript** – form generation, live rendering, validation, logo handling, and export
- **Browser APIs** – FileReader (logo upload), Blob and `URL.createObjectURL` (HTML download), ResizeObserver (preview scaling), `window.print()` (PDF export)
- **System fonts only** – Georgia, Segoe UI, Arial, and similar; no external fonts, libraries, or frameworks

## 🔐 Privacy & Data Handling

The generator runs entirely in your browser.

- No backend server is required.
- Nothing you type and no logo you upload is sent anywhere. The app makes no network requests.
- No LocalStorage, cookies, or accounts are used, so nothing is saved between sessions. Closing or refreshing the page clears the form.

Privacy note: A downloaded HTML cover contains your cover page text and your logo (embedded in the file), so share it only if you are comfortable with that.

## 🚀 How to Use

1. Download or clone this repository.
2. Open `index.html` in a modern web browser (Chrome, Edge, Firefox, or Safari).
3. Choose a template, and optionally upload your university logo.
4. Fill in the form. Fields marked with `*` are required.
5. Check the live preview. If a warning says the cover is taller than one A4 page, shorten long text or clear optional fields.
6. Click **Print / Save as PDF** and use the print settings below.
7. Save the PDF, or click **Download as HTML** for a standalone copy.

Want to see it first? Click **Load Sample Data** to fill the form with an example.

### Recommended Print Settings

| Setting | Value |
|---|---|
| Destination | Save as PDF |
| Paper size | A4 |
| Margins | None |
| Headers and footers | Off |

Option names vary slightly between browsers.

## 📌 Project Limitations

- A4 portrait only, one page per cover. Content that does not fit on one page is clipped, and the app shows a warning.
- One logo only. The color theme is fixed (navy) and there are three templates.
- Cover labels (such as "Submitted To" and "Course Code") are in English and cannot be edited from the interface. The submission date is always shown in English, day-month-year format.
- No saved drafts or reusable university details. Everything must be re-entered in each session.
- PDF export uses the browser's print dialog instead of a built-in PDF generator, so the options vary slightly between browsers.
- The downloaded HTML is a static snapshot. It cannot be loaded back into the form for editing.
- Fonts depend on what is installed on your device, so the cover may look slightly different across operating systems.

## 🔮 Future Improvements

Potential features for future versions:

- Save and reload drafts (for example, with LocalStorage or JSON export/import).
- A reusable university and department profile to pre-fill repeated details.
- More templates and an accent color picker.
- Paper size options (A4 and US Letter).
- Support for a second logo, such as a department logo.
- Editable field labels and multi-language cover pages.
- Separate name and ID columns for group members.
- Direct PDF export without the print dialog.

## 🎯 Project Objective

The objective of Assignment Cover Page Generator is to make a repetitive task quick: producing a consistent, professional-looking assignment cover page without opening a design tool or reformatting a Word template every time.

It also shows how far a single, dependency-free HTML file can go: form handling, live preview, validation, print styling, and file export, all in plain HTML, CSS, and JavaScript.

---

Project: Assignment Cover Page Generator  
Category: Education Tools | Web Development | Document Generation  
Status: Functional / Ongoing Development
