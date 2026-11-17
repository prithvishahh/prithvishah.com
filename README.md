# prithvishah.com

Personal site for Prithvi Shah. It is one static page, styled like a market terminal: a command line, a quote header, and panels for projects, research, resume, and contact.

Type a mnemonic and press Enter. `PROJ`, `RSRCH`, `RESUME`, `ABOUT`, `CONTACT`, `HELP`, and `HIRE` switch screens. Function keys F1–F9 do the same.

## Local preview

From the repository root:

```bash
python3 -m http.server 8080
```

Open http://localhost:8080. The resume file is at http://localhost:8080/resume.pdf.

## Deploy on Vercel

1. Import this repository in the Vercel dashboard.
2. Framework preset: Other. Leave the build command and install command empty. There is no build step.
3. The site is the repository root: `index.html`, `favicon.svg`, and `resume.pdf`.
4. Attach the domain `prithvishah.com`.

`vercel.json` enables `cleanUrls` so routes do not need a `.html` suffix. Nothing is compiled.
