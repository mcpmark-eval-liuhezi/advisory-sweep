# Security advisory sweep

## Lookup filters

- **Source:** GitHub global security advisories
- **Ecosystem:** `npm`
- **Severity:** `critical` and `high` (two separate lookups, results combined)
- **Type:** reviewed advisories (default)

The strict high/critical filters returned results, so no widening was required. The five most
recent advisories returned across those two lookups are recorded below (ordered most recent
first).

## Advisories

### GHSA-qx66-fv34-fjm8

- **Package(s):** `@tanstack/start-server-core`, `@tanstack/react-start`, `@tanstack/solid-start`, `@tanstack/vue-start`
- **Severity:** critical (CVSS 9.3)
- **Summary:** An unauthenticated attacker can craft a link to a TanStack Start server function that makes the app return attacker-controlled HTML from its own origin, running the attacker's JavaScript with the visitor's access.

### GHSA-x34j-47hf-4xg7

- **Package(s):** `tinacms`, `@tinacms/app`
- **Severity:** critical (CVSS 9.3)
- **Summary:** The TinaCMS admin preview iframe trusts an attacker-controlled origin derived from the URL fragment, so a single malicious link opened by a logged-in editor gives a remote attacker read/write access to the site's content API.

### GHSA-pq7j-f95f-qfcv

- **Package(s):** `@anthropic-ai/claude-code`
- **Severity:** high
- **Summary:** Claude Code's plugin installer failed to verify that the checked-out commit matched the pinned hash, so a SHA-named branch could silently install attacker-controlled code instead of the reviewed commit.

### GHSA-x586-xvc8-g7q6

- **Package(s):** `@builder.io/qwik`, `@qwik.dev/core`
- **Severity:** high
- **Summary:** A single unauthenticated HTTP request with a crafted qwik-json body triggers an unhandled promise rejection that crashes a Qwik server in its default configuration.

### GHSA-2vc4-c4r6-p6v6

- **Package(s):** `@opennextjs/cloudflare`
- **Severity:** high (CVSS 7.5)
- **Summary:** With cache interception enabled, a percent-encoded request path can skip authorization middleware during matching and then be decoded to hit the cache of a protected route, exposing cached content.
