# Headers and transport

Serve the entire site over HTTPS and add a few security headers so that traffic is encrypted and browsers enforce safer behavior. HTTPS is the non-negotiable baseline; security headers are a low-effort layer on top.

## HTTPS everywhere

Serve every page over HTTPS, not just the login or checkout. HTTPS encrypts traffic between the visitor and your site, which protects credentials, cookies, and content from being read or tampered with in transit. Modern hosts and free certificate options make this straightforward, and browsers increasingly warn on or block sites without it. There is no good reason to run a site on plain HTTP today.

## Redirect and enforce

Once HTTPS is in place, redirect all plain HTTP requests to it so no one lands on an unencrypted version. A strict-transport policy header tells browsers to use HTTPS for your site automatically in future, closing the brief window where a first request might go over HTTP. Together these make HTTPS the only way the site is served, rather than merely an option.

## A few worthwhile headers

Beyond transport, a small set of response headers ask the browser to behave more safely: controlling how your pages can be framed by other sites to limit clickjacking, telling the browser not to second-guess content types, and controlling what information is sent in referrers. These are low-cost additions that harden how browsers treat your site, and most can be set once at the server or through a plugin.

## Content security, carefully

A content security policy can restrict what scripts and resources a page is allowed to load, which limits the impact of certain injection attacks. It is powerful but needs care, because a policy that is too strict can break legitimate functionality. If you take it on, build it up gradually and test, rather than applying a blanket rule that disables parts of your own site.

## Set once, benefits ongoing

Transport and header settings are largely a one-time configuration that then protects every request. Get HTTPS enforced and add the straightforward headers, and you have closed a category of risk with little ongoing effort. Save the more involved options like a tight content security policy for when the basics are solidly in place.
