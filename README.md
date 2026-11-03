# Nuvio Ecosystem Directory

A lightweight, responsive, single-page static directory. No framework, package manager, build step, external font, analytics, or third-party JavaScript is required.

## Files
- `index.html` — complete directory page
- `favicon.svg` — site icon
- `robots.txt` — allows normal crawler access
- `404.html` — friendly not-found page

## Publish with GitHub Pages
1. Create a public GitHub repository (for example, `nuvio-ecosystem-directory`).
2. Upload all files in this folder to the repository root. Ensure the main page is named `index.html`.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**, choose `main` and `/ (root)`, then Save.
5. Wait for the Pages deployment and open the URL shown in Settings → Pages.
6. In the Pages settings, enable **Enforce HTTPS** when available.

## Before launch
- Review the project URLs. The page reflects the supplied reference document; not every community repository or live deployment has been independently verified.
- If using a custom domain, add a canonical URL and `og:url` after the final domain is known. Create a sitemap with the actual published URL and add its location to `robots.txt`.
- Add an Open Graph preview image (for example, `og-image.png`) and corresponding `og:image` / `twitter:image` metadata if social sharing previews are desired.
- GitHub Pages does not provide arbitrary custom response headers. If you need a custom Content-Security-Policy or other headers, use a host that supports header configuration (such as Cloudflare Pages) and configure them there.

## Quality checks
- HTML is static and content is present without JavaScript (progressive enhancement).
- Theme selection, directory search, mobile section navigation, and back-to-top are enhanced with small vanilla JavaScript.
- Test keyboard navigation, screen-reader output, colour contrast, 320–400 px widths, and real device browsers before claiming WCAG conformance.
- Run the deployed URL through Lighthouse / PageSpeed Insights and the W3C Nu HTML Checker. Core Web Vitals require field data after deployment; they cannot be guaranteed from the source file alone.
