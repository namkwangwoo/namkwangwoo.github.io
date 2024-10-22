# namkwangwoo.github.io

## Blog Description

This blog is a personal space where I share my thoughts, ideas, and experiences. The purpose of this blog is to document my journey, share knowledge, and connect with like-minded individuals.

## Running the Blog Locally

To run the blog locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/namkwangwoo/namkwangwoo.github.io.git
   cd namkwangwoo.github.io
   ```

2. Install Hugo:
   Follow the instructions on the [Hugo website](https://gohugo.io/getting-started/installing/) to install Hugo on your machine.

3. Start the Hugo server:
   ```bash
   hugo server -D
   ```

4. Open your browser and go to `http://localhost:1313` to see the blog.

## Deploying the Blog to GitHub Pages

To deploy the blog to GitHub Pages, follow these steps:

1. Ensure that the `baseURL` in the `config.toml` file is set to your GitHub Pages URL:
   ```toml
   baseURL = "https://<your-username>.github.io/<your-repo>/"
   ```

2. Push your changes to the `main` branch of your repository:
   ```bash
   git add .
   git commit -m "Deploy to GitHub Pages"
   git push origin main
   ```

3. GitHub Actions will automatically build and deploy the blog to GitHub Pages.
