# Riwayat adittamavincent-my-id

## 2026-11-15T08:50+07:00 — Domain live with HTTPS

- **Permintaan:** Check after Vincent updated DNS at idwebhost.
- **Dikerjakan:** Checked DNS at ns1.idwebhost.id, 1.1.1.1 and 8.8.8.8: apex A 75.2.60.5, www CNAME adittamavincent.netlify.app. Waited for Netlify to issue the certificate.
- **Hasil:** https://adittamavincent.my.id returns HTTP/2 200 with the current page. Let's Encrypt certificate covers apex and www and expires 2027-02-13. http and www redirect 301 to https://adittamavincent.my.id/.
- **Terbuka:** `PERSONAL/` folder still not listed in the hub AGENTS.md repo map.

## 2026-11-15T08:35+07:00 — Personal homepage, GitHub, Netlify

- **Permintaan:** Simple personal website (plain HTML, almost no CSS) inspired by "Hayyoth", public GitHub repo under adittamavincent, linked to Netlify via CLI, domain adittamavincent.my.id, production. Content: about me, showcase links, email.
- **Dikerjakan:** "Hayyoth" could not be found (youtube.com/@hayyoth 404, github.com/hayyoth 404, hayyoth.com no DNS, web search no match); Vincent chose a plain style instead. Bio drafted from the public GitHub profile and public non-fork repos. After review Vincent asked for a shorter page, Times New Roman, contact as "Email" and "Instagram: eezaatee", and no Sewon Family Dev mention. Installed netlify-cli with Homebrew; Vincent signed in with `netlify login`.
- **Hasil:** `index.html`, `netlify.toml`, `README.md`, `AGENTS.md`. Public repo https://github.com/adittamavincent/adittamavincent-my-id (main). Netlify project `adittamavincent` (https://adittamavincent.netlify.app), linked to the repo through a read-only deploy key plus a GitHub push webhook (manual git setup; the Netlify GitHub App was not installed). Custom domain adittamavincent.my.id with alias www.adittamavincent.my.id set in Netlify. First production deploys are ready.
- **Keputusan:** Plain style, public email adittamavincent@gmail.com, Instagram eezaatee, no Sewon Family Dev mention.
- **Terbuka:** DNS at idwebhost still points to GitHub Pages IPs and 103.169.142.0. Vincent must set apex A 75.2.60.5 and www CNAME adittamavincent.netlify.app, then Netlify issues HTTPS. New `PERSONAL/` folder is not yet listed in the hub AGENTS.md repo map.
