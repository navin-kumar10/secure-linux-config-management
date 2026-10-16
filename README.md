# 07. Secure Linux and Configuration Management

![architecture](docs/architecture.png)

**Ansible - Linux - NGINX** | *Phase 1 - Beginner foundations* | `lab` - verify before production use.

> Ansible hardening: SSH, patching, NGINX+TLS, firewall, repeatable builds. Vagrant/Docker lab included.

## Architecture

```mermaid
flowchart LR
  Control[Ansible] --> Roles[base-ssh-nginx-fw] --> Hosts
```

Full diagram: [docs/architecture.png](docs/architecture.png) - Design: [docs/architecture.md](docs/architecture.md)

## Structure

```
.
+-- app/
+-- terraform/ or infrastructure/
+-- monitoring/
+-- tests/
+-- runbooks/
+-- docs/architecture.md, architecture.png, cost-estimate.md
+-- .github/workflows/
```

## Quickstart (lab)

```bash
git clone https://github.com/navin-kumar10/secure-linux-config-management.git
cd secure-linux-config-management
make validate
make plan
make apply
make smoke
make destroy
```

See [runbooks/DEPLOYMENT.md](runbooks/DEPLOYMENT.md), [runbooks/ROLLBACK.md](runbooks/ROLLBACK.md), [docs/cost-estimate.md](docs/cost-estimate.md).

## Implementation order

10-project portfolio. Order: Phase 1 (04,07,09) -> Phase 2 (03,04,05) -> Phase 3 (01) -> Phase 4 (02) -> Phase 5 (08,09,10).

## License

MIT - see LICENSE.
