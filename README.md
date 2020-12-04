# bufu - Minimal file uploader CLI for Snowflake stage

`bufu` is a minimal file uploader CLI for Snowflake stage.

**Important Note: it is not a Snowflake official software.**

# Install

`$ pip install bufu`

# Configuration

`bufu` automatically uses `[connections]` section in `~/.snowsql/config` to setup a connection.

Database, schema and warehouse are mandatory to use `bufu`.

# Usage

`bufu show` ... List up all stages in the current schema
`bufu show <stage>` ... List up first 100 files in the stage

`bufu create <stage>` ... Create a stage in the current schema

`bufu put <file>` ... Create a stage starting with "bufu_" and put the file to the stage
`bufu put <file> <schema>` ... Put the file to the stage
