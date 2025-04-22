# OAuth Flow Hijack PoC

This is a Proof-of-Concept (PoC) demonstrating an OAuth flow hijack vulnerability by exploiting unvalidated redirection in the login flow.

## Hosted Demo

- **Start page**: [https://zonia-bad.github.io/oauth-hijack-poc/](https://zonia-bad.github.io/oauth-hijack-poc/)
- **redirect.html** (replace `REPLACE_ME` with your own webhook):  
  [View Raw File](https://raw.githubusercontent.com/yourgithubusername/oauth-hijack-poc/main/redirect.html)

## How to Use

1. Replace `REPLACE_ME` in `redirect.html` with your own Webhook URL (e.g., from https://webhook.site).
2. Replace the login url in the `index.html` with your own login endpoint
3. Host the `redirect.html` on your own test domain (or locally).
4. Open the hosted `index.html` and click **“Start Attack”**.
5. The popup will redirect to an attacker-controlled OAuth URL.
6. After login, the token will be sent to your specified webhook.

## Disclosure Note

This PoC is provided for security testing and demonstration purposes only.
