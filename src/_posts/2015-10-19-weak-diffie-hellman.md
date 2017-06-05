---
layout: post
title: "Weak Diffie-Hellman"
date: 2015-10-19 22:58:00 -0500
categories: uncategorized
---
It came to light back in May that an exploit was possible whereby an attacker could force a server to downgrade its encryption to "export-grade". I remember something about it at the time, but I don't remember thinking it was a big deal.

Boy was I wrong.

The problem is that many servers use the same Diffie-Hellman groups for key exchange. An attacker with a large amount of computing power could pre-compute most of the bits needed to break the most common DH groups, and then use a man-in-the-middle to force a connection into a 512-bit export-grade mode... and then break it.

See [Weak Diffie-Hellman and the Logjam Attack][1] for details.

(And of course, removing export-grade DH from my servers has caused me to break many things...)

[1]: https://weakdh.org/