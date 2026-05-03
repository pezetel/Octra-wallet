# octra wallet generator

## quick start

**download and start wallet generator web UI with a single command:**

**linux/macOS:**
```bash
curl -fsSL https://octra.org/wallet-generator.sh | bash
```

**windows:**
```powershell
powershell -c "irm octra.org/wallet-generator.ps1 | iex"
```

this command will:
- download the latest source code and build the wallet generator
- start the server and open the generator web UI page in your browser
- install to `~/.octra/wallet-generator` for future use

## browser-only version (no install)

a fully client-side build lives in [`public/`](./public). open `public/index.html`
directly in a browser, or deploy the `public/` folder as a static site
(e.g. on vercel — `vercel.json` is configured to serve it without a build step).
the wallet is generated entirely in the browser using `crypto.subtle` +
bundled `bip39` and `tweetnacl`; nothing is sent to a server.

## request testnet tokens

https://faucet.octra.network
