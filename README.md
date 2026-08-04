# Luke Documentation

Public how-to documentation for **Luke, from The Direction Company**.

Luke is used through approved communication channels. This repository is a reference surface only: it does not provide a customer account, dashboard, settings interface, billing interface, support portal, integration manager, or second AI assistant.

## Public-content boundary

Only material approved for public release belongs here. Do not copy internal roadmap material, implementation notes, security-sensitive architecture, customer data, credentials, private prompts, model reasoning, unannounced pricing, or unsupported capability claims from the private Luke product repository.

## Local development

Install the pinned Mint CLI version used by CI:

```bash
npm install --global mint@4.2.748
```

Run the site locally:

```bash
mint dev --no-open
```

Validate before opening a pull request:

```bash
mint validate
mint broken-links --check-anchors --check-redirects --check-snippets
mint a11y
```

## Publishing

The Mintlify deployment reads this repository's `main` branch from the repository root. Documentation changes should use pull requests, pass the repository checks, and receive the required owner review before merge.

The Mintlify AI assistant is disabled. Documentation must direct operational actions back to Luke in the approved communication channel or to an exact third-party provider handoff sent by Luke.
