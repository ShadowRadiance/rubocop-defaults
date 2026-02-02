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

## Note About Inherited Remote Files

- the inherited yml files are cached under "rubocop_cache" under the `AllCops/CacheRootDirectory`.
- if the `AllCops/CacheRootDirectory` is nil (`~`), it will default to:
  - `$XDG_CACHE_HOME`, then to `$HOME/.cache/`
- so with nothing defined the default is `$HOME/.cache/rubocop_cache`
