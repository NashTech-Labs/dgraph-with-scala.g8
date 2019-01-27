A [Giter8][g8] template for DGraph with Scala!

# How to use
---
You can import the template using
`sbt new knoldus/dgraph-with-scala.g8`

You will need to install DGraph on your local machine for using this template. For information on how to install DGraph, please refer to [Let's Start Exploring Dgraph: How to get started](https://blog.knoldus.com/lets-start-exploring-dgraph-how-to-get-started/).

The application picks two values from configuration, the host for DGraph and it's port. For local machines, the following exports would work -

```
export DGRAPH_HOST="localhost"
export DGRAPH_PORT="9080"
```

Then all you will have to do is run the project, you can use the following command for doing so -

`sbt run`

The application will -
- Create a connection to the DGraph using the host and port provided through the environment variables.
- Create a schema. Schema could be found in the file `schema.conf` present in the `resources` folder.
- Mutate some data in DGraph. It will be evident what is getting mutated in the main file of the application, i.e., `Boot.scala`.
- Read some data from DGraph.
- Delete the read data.
- Read the data again to confirm deletion.

Hope this template comes in handy and you find it useful. Please reach out to me at - **akshansh.jain@knoldus.in** in case of any queries.

# Template license
----------------
Written in 2019 by [Knoldus Inc.](http://www.knoldus.com)

To the extent possible under law, the author(s) have dedicated all copyright and related
and neighboring rights to this template to the public domain worldwide.
This template is distributed without any warranty. See <http://creativecommons.org/publicdomain/zero/1.0/>.

[g8]: http://www.foundweekends.org/giter8/
