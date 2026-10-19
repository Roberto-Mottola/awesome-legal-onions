# Methodology

How [Umbrixa](https://umbrixa.com) builds and maintains this index of legitimate onion services.

## What we index

Only sites whose content is legal and falls into one of our categories: privacy and security tools, journalism and whistleblowing, politics and civil rights, technology, community and forums, academic resources, anonymous services, media and culture.

## What we never index

Marketplaces of any kind, carding and fraud, drugs, weapons, CSAM or any content involving minors, malware and exploit kits, phishing and scams, crypto investment and doubler schemes, doxing and data leaks, mixers and money-laundering services, hitman and violence, hate forums, and link directories that aggregate the above. These are rejected and blacklisted.

## The pipeline

1. **Discovery.** Candidates come only from trusted references: vouched clearnet sources, authoritative directories (e.g. the SecureDrop directory), and outbound links from sites we have already verified. We do not mass-scrape the Tor graph, because it is dominated by illegal markets.
2. **Moderation gate.** A deterministic deny-list blocks known illegal and scam patterns outright. Everything else goes through an AI classifier with a conservative policy: anything that looks like a market, shop, escrow, mixer, carding, crypto scam or a link directory is a violation. When content cannot be read or identity cannot be positively established, the site is held as *suspect*, not published.
3. **Verification & uptime.** Sites are fetched over Tor and re-checked on a schedule. Availability is tracked; persistently dead sites are dropped.
4. **Trust signals.** Where a service also runs a public clearnet mirror, we record it. A real-world identity on the ordinary web is one of the strongest signals that an onion service is genuine.

## Data freshness

This repository is regenerated daily from the live index. Figures and listings change as the index grows and as sites go up or down. The public listing excludes thin entries (generic titles, empty or error-page descriptions); the full index is searchable at umbrixa.com.

## Corrections

To report an error, a site that should be removed, or a missing service, open an issue or write to info@umbrixa.com.
