# VRChat Domain Blocklist
## What
A list of domains used by VRChat worlds (and VRChat itself, and its SDK, and...) for advertising or tracking purposes.
## Why
Ads are cringe.

Additionally, VRChat's security model for HTTP requests is fundamentally broken. You have the option to deny requests to all domains except those on a VRChat-supplied allowlist (which may change at any time, without any notice), or allowing everything. There is no notification or user feedback when an HTTP request is made. Many worlds require access to non-allowlisted domains for basic functionality, so many users (I would bet *most* users) leave untrusted URLs enabled, which leaves them open to worlds taking advantage of this to spy on them.

If the multiple open issues on Canny which have been ignored for months or years are anything to go by, VRChat does not intend to improve this situation.

Finally, simply leaving untrusted URLs disabled is not a perfect solution, since many worlds are loading ads from allowlisted services such as GitHub.
## How
Idk you can probably use this with Pi-hole or something. I'm using PowerDNS Recursor and some shell scripts myself.
## Notes
Some worlds are using the same domains for ads/tracking as they are for normal world functions, so blocking those domains would break base functionality. In this case, the entry is commented out. It's up to you to decide if you want to uncomment these entries.
## Transparency
This is my personal list and I make no guarantees of the accuracy or efficacy of it - I actually do not normally use any of the worlds or prefabs listed here. Also in the event that any of my own worlds at some point incorporate ads or user behavior tracking, I will add them to the list as well because that's only fair.

Pull requests to add or update entries will probably be accepted.
