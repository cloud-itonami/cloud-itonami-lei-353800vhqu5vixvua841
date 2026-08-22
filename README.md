# cloud-itonami-lei-353800vhqu5vixvua841

> **Independent third-party archive/analysis. Not affiliated with, endorsed by, or sponsored by ＮＴＴ株式会社.**

Archives the publicly published NTT Group Privacy Policy / Social Media Policy of **ＮＴＴ株式会社** (Nippon
Telegraph and Telephone Corporation), with source-url and retrieval-date provenance, per ADR-2607110300.
Read-only reference/archive repository — not a governed Advisor/Governor actor.

Part of the **worldwide-scope extension** of the cloud-itonami-lei catalog (batch JP-UTIL-1, 2026-07-19).
Note: the corporate site www.ntt.co.jp returns HTTP 410 Gone (migrated); the current group site group.ntt
is the source of record.

## Company identity

- **Legal name**: ＮＴＴ株式会社 (NTT, Inc.; renamed 2025-07-01 from 日本電信電話株式会社 / Nippon Telegraph and Telephone Corporation — see `facts/catalog.edn`)
- **LEI (ISO 17442)**: [353800VHQU5VIXVUA841](https://search.gleif.org/#/record/353800VHQU5VIXVUA841) (GLEIF entity-verified, JP)
- **Jurisdiction**: JP
- **Website**: https://group.ntt
- **Ticker**: 9432 (TSE Prime)
- **ISIC Rev.5**: 6110 (wired telecommunications)

## Contents

- `80-data/public/tos.journal.edn` — EDN quad-log of the archived policy text.
  Its recorded `:tos/source-url` (`https://group.ntt/en/privacy/social.html`) is
  still live — checked by row `issuer-social-policy` in `facts/catalog.edn`.
- `NOTICE` — copyright/attribution statement.
- `blueprint.edn` — machine-readable company identity record.
- `facts/catalog.edn` — 41 live-checked citations across five independent
  authorities (GLEIF, Japan NTA corporate-number site, METI gBizINFO, US SEC
  EDGAR, the issuer), each with a `:cite/row-kind` stating what it does and
  does not prove. Includes the 2025-07-01 rename (日本電信電話株式会社 →
  ＮＴＴ株式会社) as recorded by GLEIF and the NTA.
- `tools/verify_citations.cljs` — the gate: every citation must answer HTTP 2xx
  and carry its expected substring. Run
  `nbb tools/verify_citations.cljs facts/catalog.edn --min 13`
  (exit 0 = all checked and clean, 1 = drift, 2 = could not answer).

## Design rationale

See ADR-2607110300 and the worldwide-scope extension ledger in `com-junkawasaki/root` (`90-docs/adr/`).
