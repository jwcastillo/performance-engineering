# perf-engineering

A Claude Code skill for end-to-end performance engineering: strategy, test design, execution, analysis, and optimization.

## What It Does

- **Load/Stress/Soak/Spike testing** with JMeter and k6
- **CI/CD performance gates** — automate perf tests in GitHub Actions pipelines
- **Database optimization** — index strategy, caching patterns, execution plan analysis
- **Memory leak detection** — soak testing, heap analysis, common leak patterns
- **Cloud perf testing** — AWS/GCP distributed load generation, cost optimization
- **Monitoring & observability** — Prometheus/Grafana dashboards, bottleneck decision tree
- **Core Web Vitals** — LCP, CLS, INP, TTFB optimization
- **Mobile API performance** — API-based testing via Fiddler/Charles + JMeter

## Install

```bash
claude skill install github.com/khanntm/perf-engineering
```

## Key Metrics

| Layer | Metrics |
|-------|---------|
| **API** | Response time (p50/p95/p99), throughput (TPS), error rate |
| **Web** | LCP, CLS, INP, TTFB, bundle size |
| **Mobile API** | API response time (p95), payload size, burst concurrency |
| **Database** | Query time (p95), connection pool, cache hit ratio, slow queries |
| **System** | CPU%, memory%, disk I/O, network I/O, connection pool |

## References (13 files)

### Testing & Tools
- JMeter enterprise patterns & best practices
- k6 modern load testing (load/stress/spike/soak scripts)
- Performance reporting templates

### Optimization & Analysis
- Database performance (PostgreSQL index types, EXPLAIN ANALYZE, Redis caching)
- Memory leak detection (Node.js/Java patterns, heap snapshots)
- Web performance (Core Web Vitals)
- Mobile API testing (Fiddler → JMeter workflow)

### Infrastructure & Monitoring
- Cloud perf testing (AWS EC2/ECS/EKS, GCP GKE/Cloud Run)
- CI/CD integration (GitHub Actions for k6 + JMeter)
- Monitoring & observability (Prometheus/Grafana, APM, alerting)

### Real-World Experience
- Enterprise insurance app lessons: STP bottleneck, CPU right-sizing, 12h soak test, AWS cost optimization

## License

Apache-2.0
