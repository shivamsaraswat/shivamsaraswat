<div align="center">

```
┌──────────────────────────────────────────────────────────────────┐
│  SHIFT LEFT  ·  SUPPLY CHAIN SECURITY  ·  DEVEX-FIRST APPSEC     │
└──────────────────────────────────────────────────────────────────┘
```

</div>

# Hey, I'm Shivam 👋

**Senior Product Security Engineer @PayPal**

*Security that developers actually want to use — not security they route around.*

[![PayPal](https://img.shields.io/badge/PayPal-Security%20Engineering-003087?style=flat-square&logo=paypal&logoColor=white)](https://paypal.com)
[![Blog](https://img.shields.io/badge/Blog-blog.shivamsaraswat.com-black?style=flat-square)](https://blog.shivamsaraswat.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-shivamsaraswat-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/shivamsaraswat)
[![Twitter](https://img.shields.io/badge/X-thecybersapien-000?style=flat-square&logo=x&logoColor=white)](https://twitter.com/thecybersapien)

---

## The Origin Story

I got into security through automation, not through breaking things by hand. My first job was building the scanners and detection logic that other people's pentest findings fed into — and that vantage point taught me something early: a finding that lives in a PDF report is a finding that gets fixed once and forgotten. The same class of bug would resurface in a different repo six months later. The vulnerability wasn't the real problem. The **workflow** around it was.

That's the thread running through everything I've built since — at IKEA, at Tekion, and now at PayPal: if a security control creates friction, developers will find a way around it, and the org is worse off than if the control never existed. So instead of shipping policies, I ship *platforms* — things that sit inside the pipelines developers already use, catch what matters, and stay quiet about the rest.

---

## The Problem I Keep Solving

```
   DEVELOPERS                    SECURITY TEAM
   ──────────                    ─────────────
   "Ship the feature,           "Block anything
    the deadline is Friday"      non-compliant"
        │                              │
        └──────────── FRICTION ────────┘
                        │
                        ▼
          alert fatigue · shadow IT · shipped anyway
                        │
              I build the layer in between:
        gateways, not gatekeepers · signal, not noise
                        │
                        ▼
        SECURE BY DEFAULT, INVISIBLE UNTIL IT MATTERS
```

Alert fatigue is the real enemy, not the CVE count. A scanner that cries wolf on every transitive dependency trains people to ignore it — and then it misses the one that matters. Most of my work is about **compression**: taking a firehose of findings and turning it into the handful of things a developer needs to act on today.

---

## Currently Building (PayPal)

| Area | What it does |
|---|---|
| 🛡️ **Supply Chain Firewall** | A gateway upstream of Artifactory that blocks malicious and stale packages before they ever reach a developer's machine |
| 📦 **Container Security at Scale** | Policy enforcement across 3K+ pipelines, standardized so "compliant" means the same thing everywhere |
| 🧬 **Vulnerability Deduplication Engine** | Collapses CVE/package/version noise across scanners using image-layer analysis, so one real issue doesn't become five tickets |
| 🤖 **AI-Powered SCA** | Reachability analysis and fix-suggestion prototypes to kill false positives and point straight to the safe upgrade path |

One of the more interesting weeks this year: catching and neutralizing **Shai-Hulud**, a self-replicating npm worm, along with a handful of concurrent supply-chain campaigns — before they could steal credentials or spread through build environments.

---

## Stack

```
AppSec & Supply Chain      Container / Cloud         Automation & Detection
──────────────────────     ─────────────────         ───────────────────────
Semgrep · CodeQL           Trivy · Wiz · JFrog Xray   Python · Bash
Dependabot · Renovate      Docker · Kubernetes        GitHub Actions
Syft (SBOM)                GCP · AWS                  GitLab CI/CD
Gitleaks · GHAS            Nuclei · ZAP · Burp        Harness CI/CD
```

---

## Open Source & Personal Projects

| Project | What it is |
|---|---|
| [**SeCoRA**](https://github.com/shivamsaraswat/SeCoRA) | An LLM-driven secure code review agent — OWASP Top 10 / SANS 25 detection, vulnerability chaining, CVSS-scored remediation reports |
| [**VulnSort**](https://github.com/shivamsaraswat/VulnSort) | A GitHub Action + CLI that reprioritizes scan results by real exploitability (CISA KEV, EPSS) instead of raw CVSS |
| [**PkgSafe**](https://github.com/shivamsaraswat/PkgSafe) | A quick web tool to check whether an open-source package is carrying malware |
| [**certify**](https://github.com/shivamsaraswat/certify) | Checks the health of a domain's SSL/TLS certificate posture |

Most of these exist because I got tired of asking "does a tool for this already exist?" and just built the version I wanted.

---

## Writing

I write about the gap between "the scanner found it" and "the developer fixed it" — shift-left tooling, supply chain security, and what it actually takes to get 700 teams to care about security without forcing them to.

🔗 [blog.shivamsaraswat.com](https://blog.shivamsaraswat.com/)

---

## Let's Talk

If you're working on supply chain security, container security, or building security tooling people don't hate — open an issue, or find me on [LinkedIn](https://www.linkedin.com/in/shivamsaraswat).

---

*"A control nobody uses isn't a control — it's a checkbox."*

<br>

<div align="center">
<img src="https://komarev.com/ghpvc/?username=shivamsaraswat&label=Profile%20views&color=0e75b6&style=flat" alt="profile views" />
</div>

<br>

<div align="center">
<a href="https://www.buymeacoffee.com/cybersapien"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" height="50" width="210" alt="cybersapien" /></a>
</div>
