# Minki Hong's Personal Website

This is the repository for my personal academic website, accessible at [bk123477.github.io](https://bk123477.github.io/). 

The site is built using Jekyll and is hosted on GitHub Pages. It features a clean, professional design focused on showcasing my research, publications, and latest news.

---

## 📝 How to Update Content

The website is designed to be easily updatable by adding or modifying Markdown files. Here is a quick guide on how to add new content:

### 1. Adding a New Publication
All publications are stored in the `_publications/` directory.

1. **Copy the Template**: Duplicate the `_publications/00-template.md` file and rename it to your paper's title (e.g., `new-paper-title.md`).
2. **Add Files**: 
   - Place your paper's PDF file in `assets/files/publications/`.
   - Place the framework image/thumbnail in `assets/images/publications/`.
3. **Update Frontmatter**: Open your new markdown file and update the fields:
   - `title`: The title of your paper.
   - `venue`: Where it was published (e.g., EMNLP 2026).
   - `date`: The publication date (`YYYY-MM-DD`).
   - `authors`: The list of authors (bold your name with `**Minki Hong**`).
   - `image`: The path to your thumbnail (e.g., `/assets/images/publications/my_image.png`).
   - `paperurl`: The path to your PDF (e.g., `/assets/files/publications/my_paper.pdf`).
   - `abstract`: The full abstract of the paper. This will be hidden behind a clean toggle button on the website.

### 2. Adding a New News/Blog Post
News and blog posts are stored in the `_posts/` directory.

1. **Create a File**: Create a new markdown file in `_posts/` using the format `YYYY-MM-DD-title-of-post.md`.
2. **Add Frontmatter**: Include the following at the top of the file:
   ```markdown
   ---
   title: "Your News Title"
   date: YYYY-MM-DD
   permalink: /posts/YYYY/MM/title/
   tags:
     - news
     - updates
   ---
   ```
3. **Write Content**: Write the body of your news post below the `---`. The site will automatically generate a summary card on the News page and Home page.

### 3. Updating the "About Me" Section
The main biography and contact information on the home page are located in `_pages/about.md`. Simply edit this file to update your bio or links.

### 4. Updating the CV
To update your CV, simply replace the `CV_Minki_Hong.pdf` file located in the `files/` directory with your latest version. Make sure the filename remains exactly the same so that the navigation links continue to work.

---

## ⚙️ Configuration
General site settings, such as your social media links, email, and Google Scholar URL, are managed in `_config.yml`. If you modify `_config.yml`, the changes will take effect on your next push to GitHub.

To change the items in the top navigation bar, edit `_data/navigation.yml`.
