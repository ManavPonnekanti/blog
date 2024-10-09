---
title: Cloudflare is bad
date: 2024-10-06
---
I’m going to keep this brief: never use Cloudflare for domain registration or hosting if you can help it. Here are three reasons:

1. If you register a domain with Cloudflare, you cannot use nameservers anywhere else. I cannot think of a single other modern registrar with such aggressive vendor-lock in. The most salient problem with this is that if you want to take advantage of a CDN, you are stuck with Cloudflare, which leads me to the second problem:
2. Cloudflare’s CDN has abysmal UX. Due to some sort of abstruse caching policy, it does not seem to update changes to CSS files on the edge. The deployment pipeline appears to be inhabited by sentient and capricious machine-elves who will only allow particular parts of your website to be exposed to the wider world. Perhaps their whims adhere to some sort of aesthetic logic beyond my comprehension, and this inability to execute a basic hosting feature is actually an act of protest against my design choices.
3. Finally, I have seen too many scary [stories](https://www.reddit.com/r/CloudFlare/comments/154xmd2/be_careful_about_cloudflare_for_important_tasks/) about Cloudflare’s automated systems locking people out of their accounts due to IP changes and other unpredictable actions. The common pattern is that after the lock-out, they are stuck in hellish catch-22s in which they have to be logged into the account that they are locked out of in order to access support. The general response amongst ardent Cloudflare defenders (get a life, by the way!) is that you ought to have multiple accounts for any load-bearing domains. I do not know whether I live in some kind of bizarro-world, but this is insane to me. I have jumped ship before I too end up becoming the protagonist of a Heller novel adaptation.

I’ve had better luck with [Namecheap](https://namecheap.com/), and a particularly skillful [webdev](https://joodaloop.com) has told me good things about [Porkbun](https://porkbun.com/). You deserve better than Cloudflare.
