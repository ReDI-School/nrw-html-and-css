source "https://rubygems.org"

ruby '3.2.2'

# To upgrade, run `bundle update github-pages`.
gem "github-pages", group: :jekyll_plugins

install_if -> { RUBY_PLATFORM =~ %r!mingw|mswin|java! } do
  gem "tzinfo", "~> 1.2"
  gem "tzinfo-data"
end

# Performance-booster for watching directories on Windows
gem "wdm", "~> 0.1.0", :install_if => Gem.win_platform?

gem "webrick", "~> 1.7"
