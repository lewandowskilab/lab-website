<h1 align="center">Lewandowski Lab Website</h1>

<p align="center">
<a href="https://lewandowskilab.github.io/lab-website/"><b>🌐 https://lewandowskilab.github.io/lab-website/</b></a>
</p>

The website for the Lewandowski Lab. It publishes automatically: edits pushed to
`main` are built by GitHub Actions and deployed to the live site above.

## Editing

- **Visual editor (recommended):** open [`/admin`](https://lewandowskilab.github.io/lab-website/admin/)
  and sign in with GitHub. All pages, members, publications, projects, blog
  posts, and Lab Life items are edited through forms — no code needed.
- **Editor's guide:** see [`Editing-Reference.md`](Editing-Reference.md) for what
  each page/section does and how ordering, images, and publications work.

## How it works

- Built on the Greene Lab [Lab Website Template](https://github.com/greenelab/lab-website-template) (Jekyll).
- Publications and citations are generated automatically from identifiers
  (DOI, PubMed, ORCID, …) by Manubot on every push.
- Push to `main` → GitHub Actions runs `update-citations` → `build-site` →
  deploys to the `gh-pages` branch, which serves the live site.

## Credits

Based on the Greene Lab [Lab Website Template](https://github.com/greenelab/lab-website-template)
([documentation](https://greene-lab.gitbook.io/lab-website-template-docs)).
