# সিজন ২ — DNS, Routing ও Addressing

অধ্যায় ৭–১২। লক্ষ্য: নাম কীভাবে ঠিকানা হয়, এবং প্যাকেট পরের হপ খুঁজে পায়।

## আগে কী লাগবে

[সিজন ১](../season-1-request-journey/README.md)। বিশেষ করে অধ্যায় ১-এর যাত্রা: ক্যাশ থাকতে পারে, গেটওয়ে পরের হপ, লিংক স্তর আলাদা।

এই সিজনের শুরুতেও KenaKata একটি সার্ভার। গেস্ট ওয়াই-ফাইয়ের নকশা এখনো নেই। [টাইমলাইন](../../product/timeline.md)।

## অধ্যায়

| # | অধ্যায় | অবস্থা |
| --- | --- | --- |
| ৭ | [DNS Resolution: নাম থেকে IP Address](../../docs/curriculum.md#ch-07) | planned |
| ৮ | [Recursive Resolver, Root, TLD ও Authoritative DNS](../../docs/curriculum.md#ch-08) | planned |
| ৯ | [DNS Record, Caching, TTL ও প্রচলিত ভুল](../../docs/curriculum.md#ch-09) | planned |
| ১০ | [Subnet, CIDR ও Subnet Mask](../../docs/curriculum.md#ch-10) | planned |
| ১১ | [Routing Table, Gateway, NAT ও Port Forwarding](../../docs/curriculum.md#ch-11) | planned |
| ১২ | [DHCP, IPv6-এর ভিত্তি ও নেটওয়ার্ক Troubleshooting](../../docs/curriculum.md#ch-12) | planned |

## শেষে কী ব্যাখ্যা করতে পারবে

- রিকার্সিভ রিজলভার, রুট, TLD, ও অথরিটেটিভ সার্ভার কে কী উত্তর দেয়।
- TTL ক্যাশের মেয়াদ। বিশ্বজোড়া এক ঘড়ির প্রপাগেশন নয়।
- প্রিফিক্স বদলালে লোকাল ও রিমোট সিদ্ধান্ত বদলায়।
- NAT ঠিকানা বদলায়। মানুষের পরিচয় দেয় না।

আগের সিজন [Request-এর যাত্রা](../season-1-request-journey/README.md)। পরের সিজন [TLS](../season-3-tls-secure-communication/README.md)।
