# App Factory

A landing page and checkout flow for custom iOS app builds. Visitors choose
what they want built and pay through a Stripe checkout session created by a
serverless function, then land on a confirmation page.

**Live:** https://app-factory-olive.vercel.app

**Stack:** HTML, CSS, JavaScript · Stripe Checkout · Vercel serverless
functions

The payment flow runs server-side, so no Stripe key is ever exposed to the
browser. Same pattern I use elsewhere: keep the credential on the server and
give the client a session, never a secret.
