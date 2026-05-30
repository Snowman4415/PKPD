# PMxAIBot — PK/PD Pharmacometric AI Assistant

> An AI-powered chatbot for pharmacokinetics, pharmacodynamics, and pharmacometrics — hosted at **pharmconsulting.net**

![PMxAIBot](https://img.shields.io/badge/PMxAIBot-PK%2FPD%20AI-1D9E75?style=flat-square)
![GitHub Pages](https://img.shields.io/badge/Hosted%20on-GitHub%20Pages-0F6E56?style=flat-square)
![Model](https://img.shields.io/badge/Powered%20by-Claude%20Sonnet-5DCAA5?style=flat-square)

## Features

- Compartmental PK modeling (1-cmt, 2-cmt, 3-cmt; IV, oral, infusion)
- Non-compartmental analysis (NCA): AUC, Cmax, t½, CL, Vd, MRT
- PD models: Emax, sigmoid Emax, indirect response, effect compartment
- Population PK/PD: NONMEM, Monolix, nlmixr2, covariate modeling
- PBPK, DDI, organ impairment, allometric scaling
- Therapeutic drug monitoring (TDM) and Bayesian dosing
- Bioequivalence, pediatric PK, software guidance (R, NONMEM, Phoenix)

## Deployment

### 1. Enable GitHub Pages

1. Go to your repository: `https://github.com/Snowman4415/PKPD`
2. Click **Settings** → **Pages** (left sidebar)
3. Under **Source**, select `Deploy from a branch`
4. Set branch to `main`, folder to `/ (root)`
5. Click **Save**

Your site will be live at: `https://Snowman4415.github.io/PKPD`

### 2. Connect pharmconsulting.net

In your domain registrar (where you manage pharmconsulting.net):

Add these DNS records:

| Type  | Host | Value                         |
|-------|------|-------------------------------|
| A     | @    | 185.199.108.153               |
| A     | @    | 185.199.109.153               |
| A     | @    | 185.199.110.153               |
| A     | @    | 185.199.111.153               |
| CNAME | www  | Snowman4415.github.io         |

Then in GitHub Pages settings, set **Custom domain** to `pharmconsulting.net` and check **Enforce HTTPS**.

### 3. Set Your API Key

When you open the app, you'll be prompted to enter your Anthropic API key (`sk-ant-...`).  
The key is stored only in your browser's localStorage — it never leaves your device.

Get your API key at: https://console.anthropic.com/

## Tech Stack

- Pure HTML/CSS/JS — zero dependencies, no build step
- Anthropic Claude Sonnet API
- GitHub Pages hosting

## License

For educational and research use. Not intended for clinical decision-making.
