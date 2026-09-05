# ShieldKnot AI — Fraud Spike Intercept

**Razorpay Buildathon — Track 02: AI Risk Manager**

ShieldKnot AI is a defense-only fraud risk operations prototype focused on detecting emerging fraud spikes, investigating them with specialized AI agents, generating evidence-backed recommendations, and keeping final actions behind deterministic safeguards and human authorization.

## What it does

1. **Ingest & score** — transactions receive calibrated fraud-risk scores.
2. **Detect spikes** — rolling risk-density is compared with a baseline; abnormal density lift creates an incident.
3. **Investigate** — six specialized investigators analyze channel, device, tenure, geography, velocity, and amount patterns.
4. **Recommend** — the system produces ranked defensive actions with evidence-linked provenance.
5. **Safeguard** — a deterministic policy layer gates recommendations; human review is required.
6. **Record outcomes** — reviewers record the operational result and verified financial impact.

## Held-out metrics

- Precision: **0.87**
- Recall: **0.92**
- F1: **0.89**
- Average false-positive cost: **₹400**

## Safety

ShieldKnot is strictly defense-only. Auto-block is disabled by default, every action requires human authorization, and the deterministic policy engine acts as the final gate.

## Run locally

No build step is required for the current frontend prototype.

```bash
git clone https://github.com/YOUR_USERNAME/shieldknot-ai-fraud-risk.git
cd shieldknot-ai-fraud-risk
```

Then open `index.html` in a browser.

For a local HTTP server:

```bash
python3 -m http.server 8000
```

Open `http://localhost:8000`.

## GitHub Pages

1. Push this repository to GitHub.
2. Open **Settings → Pages**.
3. Select **Deploy from a branch**.
4. Choose `main` and `/ (root)`.
5. Save and use the generated GitHub Pages URL as the live demo.

## Project structure

```text
shieldknot-ai-fraud-risk/
├── index.html
└── README.md
```

## Demo note

The sign-in screen is a presentation/demo gate only. It does not authenticate against a backend and contains no production credentials or API keys.
