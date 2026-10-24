# Supreme Reporters — Netlify starter

A blue-and-white, responsive digital news website built with Astro. It includes article pages, category pages, homepage features, basic search, About, Contact, Privacy and Editorial Policy pages.

## Before publishing
1. Replace the placeholder contact email in `src/pages/contact.astro`.
2. Review the About, Privacy and Editorial Policy pages and replace starter wording with your actual policies.
3. Add real, verified articles and images. The supplied welcome story is a draft and is not displayed publicly.
4. If you choose a custom domain, update `site` in `astro.config.mjs`.

## Deploy to Netlify
1. Create a GitHub account at https://github.com/.
2. Create a new repository named `supreme-reporters`.
3. Upload the contents of this project folder (not the ZIP file itself) to the repository.
4. In Netlify, choose **Add new project → Import an existing project → GitHub**.
5. Select the repository. Build command: `npm run build`. Publish directory: `dist`.
6. Deploy. Netlify provides a `*.netlify.app` URL. A production deploy currently costs 15 credits on credit-based plans; bandwidth and requests also use credits. Check your usage dashboard before repeated production deploys.

## Article publishing dashboard
This starter uses Pages CMS, a hosted editor that signs in with GitHub and edits the article files in your repository:
1. Open https://app.pagescms.org/ and sign in with GitHub.
2. Install/authorise the Pages CMS GitHub App for your `supreme-reporters` repository.
3. Open that repository. Pages CMS reads the `.pages.yml` configuration included here.
4. Open **News articles**, create an article, fill in headline, summary, publication date, author, section and article body.
5. Set **Keep as draft** to `false` when it has been edited and approved for publication. Mark only one story as **Feature on homepage** if you want it to lead.
6. Save/commit the change to the publishing branch (normally `main`). Netlify detects the GitHub update and rebuilds the site automatically.
7. After the deployment succeeds, open your Netlify URL and check the article.

Pages CMS is an external, free/open-source editing service. It is separate from Netlify. It does not require Netlify Identity or Git Gateway. You must sign in with GitHub and grant access to the correct repository.

## Credit-saving tips
- Keep the site static; this avoids server functions and a database for the basic news workflow.
- Use Deploy Previews to test changes where possible; Netlify documents previews as not consuming credits.
- Production deploys cost 15 credits each on current credit-based plans. At 400 credits, that is about 26 production deploys before bandwidth and requests are counted (400 / 15 = 26 full deploys with 10 credits left).
- Compress images before uploading. Netlify bandwidth is metered.
- Never share GitHub passwords, Netlify passwords, access tokens or recovery codes in chat.

## Important
This package is a deployable starter, not an already-published website. You must connect your own GitHub and Netlify accounts to activate it. Pages CMS publishing requires the repository and permissions to be configured as described above.
