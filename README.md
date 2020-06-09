# dotnetsqlite
The [example from microsoft](https://docs.microsoft.com/en-us/dotnet/standard/data/sqlite/?tabs=visual-studio) with a readme that covers [Jade](https://rhildred.github.iol/jade).

In this repo do `dotnet run`. The first time you will get this error but it will create the hello.db file in the current folder:

```
Unhandled exception. Microsoft.Data.Sqlite.SqliteException (0x80004005): SQLite Error 1: 'no such table: user'.
   at Microsoft.Data.Sqlite.SqliteException.ThrowExceptionForRC(Int32 rc, sqlite3 db)
   at Microsoft.Data.Sqlite.SqliteCommand.PrepareAndEnumerateStatements(Stopwatch timer)+MoveNext()
   at Microsoft.Data.Sqlite.SqliteCommand.GetStatements(Stopwatch timer)+MoveNext()
   at Microsoft.Data.Sqlite.SqliteDataReader.NextResult()
   at Microsoft.Data.Sqlite.SqliteCommand.ExecuteReader(CommandBehavior behavior)
   at Microsoft.Data.Sqlite.SqliteCommand.ExecuteReader()
   at Jun9sqlitedotnet.Program.Main(String[] args) in /Volumes/esgaroth/source/repos/Jun9sqlitedotnet/Program.cs:line 24
```

1. Open the hello.db using the [Jade editor](https://rhildred.github.io) and create the user table with a row. 
2. Save the hello.db from Jade into your Downloads folder. 
3. Move it over top of the hello.db that you copied in step 1.
4. `dotnet run` and you should see something like:

```

rhildred@Richs-Mac-mini Jun9sqlitedotnet % dotnet run
Hello, Rich!
rhildred@Richs-Mac-mini Jun9sqlitedotnet %

```


