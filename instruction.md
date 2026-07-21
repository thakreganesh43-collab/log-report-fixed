You need to generate a structured JSON report from the provided log data. The output must be written to the absolute path /app/report.json.

Success criteria:

1. A file named report.json must be created at /app/report.json.
2. The file must contain valid JSON that can be parsed without error.
3. The JSON must include the top-level keys "summary" and "entries".
4. The "entries" key must map to a non-empty list of log records.
5. The "summary" key must include a "total" field whose value equals the number of items in "entries".
