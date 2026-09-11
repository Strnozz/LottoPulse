LottoPulse site package

Includes:
- /index.html            Landing page
- /success/index.html    Post-payment page
- /privacy/index.html    Privacy policy
- /assets/               Site assets

Chrome Web Store:
https://chromewebstore.google.com/detail/lottopulse/iohmpiampekjmbgnghdcdmflpkhjbial

Recommended GitHub Pages URL after uploading to the existing LottoPulse repository:
https://strnozz.github.io/LottoPulse/

Stripe success redirect:
https://strnozz.github.io/LottoPulse/success/

NEXT STEPS
1. Upload the CONTENTS of this folder to the root of your GitHub repository.
2. Ensure GitHub Pages deploys from the branch/folder you use for the site.
3. In Stripe Payment Link > After payment, choose redirect and enter:
   https://strnozz.github.io/LottoPulse/success/
4. When you have the LIVE Stripe Payment Link, replace the href="#purchase"
   on the pricing purchase button in index.html with that Stripe URL.
5. Test the complete flow in an incognito/private window.
