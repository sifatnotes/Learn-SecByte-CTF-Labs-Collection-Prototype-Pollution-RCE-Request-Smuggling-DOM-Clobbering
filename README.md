# Learn-SecByte-CTF-Labs-Collection-Prototype-Pollution-RCE-Request-Smuggling-DOM-Clobbering
A curated collection of hands-on cybersecurity CTF labs covering Prototype Pollution to RCE, HTTP Request Smuggling, DOM Clobbering, Browser Cache Poisoning, and Open Redirects from Learn SecByte.
# Learn SecByte CTF & Cybersecurity Labs Collection

Welcome to the **Learn SecByte CTF & Cybersecurity Labs Collection**. This repository is a dedicated, searchable index of hands-on Advanced Client-Side Web Vulnerabilities (Prototype Pollution to RCE, DOM Clobbering, Tabnabbing, Clickjacking UI Redress, Cross-Origin Misconfigurations), Server & Protocol Desynchronization (HTTP Request Smuggling, HTTP Response Splitting, Host Header Injection), Web & Browser Cache Poisoning (Browser Cache Poisoning, Vary-based Cache Poisoning), and Input Validation & Authentication Misconfigurations (Open Redirects, Default Admin Panel Access) labs designed for cybersecurity students, CTF players, application security engineers, bug bounty hunters, penetration testers, and security research trainees.

---

## Table of Contents
- [Introduction](#introduction)
- [Lab Collection & Index](#lab-collection--index)
- [Categories](#categories)
- [Learning Path](#learning-path)
- [How to Use the Labs](#how-to-use-the-labs)
- [Disclaimer](#disclaimer)

---

## Introduction

Modern web security requires mastering both low-level client-side JavaScript execution environments and front-end/back-end proxy protocol desynchronization. Hosted on [Learn SecByte](https://learn.secbyte.org/), this advanced client-side web exploitation, HTTP protocol desynchronization, cache poisoning, and authentication misconfiguration collection provides practical, hands-on technical training to audit, exploit, and remediate complex web infrastructure and browser-level vulnerabilities.

From polluting Object prototypes in Node.js to achieve Remote Code Execution (RCE) and overriding DOM attributes via DOM Clobbering to desynchronizing HTTP front-end/back-end request boundaries, injecting CRLF sequences for HTTP Response Splitting, poisoning web and browser cache layers via unkeyed headers, abusing `target="_blank"` for reverse tabnabbing, constructing clickjacking UI redress overlays, and auditing default admin panel credentials, these exercises build complete web application security tradecraft.

---

## Lab Collection & Index

Below is the complete, searchable index of all client-side JavaScript vulnerabilities, HTTP protocol smuggling, cache poisoning, and authentication misconfiguration challenges in this collection:

| # | Lab / Challenge Name | Category | Focus / Key Topics | Lab Link |
|---|----------------------|----------|---------------------|----------|
| 1 | **Prototype Pollution to RCE** | Advanced Client-Side JavaScript & Browser Exploitation | Object prototype manipulation (`__proto__`), property injection in Node.js runtime, gadget chain exploitation, remote code execution | [Access Lab](https://learn.secbyte.org/ctf/prototype-pollution-to-rce) |
| 2 | **DOM Clobbering: Learning Room** | Advanced Client-Side JavaScript & Browser Exploitation | Overriding global JavaScript variables/DOM objects using HTML elements (`id`/`name` attributes), logic bypass, XSS payload execution | [Access Lab](https://learn.secbyte.org/ctf/dom-clobbering-learning-room) |
| 3 | **Tabnabbing: Trusted Tabs, Untrusted Targets** | Advanced Client-Side JavaScript & Browser Exploitation | Unsanitized `target="_blank"` link exploitation, `window.opener.location` redirection, phish-over-tab credential harvesting | [Access Lab](https://learn.secbyte.org/ctf/tabnabbing-trusted-tabs-untrusted-targets) |
| 4 | **Clickjacking: UI Redress and Interface Manipulation** | Advanced Client-Side JavaScript & Browser Exploitation | Transparent iframe overlays, CSS positioning manipulation, unauthorized action execution, frame-busting bypasses | [Access Lab](https://learn.secbyte.org/ctf/clickjacking-ui-redress-and-interface-manipulation) |
| 5 | **Cross-Origin Misconfiguration** | Advanced Client-Side JavaScript & Browser Exploitation | Insecure CORS policies (`Access-Control-Allow-Origin`), null origin reflection, authenticated cross-origin data extraction | [Access Lab](https://learn.secbyte.org/ctf/cross-origin-misconfiguration) |
| 6 | **HTTP Request Smuggling: Front-End Confusion Lab** | Server & Protocol Desynchronization Attacks | CL.TE and TE.CL request desynchronization, Transfer-Encoding header obfuscation, request queue hijacking, response splitting | [Access Lab](https://learn.secbyte.org/ctf/http-request-smuggling-front-end-confusion-lab) |
| 7 | **HTTP Response Splitting: Header Injection & Cache Poisoning** | Server & Protocol Desynchronization Attacks | CRLF (`\r\n`) injection in response headers, HTTP header splitting, persistent web cache poisoning, XSS injection | [Access Lab](https://learn.secbyte.org/ctf/http-response-splitting-header-injection-cache-poisoning) |
| 8 | **Host Header Injection: From Discovery to Defense** | Server & Protocol Desynchronization Attacks | Unvalidated `Host` header processing, password reset token poisoning, SSRF via host headers, virtual host brute-forcing | [Access Lab](https://learn.secbyte.org/ctf/host-header-injection-from-discovery-to-defense) |
| 9 | **Browser Cache Poisoning: When the Browser Trusts Too Much** | Web & Browser Cache Poisoning | Unkeyed response header exploitation, static asset browser cache contamination, persistent client-side payload execution | [Access Lab](https://learn.secbyte.org/ctf/browser-cache-poisoning-when-the-browser-trusts-too-much) |
| 10 | **Cache Poisoning: From Varying Responses to Exploitation and Defense** | Web & Browser Cache Poisoning | Unkeyed header injection (`X-Forwarded-Host`/`X-Original-URL`), `Vary` header manipulation, web cache contamination, persistent XSS | [Access Lab](https://learn.secbyte.org/ctf/cache-poisoning-from-varying-responses-to-exploitation-and-d) |
| 11 | **Open Redirect: Trust Boundary Failures** | Input Validation & Authentication Misconfigurations | Unvalidated parameter redirection (`url=`, `next=`), phishing trust boundary abuse, OAuth state flow interception | [Access Lab](https://learn.secbyte.org/ctf/open-redirect-trust-boundary-failures) |
| 12 | **Default Admin Panel** | Input Validation & Authentication Misconfigurations | Factory default administrative credentials, administrative interface exposure, unauthenticated portal takeover | [Access Lab](https://learn.secbyte.org/ctf/default-admin-panel) |

---

## Categories

### 1. Advanced Client-Side JavaScript & Browser Exploitation
Exploit JavaScript Object prototypes in Node.js to achieve RCE, override global DOM variables via HTML clobbering, hijack open window references with tabnabbing, construct clickjacking UI overlays, and exploit insecure cross-origin policies.
- [Prototype Pollution to RCE](https://learn.secbyte.org/ctf/prototype-pollution-to-rce)
- [DOM Clobbering: Learning Room](https://learn.secbyte.org/ctf/dom-clobbering-learning-room)
- [Tabnabbing: Trusted Tabs, Untrusted Targets](https://learn.secbyte.org/ctf/tabnabbing-trusted-tabs-untrusted-targets)
- [Clickjacking: UI Redress and Interface Manipulation](https://learn.secbyte.org/ctf/clickjacking-ui-redress-and-interface-manipulation)
- [Cross-Origin Misconfiguration](https://learn.secbyte.org/ctf/cross-origin-misconfiguration)

### 2. Server & Protocol Desynchronization Attacks
Desynchronize front-end reverse proxies and back-end web servers using CL.TE/TE.CL HTTP request smuggling, inject CRLF characters for response splitting, and manipulate host headers for password reset poisoning.
- [HTTP Request Smuggling: Front-End Confusion Lab](https://learn.secbyte.org/ctf/http-request-smuggling-front-end-confusion-lab)
- [HTTP Response Splitting: Header Injection & Cache Poisoning](https://learn.secbyte.org/ctf/http-response-splitting-header-injection-cache-poisoning)
- [Host Header Injection: From Discovery to Defense](https://learn.secbyte.org/ctf/host-header-injection-from-discovery-to-defense)

### 3. Web & Browser Cache Poisoning
Contaminate intermediate web caches and local client browser caches by injecting unkeyed headers and manipulating HTTP response behavior.
- [Browser Cache Poisoning: When the Browser Trusts Too Much](https://learn.secbyte.org/ctf/browser-cache-poisoning-when-the-browser-trusts-too-much)
- [Cache Poisoning: From Varying Responses to Exploitation and Defense](https://learn.secbyte.org/ctf/cache-poisoning-from-varying-responses-to-exploitation-and-d)

### 4. Input Validation & Authentication Misconfigurations
Bypass perimeter trust boundaries by exploiting unvalidated parameter open redirects and discovering exposed default administrative credentials.
- [Open Redirect: Trust Boundary Failures](https://learn.secbyte.org/ctf/open-redirect-trust-boundary-failures)
- [Default Admin Panel](https://learn.secbyte.org/ctf/default-admin-panel)

---

## Learning Path

Follow this structured progression path to master client-side DOM manipulation, HTTP protocol desynchronization, web/browser cache poisoning, and prototype pollution RCEs:

1. **Phase 1: Input Validation, Authentication & Client UI Exploitation** — Audit exposed default admin portals, analyze open redirect parameters, and build clickjacking overlays:
   - [Default Admin Panel](https://learn.secbyte.org/ctf/default-admin-panel)
   - [Open Redirect: Trust Boundary Failures](https://learn.secbyte.org/ctf/open-redirect-trust-boundary-failures)
   - [Clickjacking: UI Redress and Interface Manipulation](https://learn.secbyte.org/ctf/clickjacking-ui-redress-and-interface-manipulation)
   - [Tabnabbing: Trusted Tabs, Untrusted Targets](https://learn.secbyte.org/ctf/tabnabbing-trusted-tabs-untrusted-targets)
   - [Cross-Origin Misconfiguration](https://learn.secbyte.org/ctf/cross-origin-misconfiguration)

2. **Phase 2: Advanced Client-Side JavaScript (DOM Clobbering & Prototype Pollution)** — Clobber DOM attributes to bypass logic filters and pollate JavaScript prototypes for Node.js RCE:
   - [DOM Clobbering: Learning Room](https://learn.secbyte.org/ctf/dom-clobbering-learning-room)
   - [Prototype Pollution to RCE](https://learn.secbyte.org/ctf/prototype-pollution-to-rce)

3. **Phase 3: Web & Browser Cache Poisoning** — Identify unkeyed request inputs to contaminate intermediate web proxy caches and persistent browser storage:
   - [Browser Cache Poisoning: When the Browser Trusts Too Much](https://learn.secbyte.org/ctf/browser-cache-poisoning-when-the-browser-trusts-too-much)
   - [Cache Poisoning: From Varying Responses to Exploitation and Defense](https://learn.secbyte.org/ctf/cache-poisoning-from-varying-responses-to-exploitation-and-d)

4. **Phase 4: HTTP Protocol Desynchronization & Response Splitting** — Master host header injections, CRLF response splitting, and CL.TE/TE.CL request smuggling:
   - [Host Header Injection: From Discovery to Defense](https://learn.secbyte.org/ctf/host-header-injection-from-discovery-to-defense)
   - [HTTP Response Splitting: Header Injection & Cache Poisoning](https://learn.secbyte.org/ctf/http-response-splitting-header-injection-cache-poisoning)
   - [HTTP Request Smuggling: Front-End Confusion Lab](https://learn.secbyte.org/ctf/http-request-smuggling-front-end-confusion-lab)

---

## How to Use the Labs

1. Select a challenge link from the index or category sections above.
2. Read the scenario directives, architecture maps, and application specs on [Learn SecByte](https://learn.secbyte.org/).
3. Deploy analysis toolsets (Burp Suite Pro/Community with HTTP Request Smuggler / Param Miner, Node.js CLI, Python, Chrome DevTools) inside an isolated workstation.
4. Craft prototype pollution payloads, clobber DOM tree elements, desynchronize HTTP request headers, poison proxy caches, and capture target flags.

---

## Disclaimer

This repository and its linked challenge resources are strictly intended for educational, threat research, and authorized technical security training purposes. Never execute prototype pollution RCEs, HTTP request smuggling, cache poisoning, or credential harvesting attacks against unauthorized production servers, live CDNs, or third-party web application users.
