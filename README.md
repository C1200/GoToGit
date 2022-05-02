# GoToGit

A JS Forwarder to Github inspired by [byemc/gitforwarder](https://github.com/byemc/gitforwarder).

## URL Formats

- Profile: https://example.com/
- Repo: https://example.com/:repo
- Branch: https://example.com/:repo/:branch
- Path: https://example.com/:repo/:branch/:path[0]/path[1]/:path[n]

## How to use

1. Fork this repo
2. Setup Github Pages
3. If you are using the default Github pages URL (Example: `https://<username>.github.io/<repo>`):
   1. Delete the `CNAME` file
   2. Set `PATH_SEGMENTS_TO_SKIP` to 1 in `404.html`
4. If you have your own domain:
   1. Configure your DNS to work with Github Pages
   2. Change the content of the `CNAME` file to your (sub)domain
5. Set `GIT_URL` in `404.html` to your Github user link (Example: `https://github.com/<username>`)
   1. Do not add a trailing `/`!
6. You're all set!

---

License: [MIT](LICENSE)