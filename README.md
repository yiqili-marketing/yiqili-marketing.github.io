# Yiqi Li academic website

A simple three-page academic site made for GitHub Pages. It uses only HTML and CSS, so there is nothing to install or build.

## Personalize the site

1. Open `index.html` and replace every phrase in square brackets. Change `your.email@example.com` in the Contact me link to your real email address. The Education section already contains the degree information supplied from the reference screenshot; update the expected year when needed.
2. Open `research.html`, `teaching.html`, and `cv.html` and replace the placeholder entries. Copy and paste an `<article class="item-card">...</article>` block to add more publications, papers, or courses.
3. Create an `images` folder and place your portrait inside it as `portrait.jpg`.
4. In `index.html`, replace the `portrait-placeholder` block with:

   ```html
   <img src="images/portrait.jpg" alt="Portrait of Yiqi Li">
   ```

5. To change colors, edit the values at the top of `styles.css` under `:root`.

You can preview the site by double-clicking `index.html`.

## Publish with GitHub Pages — easiest browser method

1. Sign in at [github.com](https://github.com) and select the **+** menu, then **New repository**.
2. Name the repository `yourusername.github.io`, replacing `yourusername` with your exact GitHub username. Make it **Public**, leave the other options unchanged, and select **Create repository**.
3. On the repository page, choose **uploading an existing file**. Drag in `index.html`, `research.html`, `teaching.html`, `cv.html`, `styles.css`, and your `images` folder if you added one.
4. Enter a short message such as `Add personal website`, then choose **Commit changes**.
5. Open **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**. Select the `main` branch and `/ (root)`, then choose **Save**.
6. After a few minutes, visit `https://yourusername.github.io`.

If you prefer a project repository with another name, the process is the same, but the address will be `https://yourusername.github.io/repository-name/`.

## Publish with Git instead

After creating an empty GitHub repository, open a terminal in this folder and run:

```sh
git init
git add index.html research.html teaching.html cv.html styles.css README.md images
git commit -m "Add academic website"
git branch -M main
git remote add origin https://github.com/yourusername/yourusername.github.io.git
git push -u origin main
```

If you have not added an `images` folder yet, omit `images` from the `git add` line. Then enable Pages using step 5 above.

## Add a custom domain later

1. Buy or keep a domain from any registrar.
2. In the repository, open **Settings → Pages** and enter the domain under **Custom domain**. GitHub will create the required `CNAME` file.
3. At your domain registrar, add the DNS records GitHub shows. For a domain such as `www.example.com`, this is usually a `CNAME` record pointing `www` to `yourusername.github.io`. Root domains use GitHub's published `A`/`AAAA` records.
4. Wait for GitHub's DNS check to succeed, then turn on **Enforce HTTPS**.

DNS changes can take time to spread. Follow GitHub's current Pages custom-domain documentation when you are ready, since DNS values and registrar screens can change.
