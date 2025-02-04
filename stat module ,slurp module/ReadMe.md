# Ansible `stat` vs `slurp` Modules

## `stat` Module
The `stat` module is useful for verifying file metadata, such as checking if a file exists, its permissions, owner, group, and timestamps. This is commonly used for tasks like:
- File verification
- Conditional actions based on file properties
- Backup verification

### Example Use Case:
You might use the `stat` module to check whether a configuration file exists before backing it up or applying any changes.

## `slurp` Module
The `slurp` module is useful for fetching the contents of a file, especially when you need to process or inspect the file’s data, such as:
- Parsing logs
- Transferring file contents across systems

It returns the file content as a base64-encoded string, which can then be decoded and used in subsequent tasks.

### Example Use Case:
You might use the `slurp` module to fetch the contents of a log file, then process it to look for specific error messages or other events.
