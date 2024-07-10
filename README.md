# Luigi utils

Utils for https://github.com/emerald-geomodelling/poltergust and https://github.com/spotify/luigi

# Filesystem access

`poltergust_luigi_utils.caching.CachingOpenerTarget` like `luigi.contrib.opener.OpenerTarget` but caches the file locally (forever, cleaning the cache directory must be done by  a cron job).

`poltergust_luigi_utils.gcs_opener` adds support for Google Cloud Storage targets (`gs://bucket/file` style url:s) to `luigi.contrib.opener.OpenerTarget`

# Logging

`poltergust_luigi_utils.logging_task.LoggingTask` mixin class for `luigi.Task` that integrates with the python logging framework to log task activity to a luigi target.

# Scheduler communication

`poltergust_luigi_utils.luigi_client.LuigiTaskClient` client to check status and progress of a task with the central scheduler.

# Poltergust client

`poltergust_luigi_utils.poltergust_pipeline_client.PoltergustPipelineClient` client library to submit tasks to Poltergust (by writing the config files) and to retrieve status, progress and logs from tasks.
