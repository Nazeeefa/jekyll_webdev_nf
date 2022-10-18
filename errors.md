- adding webrick: https://github.com/jekyll/jekyll/issues/8523
- adding `exclude: [vendor]` in _config.yml to resolve error "welcome-to-jekyll.markdown.erb does not have valid date" [Source](https://github.com/jekyll/jekyll/issues/5267)
- How to switch to ruby version: https://www.moncefbelyamani.com/how-to-install-xcode-homebrew-git-rvm-ruby-on-mac/#how-to-install-different-versions-of-ruby-and-switch-between-them
- commands: <br>
  ` bundle exec jekyll serve`
  `jekyll new .`
  `bundle install`
  `bundle add webrick`
  `jekyll serve -l`
- If i18n is being used, mention specific version:
  `~> 0.9.5` means ['>= 0.9.5', '< 0.10.5']
  `>= 0.9.5` ['>= 0.9.5', inf]
- If running `jekyll serve -l` says anything about plugin versions e.g. i18n, resolve as:
  remove version `"~> 227",` from `gem "github-pages", "~> 227", group: :jekyll_plugins`
  So: `gem "github-pages", group: :jekyll_plugins` solves it.