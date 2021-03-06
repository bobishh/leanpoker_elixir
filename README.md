# LeanpokerElixirPlayer

Leanpoker Player API for Elixir

Main Player file is lib/leanpoker_elixir/player.ex

## Heroku:

1. Create an app with build pack
    ```
      heroku create --buildpack "https://github.com/HashNuke/heroku-buildpack-elixir.git"
    ```

2. Change config if needed (elixir_buildpack.config)
    ```
      # Erlang version
      erlang_version=18.1

      # Elixir version
      elixir_version=1.1.1

      # Always rebuild from scratch on every deploy?
      always_rebuild=false

      # Export heroku config vars
      config_vars_to_export=(DATABASE_URL)

      # A command to run right after compiling the app
      post_compile="pwd"
    ```
3. Push to heroku
    ```
      git push heroku master
    ```

[buildpack github link](http://github.com/HashNuke/heroku-buildpack-elixir)
