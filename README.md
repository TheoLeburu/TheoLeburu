# Theo Leburu

Computer engineering student in Botswana, working in cybersecurity and software development.

## Security projects

**[security-posture-scanner](https://github.com/TheoLeburu/security-posture-scanner)** — Grades a website's HTTP header and TLS configuration from A to F and gives a remediation step for every finding. Five weighted checks, where a single critical finding caps the grade instead of being averaged away by the clean ones.

**[auth-log-analyser](https://github.com/TheoLeburu/auth-log-analyser)** — Finds brute-force attempts, credential spraying and successful compromises in SSH and web authentication logs. Six detection rules run over one normalised event model, so supporting a new log format means writing a parser and changing no rules.

Both are Python. Each is a dependency-free engine with a CLI and an HTTP API as separate interfaces onto it, so the analysis can run in a cron job or behind a dashboard without changing.

## Software

**[quote-to-invoice](https://github.com/TheoLeburu/quote-to-invoice)** — Quotes, invoices and automated payment chasing for small businesses: branded PDFs, a private link the client accepts from, and reminders that escalate at 3, 14 and 30 days overdue. No float touches a monetary value — amounts are integer cents rounded half up per line, and a document discount is spread proportionally across lines so the per-rate VAT breakdown stays correct. Reminders cannot double-send, because that guarantee lives in a database constraint rather than a flag the code has to remember. Python, Flask and SQLite; 134 tests.
