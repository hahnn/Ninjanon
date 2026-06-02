# NinjAnon
NinjAnon is a database anonymization solution based on the Dalibo anon extension. The goal of this code is to provide an open source solution able to anonymize any database hosted on any database engine having a matching PostgreSQL Foreign Data Wrapper.

One of the goals of NinjAnon is to be able to be used by any DBA dealing with pure SQL commands only inside PostgreSQL psql tool. It's designed to not be a huge gas factory or complicated product.

# Mandatory dependencies
NinjAnon is fully coded using PlPgsql and SQL.
It also needs the anon (from Dalibo), pgcrypto and pg_cron PostgreSQL addons or extensions.
And of course, you will need to deploy those FDWs: oracle_fdw, mysql_fdw, tds_fdw (for MSSQL), mongo_fdw and postgres_fdw.

# Optionnal dependencies
NinjAnon is a sub-project of the main PGNinja project.
PGNinja is an optionnal dependency (well, it WILL become an optionnal dependency at some point in the future) as it will provide a graphical interface for NinjAnon which is web based. But for now it's not there yet as this still needs to be developped and integrated to PGNinja. We are focused on the development of the core features of NinjAnon for now.

# Installation
In your PostgreSQL server, create a database called ninjanon.
Then play the PostgreSQL files provided:
ninjanon.schema
ninjanon_small.data
ninjanon_last_name.data
ninjanon_avs.data.gz (uncompress before)
ninjanon_streets_fra1.data.gz (uncompress before)
ninjanon_streets_fra2.data.gz (uncompress before)
ninjanon_streets_fra3.data.gz (uncompress before)
ninjanon_streets_fra4.data.gz (uncompress before)

Note for myself: more installation instructions will be provided

