### moonsc112-afk

Security researcher — smart contracts & web/API authorization surfaces.

I hunt bugs the report-driven way: read the program's rubric and scope first, map
the intended security model, then test whether every route, tool, and token type
enforces the same checks — and prove it with a working PoC.

**Focus**
- Smart contracts: EVM (Solidity/Vyper) & Solana (Anchor) — authorization,
  accounting & rounding, oracle manipulation, reentrancy, privilege escalation,
  loss-of-funds paths.
- Web / API / OAuth / MCP: org & tenant scoping, token-type confusion, IDOR,
  allowlist bypass, confirmation-gate TOCTOU, SSRF, query scoping.

**Method**
- PoC-first, not scanner output.
- Impact quantified against the program's own severity rubric.
- Rule-compliant: test only what I own, low volume, stop at proof, minimal
  redacted evidence, coordinated disclosure.

**Tooling**
- EVM: Foundry · slither · echidna · medusa · solc-select
- Solana: Anchor / Agave · on-chain PoC against deployed bytecode
- Web/OAuth/MCP: curl + browser harnesses · custom JSON-RPC / PKCE clients
- AI-agent-assisted recon & evidence; account-side actions kept manual

**Activity**
- Bug bounty on HackenProof.

> Pinning reproducible PoCs and disclosed writeups here as they go public.
