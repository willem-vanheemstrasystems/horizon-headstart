# horizon-headstart
Horizon - Headstart

See also http://horizon.io/docs/getting-started/

# Sample application

We already created a new Horizon application by running:

hz init example_app

 (If you run hz init without giving it a directory, it will install these files into the current directory.)

Here’s what these files and directories are:

- dist is for static files. You can create files directly here, or use it as the output directory for a build system of your choice.

- src is for source files for your build system. This isn’t a convention you have to follow; Horizon doesn’t touch anything in this directory.

- dist/index.html is a sample file. You’ll replace this as you develop your application, but there’s enough in it to verify that Horizon is installed and working.

- .hz/config.toml is a TOML configuration file for the Horizon server.

# Start the server

Start Horizon to test it out, from within the root directory run:

hz serve example_app--dev

NOTE: If you receive following error: 
  serve failed with Error: `rethinkdb` not found in $PATH, please install RethinkDB.

  then added the path to RethinkDB to your environment variable PATH.

NOTE: If you receive following error:
  serve failed with Error: RethinkDB (2.2.4) is below required version (2.3.0) for use with Horizon.

  then upgrade to RethinkDB version 2.3.0.

You can now see the index page of the example_app at http://127.0.0.1:8181/

