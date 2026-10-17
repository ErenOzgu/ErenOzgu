<h1 align="center">Hi, I'm Eren 👋</h1>

<p align="center">
  <b>Test, integration and DevOps</b> · legacy system modernization · automation and AI
</p>

<p align="center">
  <a href="https://github.com/ErenOzgu/legacy-modernizer-mcp">
    <img src="https://raw.githubusercontent.com/ErenOzgu/legacy-modernizer-mcp/main/docs/banner.svg" alt="legacy-modernizer-mcp" width="100%">
  </a>
</p>

## About me

- I work in test, integration and DevOps in the defense industry. Right now I focus on improving internal processes and structures in a digital transformation team.
- I work on modernizing legacy Python 2.7 / Django codebases, CI/CD and test automation, and AI-assisted automation.
- I like combining technical leadership with hands-on delivery: working with board-level stakeholders and shipping the work in the field.
- Working languages: Turkish, English (upper advanced).

## Projects

Most of these are tested in CI against the real software (Asterisk, Ubuntu, Django, Wireshark) rather than mocks.

### Voice and telecom

| Project | Description |
|---|---|
| [**Dev-Ops (RNVCS)**](https://github.com/ErenOzgu/Dev-Ops) | An Asterisk-based voice communication system: zero-dependency Go services, a SIP/RTP engine, PostgreSQL and CI/CD with canary deployments. Starts with one Docker Compose command; verified on GitHub Actions with end-to-end tests against a real PostgreSQL. |
| [**asterisk-gcp-iac**](https://github.com/ErenOzgu/asterisk-gcp-iac) | Terraform and Ansible for a hardened Asterisk PBX on Google Cloud: SSH only through IAP, nftables, fail2ban, Prometheus metrics. CI builds the Terraform plan without credentials and checks it against policy rules, then applies the Ansible roles twice on real Ubuntu 22.04 and 24.04. |
| [**sip-regression**](https://github.com/ErenOzgu/sip-regression) | SIPp scenarios and a Python runner that put a real Asterisk through 22 checks: registration, calls, audio, hostile packets, load. Ten deliberately broken PBX configurations must fail them. |
| [**asterisk-exporter**](https://github.com/ErenOzgu/asterisk-exporter) | A Go exporter with no third-party dependencies that turns the Asterisk Manager Interface into Prometheus metrics. Comes with a Grafana dashboard and unit-tested alert rules; verified in CI against real Asterisk 18 and 20. |
| [**asterisk-conf-lint**](https://github.com/ErenOzgu/asterisk-conf-lint) | A security linter for Asterisk configuration files: open AMI, endpoints without passwords, weak secrets, toll-fraud dialplans. 25 rules, no dependencies, checked against real Asterisk 18 and 20. |
| [**rtp-quality**](https://github.com/ErenOzgu/rtp-quality) | Jitter, packet loss and estimated MOS from pcap and pcapng captures of RTP, as text, JSON or Prometheus metrics. No dependencies; its numbers are checked against Wireshark and a real SIPp call. |

### Linux, CI and modernization

| Project | Description |
|---|---|
| [**legacy-modernizer-mcp**](https://github.com/ErenOzgu/legacy-modernizer-mcp) | An MCP server that scans legacy Python 2 / Django projects, ranks the findings and drafts a migration plan. 52 rules, read-only analysis, tested in CI. |
| [**django-upgrade-lab**](https://github.com/ErenOzgu/django-upgrade-lab) | A small Django 1.11 project upgraded to 5.2 one LTS at a time. The upgrade is the git history: every stage is a commit that CI installs and tests on the Python version it was meant for. |
| [**ubuntu-hardening-roles**](https://github.com/ErenOzgu/ubuntu-hardening-roles) | Nine Ansible roles that harden Ubuntu 22.04 and 24.04, and a read-only audit script. CI converges real machines, checks that a second run changes nothing, then breaks things on purpose and expects the audit to notice. |
| [**minimal-rootfs**](https://github.com/ErenOzgu/minimal-rootfs) | A bootable Ubuntu 22.04 or 24.04 root file system built with debootstrap (about 185 MB). CI boots it in QEMU and fails if it grows past a size budget. |

### Other

| Project | Description |
|---|---|
| [**D-etud**](https://github.com/ErenOzgu/D-etud) | An education platform where students ask teachers questions: React front end, Node.js/MongoDB API, JWT and Socket.IO. |

## Tools

![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?logo=go&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?logo=django&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black)
![Ubuntu](https://img.shields.io/badge/Ubuntu-E95420?logo=ubuntu&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?logo=gnubash&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?logo=git&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?logo=githubactions&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?logo=node.js&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?logo=react&logoColor=black)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?logo=mongodb&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white)
![Asterisk](https://img.shields.io/badge/Asterisk-F68F1E)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?logo=terraform&logoColor=white)
![Ansible](https://img.shields.io/badge/Ansible-EE0000?logo=ansible&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)
![QEMU](https://img.shields.io/badge/QEMU-FF6600?logo=qemu&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?logo=grafana&logoColor=white)
![Google Cloud](https://img.shields.io/badge/Google_Cloud-4285F4?logo=googlecloud&logoColor=white)

## Currently learning

- Google Cloud and cloud architecture
- AI-assisted automation and building tools with MCP
