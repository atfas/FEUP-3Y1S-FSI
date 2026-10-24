# FSI — Fundamentos de Segurança Informática

Lab logbooks for **FSI (Fundamentos de Segurança Informática / Fundamentals of Computer Security)** at FEUP, 3rd year, 1st semester (2025/2026). Group project (class T09, group 05).

Each logbook documents one hands-on security lab, most of them based on the [SEED Labs](https://seedsecuritylabs.org/), with the commands we ran, the code we wrote or modified, screenshots of every step and an explanation of why each attack works.

## Contents

| Logbook | Topic | Summary |
|---|---|---|
| [LOGBOOK2](LOGBOOK2.md) | CVE-2015-0310 | Analysis of an Adobe Flash Player ASLR-bypass vulnerability: identification, cataloguing, exploits and attacks |
| [LOGBOOK4](LOGBOOK4.md) | Environment Variables & Set-UID | How environment variables reach child processes, `PATH` / `LD_LIBRARY_PATH` abuse, Set-UID privilege escalation and capability leaking |
| [LOGBOOK5](LOGBOOK5.md) | Buffer Overflow (Set-UID) | Stack smashing with ASLR disabled to inject shellcode and get a root shell |
| [LOGBOOK6](LOGBOOK6.md) | Format String Vulnerability | Crashing the server, reading stack and heap memory, and writing arbitrary values through `printf` |
| [LOGBOOK7](LOGBOOK7.md) | Cross-Site Scripting (Elgg) | Stored XSS on a social network: stealing cookies and forcing victims to send friend requests just by viewing a profile |
| [LOGBOOK9](LOGBOOK9.md) | Secret-Key Encryption | Frequency analysis on a substitution cipher; AES in ECB, CBC and CTR modes and how each handles corrupted ciphertext |
| [LOGBOOK10](LOGBOOK10.md) | Hash Length Extension | Forging a valid MAC for an extended request without knowing the secret key |
| [LOGBOOK11](LOGBOOK11.md) | Public Key Infrastructure | Becoming a root CA, issuing certificates, deploying HTTPS on Apache and a MITM attack with a compromised CA |
| [LOGBOOK13](LOGBOOK13.md) | Packet Sniffing & Spoofing | Sniffing and spoofing packets with Scapy in a Docker network |

## Repository structure

```
.
├── LOGBOOK*.md        # one report per lab
└── Images/
    └── logbook<N>/    # screenshots referenced by each logbook
```

## Environment

The labs were run on the SEED Ubuntu VM, using the Docker-based lab setups provided by SEED (`docker-compose build` / `docker-compose up`). Each logbook starts with the environment setup it needs (disabling ASLR, `/etc/hosts` entries, containers, etc.).

## Team

- Afonso Saraiva
- Daniel Marques
- Inês Francisco

---

Originally developed on FEUP's GitLab ([t09-group05](https://gitlab.up.pt/class/fsi/2526/t09/t09-group05)) and mirrored here with full commit history.
