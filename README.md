# Rubocop Defaults

These are the defaults I like to be available in all my projects.

Example for a Rails app with Rspec

```yml
# .rubocop.yml
inherit_from:
  - https://raw.githubusercontent.com/ShadowRadiance/rubocop-defaults/refs/heads/main/.rubocop-defaults.yml
  - https://raw.githubusercontent.com/ShadowRadiance/rubocop-defaults/refs/heads/main/.rubocop-rails-defaults.yml
  - https://raw.githubusercontent.com/ShadowRadiance/rubocop-defaults/refs/heads/main/.rubocop-rspec-defaults.yml
```

Example for a Rails app with Minitest

```yml
# .rubocop.yml
inherit_from:
  - https://raw.githubusercontent.com/ShadowRadiance/rubocop-defaults/refs/heads/main/.rubocop-defaults.yml
  - https://raw.githubusercontent.com/ShadowRadiance/rubocop-defaults/refs/heads/main/.rubocop-minitest-defaults.yml
  - https://raw.githubusercontent.com/ShadowRadiance/rubocop-defaults/refs/heads/main/.rubocop-rails-defaults.yml
```
