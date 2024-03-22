
This was done by: 

- From these lines (from [here](https://jekyllrb.com/)): 

```sh
gem install bundler jekyll
jekyll new my-awesome-site
cd my-awesome-site
bundle exec jekyll serve
# => Now browse to http://localhost:4000
```

- Push to github
- Repo -> settings -> Pages. Source: 'Deploy from branch. Select branch: 'main'.
- Will take a few seconds to build (via a Github Actions-like background process (look for the yellow 'running' icon next to the commit)
- Site will be live at: https://<username>.github.io/<reponame>/
- Pretty sure the base url had to be altered for the site to find the css
  - In `_config.yml`, change baseurl: from "" to "/reponame" (/ at the start, no / at the end)
  - Commit and push to github
  - Now css should work


