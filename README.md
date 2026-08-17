# Theo Leburu

Computer engineering student in Botswana, working in cybersecurity and software development.

## Security projects

**[security-posture-scanner](https://github.com/TheoLeburu/security-posture-scanner)** — Grades a website's HTTP header and TLS configuration from A to F and gives a remediation step for every finding. Five weighted checks, where a single critical finding caps the grade instead of being averaged away by the clean ones.

**[auth-log-analyser](https://github.com/TheoLeburu/auth-log-analyser)** — Finds brute-force attempts, credential spraying and successful compromises in SSH and web authentication logs. Six detection rules run over one normalised event model, so supporting a new log format means writing a parser and changing no rules.

Both are Python. Each is a dependency-free engine with a CLI and an HTTP API as separate interfaces onto it, so the analysis can run in a cron job or behind a dashboard without changing.
