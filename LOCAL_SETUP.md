# Local Development Setup

## Prerequisites

Install Ruby via Homebrew (if not already installed):
```bash
brew install ruby
```

## Setup

1. **Add Ruby to PATH** (add to `~/.zshrc` or `~/.bash_profile`):
```bash
export PATH="/opt/homebrew/opt/ruby/bin:/opt/homebrew/lib/ruby/gems/3.4.0/bin:$PATH"
```

2. **Install dependencies** (one-time setup):
```bash
bundle install
```

## Running the Site

Start the Jekyll server:
```bash
bundle exec jekyll serve
```

Access the site at: **http://localhost:4000**

Stop the server with `Ctrl+C`.

## Optional: Enable Image Optimization

Install ImageMagick and enable in `_config.yml`:
```bash
brew install imagemagick
# Set imagemagick: enabled: true in _config.yml
```

## Deploying

Push changes to GitHub:
```bash
git add .
git commit -m "Your message"
git push origin master
```

Site will be live at https://hcagri.github.io in 1-2 minutes.

