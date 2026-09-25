LottoPulse website — v1.4 flow
==============================

CONTENTS
- /index.html            Public landing page
- /success/index.html    Post-payment activation page
- /privacy/index.html    Updated privacy policy
- /assets/               Site assets

NEW FLOW
1) Visitor opens the landing page.
2) "Install LottoPulse" opens the Chrome Web Store.
3) The installed extension asks for a local username.
4) The extension opens the Stripe checkout for the €1.99 one-time unlock.
5) Stripe redirects to /success/ with the private activation key supplied in the redirect URL.
6) /success/ passes that key to the installed extension.
7) The extension validates it and stores the local license.

IMPORTANT
- Do not place the private activation key in this public GitHub repository.
- The /success/ page contains no secret; it only reads the key supplied by the Stripe redirect.
- The extension contains only the SHA-256 hash of the activation key.
- The success page targets the published Chrome extension ID:
  iohmpiampekjmbgnghdcdmflpkhjbial

DEPLOY
Upload these files to the root of the existing GitHub Pages repository.
