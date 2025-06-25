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
