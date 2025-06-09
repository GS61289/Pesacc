# Website Build Checklist

> **Progress:** ![progress-bar](https://progress-bar.dev/0/?title=Not%20Started)

This checklist outlines the key steps for building the Cognia accreditation website. Update the progress bar and checkboxes as you complete each step.

---

## Build Steps

- [ ] **1. Initialize the Project Repository**
    1. Go to [GitHub](https://github.com/) and create a new repository (public or private as needed).
    2. Clone the repository to your local machine using `git clone <repo-url>`.
    3. (Optional) Set up a `.gitignore` file for Jekyll or your chosen SSG.
    4. Make an initial commit (e.g., a README file) and push to GitHub.

- [ ] **2. Set Up the Static Site Generator**
    **Option A: Local Setup (Recommended if you have Jekyll installed locally)**
    1. Install [Jekyll](https://jekyllrb.com/docs/installation/) (recommended) or another SSG (Hugo, Eleventy) on your local machine.
    2. Run `jekyll new .` in your project directory to scaffold a new Jekyll site (or follow the equivalent for your SSG).
    3. Test the local build with `bundle exec jekyll serve` (or the SSG's local server command).
    4. Commit and push the generated files to GitHub.

    **Option B: Set Up Jekyll Directly on GitHub (No Local Installation Needed)**
    1. Go to the [Jekyll Minima template repository](https://github.com/jekyll/minima) (or [Jekyll basic starter](https://github.com/jekyll/jekyll)).
    2. Click the "Use this template" button to create a new repository in your GitHub account.
    3. Name your new repository and create it.
    4. (Optional) Clone the new repository to your local machine or open it in Cursor for further editing.
    5. Edit files directly on GitHub or in your editor as needed.
    6. Enable GitHub Pages in your repository settings (Settings > Pages) and select the branch (usually `main` or `gh-pages`).
    7. Your site will be live at the provided GitHub Pages URL.

    **Option C: Manual File Creation on GitHub**
    1. Create a new repository on GitHub.
    2. Manually add the following files/folders via the GitHub web interface:
        - `_config.yml` (basic config file)
        - `index.md` or `index.html` (homepage)
        - `_layouts/` (with at least a `default.html`)
        - `_includes/` (optional, for reusable components)
        - Any other folders you need (`assets/`, `pages/`, etc.)
    3. Enable GitHub Pages as above.
    4. Edit and build your site directly on GitHub or in your editor.

- [ ] **3. Create the Folder Structure**
    1. Create folders as per the technical approach:
        - `_layouts/` for templates
        - `_includes/` for reusable components
        - `pages/` for main content sections
        - `assets/` for CSS, JS, images
        - `index.html` for the homepage
    2. Add placeholder files (e.g., `home.md`, `standards.md`) in the `pages/` folder.
    3. Commit and push the structure to GitHub.

- [ ] **4. Build the Navigation and Layouts**
    1. Edit `_layouts/default.html` (or equivalent) to include a header, footer, and navigation bar.
    2. Add navigation links for all main sections and sub-sections (dropdowns or sidebar as needed).
    3. Ensure navigation is responsive and accessible.
    4. Commit and push changes.

- [ ] **5. Add Content Pages**
    1. For each main section (Home, Overview, Standards, Data Collection, etc.), create a Markdown file in `pages/`.
    2. Use the templates and structure defined in the technical approach.
    3. Add sample or initial content to each page.
    4. Commit and push content updates.

- [ ] **6. Apply Styling**
    1. Choose a CSS framework (Bootstrap, Tailwind, etc.).
    2. Add the framework to your project (via CDN or npm/yarn as appropriate).
    3. Update your layouts and includes to use the framework's classes for a modern, responsive design.
    4. Test on different devices for mobile-friendliness.
    5. Commit and push styling changes.

- [ ] **7. Test Locally**
    1. Run the local server (`bundle exec jekyll serve` or equivalent).
    2. Click through all pages and navigation links to check for errors or broken links.
    3. Review layout and content for consistency and clarity.
    4. Fix any issues found and commit changes.

- [ ] **8. Deploy to GitHub Pages**
    1. Push your latest changes to the branch/folder configured for GitHub Pages (`main`, `gh-pages`, or `/docs`).
    2. Go to the repository's Settings > Pages and ensure the correct branch/folder is selected.
    3. Wait for GitHub Pages to build and deploy your site.
    4. Visit the published URL to verify the site is live and working.

- [ ] **9. Iterate and Refine**
    1. Gather feedback from users and stakeholders.
    2. Add new features, improve content, and fix issues as needed.
    3. Update the checklist and progress bar to reflect your progress.
    4. Repeat testing and deployment as changes are made.

---

**Tip:** Update the progress bar URL (https://progress-bar.dev/XX) with your current completion percentage (e.g., 30, 50, 100) as you check off steps. 