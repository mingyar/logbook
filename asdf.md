# Adding a plugin
````
asdf plugin-add elixir https://github.com/asdf-vm/asdf-elixir.git
````
# All available versions
````
asdf list-all erlang
````
# Installing a specific version
````
asdf install elixir 1.9.4-otp-22
````
# Activating versions
````
asdf local/global erlang 22.1.7
asdf local/global elixir 1.9.4-otp-22
````
# The difference between local and global
* global – used everywhere by your user
* local – used specifically for the current directory
# Dont forget to clean up after change versions
````
mix do clean, compile
````
https://thinkingelixir.com/install-elixir-using-asdf/
