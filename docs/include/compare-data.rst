::

   pgcopydb compare data: Compare source and target data
usage: pgcopydb compare data  --source ... --filters <file>

The command ``pgcopydb compare data`` connects to the source and target
databases and computes a checksum of the data found in each table. The
checksums are then compared and pgcopydb outputs a list of tables that
have the same checksum on both nodes, and a list of tables that have
different checksums.

.. option:: --source <PGURI>

   Postgres URI to the source database.

.. option:: --target <PGURI>

   Postgres URI to the target database.

.. option:: --dir <path>

   Work directory to use.

.. option:: --table-jobs <count>

   Number of concurrent jobs to run to compare table data.

.. option:: --filters <file>

   Path to a file containing filtering rules.

.. option:: --json

   Format the output using JSON.
