# Security, Cost & Operations

## AWS billing incident: 20M KRW in 5 days

- Link: https://pointer81.tistory.com/entry/AWS-5%EC%9D%BC%EA%B0%84-2000%EB%A7%8C%EC%9B%90-%EB%B9%84%EC%9A%A9-%EC%82%AC%EC%9A%A9%EA%B8%B0
- Type: Cloud cost / operational safety case study
- Why it matters:
  - AI agents, automated scripts, and accidental credential leaks can create expensive failures quickly.
  - CFD/ML workloads often involve cloud GPUs, storage, and long-running jobs, so cost controls matter.
- Practical reminders:
  - Never commit secrets.
  - Use billing alerts and hard budget notifications.
  - Prefer least-privilege credentials.
  - Be careful with automated agents that can create, scale, or push infrastructure changes.
