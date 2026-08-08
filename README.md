# kota.fo

Static landing page for `kota.fo`. It has no build step or runtime dependencies.

## Preview locally

From this directory, run:

```sh
python3 -m http.server 8080
```

Then open `http://localhost:8080`.

## Deploy to Cloudflare Pages

### Direct upload

1. Open Cloudflare Dashboard > Workers & Pages.
2. Select Create > Pages > Upload assets.
3. Use `kota-fo` as the project name.
4. Upload this directory.
5. Open the project, then Custom domains, and add `kota.fo`.
6. Add `www.kota.fo` too if both domain variants should work.

### Git deployment

Push this directory to a GitHub or GitLab repository. In Cloudflare Pages,
connect that repository with these settings:

- Framework preset: None
- Build command: leave empty
- Build output directory: `/`

Every push to the production branch will then deploy automatically.
