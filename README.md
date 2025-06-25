# namkwangwoo.github.io

## Blog Description

This is a personal blog (초안 블로그) built with Hugo, where I share my thoughts, ideas, and experiences in both Korean and English. The purpose of this blog is to document my journey, share knowledge, and connect with like-minded individuals. The blog covers topics including technology, AI, development, and personal reflections.

## Technical Stack

- **Static Site Generator**: [Hugo](https://gohugo.io/) v0.145.0
- **Theme**: [PaperMod](https://github.com/adityatelange/hugo-PaperMod)
- **Hosting**: GitHub Pages
- **Deployment**: Automated via GitHub Actions
- **Language**: Korean (ko-kr) with English content support

## Running the Blog Locally

To run the blog locally using Hugo, follow these steps:

1. **Prerequisites**: Ensure you have Hugo installed on your machine. Follow the instructions on the [Hugo website](https://gohugo.io/getting-started/installing/) to install Hugo.

2. **Clone the repository**:
   ```bash
   git clone https://github.com/namkwangwoo/namkwangwoo.github.io.git
   cd namkwangwoo.github.io
   ```

3. **Initialize submodules** (required for the PaperMod theme):
   ```bash
   git submodule update --init --recursive
   ```

4. **Start the Hugo development server**:
   ```bash
   hugo server -D
   ```

5. **Access the blog**: Open your browser and go to `http://localhost:1313/namkwangwoo.github.io/` to see the blog.

The `-D` flag includes draft posts in the development build. Remove it if you only want to see published content.

## Deploying the Blog to GitHub Pages

This blog is automatically deployed to GitHub Pages using GitHub Actions. To deploy changes:

1. **Verify configuration**: Ensure that the `baseURL` in the `config.toml` file is correctly set:
   ```toml
   baseURL = "https://namkwangwoo.github.io/namkwangwoo.github.io/"
   ```

2. **Push your changes** to the `main` branch of your repository:
   ```bash
   git add .
   git commit -m "Update blog content"
   git push origin main
   ```

3. **Automatic deployment**: GitHub Actions will automatically build and deploy the blog to GitHub Pages. You can monitor the deployment progress in the "Actions" tab of your GitHub repository.

4. **Access the live blog**: Once deployed, the blog will be available at [https://namkwangwoo.github.io/namkwangwoo.github.io/](https://namkwangwoo.github.io/namkwangwoo.github.io/)

The deployment process typically takes 2-5 minutes to complete.

## Creating New Blog Posts

To create a new blog post:

1. **Create a new post using Hugo's archetype**:
   ```bash
   hugo new posts/YYYY-MM-DD-your-post-title.md
   ```

2. **Edit the post**: Open the newly created file in `content/posts/` and update the front matter and content:
   ```markdown
   ---
   title: "Your Post Title"
   date: 2024-01-01T10:00:00+09:00
   tags: ["tag1", "tag2"]
   draft: false  # Set to false when ready to publish
   ---
   
   Your post content here...
   ```

3. **Preview your post**: Use `hugo server -D` to preview draft posts locally.

4. **Publish**: Set `draft: false` in the front matter and push to the main branch.

## Project Structure

```
namkwangwoo.github.io/
├── .github/workflows/     # GitHub Actions for deployment
├── archetypes/           # Template for new posts
├── content/posts/        # Blog post markdown files
├── themes/papermod/      # PaperMod theme (Git submodule)
├── config.toml          # Hugo configuration
├── README.md            # This file
└── LICENSE              # MIT License
```

## Content Management

- **Languages**: Content is primarily in Korean with English support
- **Tags**: Use Korean tags to categorize posts (e.g., "인공지능", "개발", "기술")
- **Drafts**: Posts with `draft: true` are only visible when using `hugo server -D`
- **Date Format**: Use KST timezone (`+09:00`) for consistent post dating

## Useful Hugo Commands

- `hugo server -D` - Start development server with drafts
- `hugo server --navigateToChanged` - Auto-navigate to changed content
- `hugo --minify` - Build optimized production site
- `hugo new posts/filename.md` - Create new post from archetype
- `hugo list drafts` - List all draft posts
- `hugo list future` - List posts with future publish dates

## Theme Customization

This blog uses the [PaperMod theme](https://github.com/adityatelange/hugo-PaperMod). Key customization options in `config.toml`:

- `title`: Blog title (currently "초안 블로그")
- `description`: Blog description for SEO
- `languageCode`: Set to "ko-kr" for Korean
- `baseURL`: Must match GitHub Pages URL

For advanced customization, refer to the [PaperMod documentation](https://github.com/adityatelange/hugo-PaperMod/wiki).

## Troubleshooting

**Common Issues:**

1. **Submodule not initialized**: If the theme doesn't load, run:
   ```bash
   git submodule update --init --recursive
   ```

2. **Local server not accessible**: Ensure you're accessing `http://localhost:1313/namkwangwoo.github.io/` (note the repository name in the path).

3. **Deployment failures**: Check the GitHub Actions logs in the "Actions" tab of the repository.

4. **Hugo command not found**: Install Hugo from [the official website](https://gohugo.io/getting-started/installing/).

## Contributing

1. Fork the repository
2. Create a new branch for your changes
3. Make your changes and test locally
4. Submit a pull request with a clear description

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
