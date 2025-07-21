# Project Deployment

This repository is structured for deployment to GitHub and Cloudflare Pages.

## Structure
```
/
├── .gitignore
├── .env.example
├── package.json
├── netlify.toml
├── functions/
└── public/
    ├── css/
    ├── js/
    ├── images/
    ├── json/
    ├── index.html
    └── ... other html pages
```

### Deployment
1. Push to GitHub.
2. In Cloudflare Pages dashboard, connect to this repo.
3. Set build command: `npm install && npm run build` (if you have build process) or leave blank for static.
4. Set output directory: `public`.
5. Add environment variables from `.env.example` as needed.
