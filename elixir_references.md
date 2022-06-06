# Elixir refences

[Elixir Casts](https://elixircasts.io/)

[Thinging Elixir](https://thinkingelixir.com/)

[Elixir X Erlang Compatibility](https://hexdocs.pm/elixir/1.12/compatibility-and-deprecations.html)

### Blog posts/gists

https://dennisbeatty.com/cool-clis-in-elixir-with-io-write-2.html

https://gist.github.com/jdesilvio/7972ff3274e85b37dd933aca6d3bab22

https://zorbash.com/post/building-command-line-applications-with-elixir/

https://stackoverflow.com/questions/47783996/format-date-with-elixir

https://stackoverflow.com/questions/56941063/elixir-how-to-cast-from-string-to-ecto-date

### Mongodb

In case you are trying to run a task, you have to ensure that there is an application running:
````
Application.ensure_all_started(:mongodb)
{:ok, conn} = Mongo.start_link(url: "mongodb://127.0.0.1:27017/yourdb")
````
https://elixirforum.com/t/starting-mongo-inside-a-mix-task/28164
