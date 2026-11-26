## Prosper Okah

Computer Engineering student at the University of Lagos. I build backend and systems software (storage engines, a rate-limiting server, market-data tooling, concurrent services) and do smart contract security research.

- **Systems:** C++20 and Python. LSM-tree storage, order-book replay, async services that stay correct under retries and concurrent load.
- **Security:** independent auditor on Code4rena and HackenProof (7 valid findings, including high severity); wrote a [detection module](https://github.com/OWASP/Nettacker/pull/1476) for [OWASP Nettacker](https://github.com/OWASP/Nettacker) covering the Next.js middleware auth bypass (CVE-2025-29927, on CISA's Known Exploited list).
- **Competitive programming:** ICPC, top 4.5%.

### Selected projects

| Project | What it is | Numbers |
|---|---|---|
| [ratelimitd](https://github.com/Dami99-b/ratelimitd) | Rate-limiting server in C++20: GCRA over a sharded key store, one epoll event loop per CPU, speaks the Redis protocol | 2.0M decisions/s pipelined, 11.5x Redis + Lua; 37 tests under ASan, UBSan and TSan |
| [MicroFS](https://github.com/Dami99-b/MicroFS) | LSM-tree key-value store in C++20 with a WAL, SSTables, Bloom filters, compaction and a TickStore API for market data | 1.2M reads/s at p99 1.3 µs; 27/27 tests under ASan/UBSan |
| [lob-backtester](https://github.com/Dami99-b/lob-backtester) | Limit-order-book backtester on market-by-order data (ITCH 5.0), with latency, queue position, fees and Deflated Sharpe | Numba replay ~9M msgs/s |
| [distributed-file-storage-engine](https://github.com/Dami99-b/distributed-file-storage-engine) | File storage backend: presigned S3 uploads, content-addressed dedup, background workers | streaming SHA-256 at ~130 MB/s, flat memory |
| [async-idempotency-engine](https://github.com/Dami99-b/async-idempotency-engine) | Redis-backed idempotency layer for FastAPI with a circuit breaker, deployed to Kubernetes with Terraform and Ansible and monitored with Prometheus and Grafana | 1,000 concurrent duplicates → exactly one charge; 0 failed requests through a pod kill and a rolling restart |

### Tools

C++ · Python · Rust · TypeScript · FastAPI · PostgreSQL · Redis · NumPy / Numba · Docker · Kubernetes · Terraform · Ansible · Prometheus · Grafana · Linux · GitHub Actions

### Contact

[Portfolio](https://prosperokah.vercel.app) · [LinkedIn](https://www.linkedin.com/in/prosper-okah-150672372) · [LeetCode](https://leetcode.com/u/damillz)

Looking for software engineering and quant developer internships for 2027.
