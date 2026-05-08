# OrbitDesk

OrbitDesk is a hard Red Team CTF machine packaged as a single Docker target.

## Run

```bash
docker compose up --build
```

If Compose is not installed:

```bash
docker build -t orbitdesk .
docker run --rm -p 8080:8080 -p 2222:22 orbitdesk
```

Target services:

- Web: `http://127.0.0.1:8080`
- SSH: `127.0.0.1:2222`

Flags use the `HackCTF{}` format.

## Player Brief

OrbitDesk is an operations support portal used by a managed services team. The public console exposes ticket and vendor preview workflows, while deployment synchronization and backup automation are expected to be internal-only.

The objective is to obtain both flags.

## Notes

This image intentionally contains vulnerabilities for an isolated lab. Do not expose it to an untrusted network.
# Machine
