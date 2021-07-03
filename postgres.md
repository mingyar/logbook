# ** (DBConnection.ConnectionError) tcp connect (localhost:5432): connection refused
```
21:01:08.023 [error] GenServer #PID<0.384.0> terminating
** (DBConnection.ConnectionError) tcp connect (localhost:5432): connection refused - :econnrefused
    (db_connection 2.4.0) lib/db_connection/connection.ex:100: DBConnection.Connection.connect/2
    (connection 1.1.0) lib/connection.ex:622: Connection.enter_connect/5
    (stdlib 3.15.1) proc_lib.erl:226: :proc_lib.init_p_do_apply/3
Last message: nil
State: Postgrex.Protocol

** (Mix) The database for App couldn't be created: killed
```

https://qastack.com.br/programming/12472988/postgresql-error-could-not-connect-to-server-no-such-file-or-directory

Check if there's no postmaster.pid on your postgres directory, probrably: ```/usr/local/var/postgres/```, remove it and restart the server.
