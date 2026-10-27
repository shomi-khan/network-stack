# Network Stack

**বাংলায় কম্পিউটার নেটওয়ার্ক, নেটওয়ার্ক সিকিউরিটি, ও প্রোডাকশন নেটওয়ার্ক আর্কিটেকচার শেখার গল্পভিত্তিক সিরিজ।**

রাফির পোশাকের দোকানের একটি পাতা ক্রেতার ফোন পর্যন্ত কীভাবে পৌঁছায়, পথে কী ভাঙতে পারে, এবং দোকান বড় হলে সেই পথকে কীভাবে আলাদা ও টিকিয়ে রাখা যায়? আরিফের সঙ্গে **KenaKata** চালাতে চালাতে সেই প্রশ্নগুলো পড়া হয়।

একই কাল্পনিক দোকান নিয়ে Trust Stack অথেন্টিকেশন ও অথরাইজেশন শেখায়। এই রিপোজিটরি সেই মহাবিশ্বের নেটওয়ার্ক সঙ্গী। অ্যাপ্লিকেশন নিরাপত্তার সিরিজ এখানে আবার লেখা হয়নি।

> **শেখার লক্ষ্য:** প্রোটোকলের সংজ্ঞা মুখস্থ করা নয়। একটি রিকোয়েস্টের পথ, সীমানা, ও ব্যর্থতা নিয়ে নিজে যুক্তি করতে শেখা।

এই রিপোজিটরি ধারণা ও ইঞ্জিনিয়ারিং যুক্তি শেখায়। প্রোডাকশন ফায়ারওয়াল রুল, ক্লাউড কনসোলের ধাপ, বা কপি করে চালানোর কনফিগারেশন এখানকার উদ্দেশ্য নয়।

## কার জন্য

বাংলাভাষী জুনিয়র ব্যাকএন্ড ইঞ্জিনিয়ার, যারা প্রোগ্রামিং জানেন এবং HTTP ও REST-এর সঙ্গে পরিচিত। নেটওয়ার্কিং আলাদা করে পড়েননি। রাউটার, সার্টিফিকেট, বা ভিলানের নাম শুনেছেন, কিন্তু একটি রিকোয়েস্ট সেগুলোর মধ্যে দিয়ে কীভাবে যায় সেটা সাজাননি।

এটি প্রোগ্রামিংয়ের প্রথম কোর্স নয়। কোনো একটি ক্লাউড বা ফায়ারওয়াল বিক্রেতার ম্যানুয়ালও নয়।

## কী শিখবে

- ব্রাউজার থেকে অ্যাপ্লিকেশন সার্ভার পর্যন্ত একটি রিকোয়েস্টের ধাপ, এবং কোন ধাপের সাফল্য কী প্রমাণ করে না।
- নাম, ঠিকানা, সাবনেট, রাউট, NAT, ও DHCP।
- TLS, সার্টিফিকেট, ও এনক্রিপশন যেখানে পরিচয় যাচাই থেকে আলাদা।
- দোকানের গেস্ট ওয়াই-ফাই কেন কর্মীর যন্ত্র ও ডেটাবেস থেকে আলাদা থাকতে হয়।
- লোড ব্যালেন্সার, একাধিক সার্ভার, ও ক্লাউড জোন কোন ব্যর্থতা সামলায়।
- লগ ও উপসর্গ দেখে কোন স্তরে খুঁজতে হয়।

## KenaKata

শুরুতে একটি অ্যাপ্লিকেশন সার্ভার, জনমুখী নাম, ও HTTPS। ক্রেতা পণ্যের পাতা খোলে। পরে নাম ও TLS-এর ভিতরের নিয়ম, ভৌত দোকানের গেস্ট ওয়াই-ফাই, আলাদা জোন, একাধিক সার্ভার, সীমিত ডেটাবেস, এবং অ্যাডমিন পথ আসে।

পরে আসা যন্ত্র আগের অধ্যায়ে চালু ধরা হয় না। কখন কী আছে, [টাইমলাইন](product/timeline.md)। শেষ লক্ষ্যের ছবি [আর্কিটেকচার](product/architecture.md)। সেটি শুরুর সিস্টেম নয়।

আরিফ সিস্টেম বানান ও চালান। নীরা ব্যবসার দাবি আনেন এবং সহজ উত্তর ভাঙেন। রাফি দোকানের সমস্যা বলেন। তিনজনের পরিচয় [characters.md](product/characters.md)।

## কীভাবে পড়ানো হয়

প্রতিটি অধ্যায় দোকানের একটি সমস্যা দিয়ে শুরু হয়। প্রথম সমাধান কোথায় থেমে যায়, ভিতরে কী হয়, কী ঝুঁকি, এবং উন্নত নকশা কী বিনিময় রাখে।

```text
সমস্যা
    ↓
প্রথম সমাধান
    ↓
ব্যর্থতা বা সীমা
    ↓
ভেতরের প্রক্রিয়া
    ↓
ঝুঁকি
    ↓
উন্নত নকশা
    ↓
বিনিময় ও যা থেকে যায়
```

কোনো প্রযুক্তি নিজে থেকে নিরাপদ বা সব জায়গায় মানানসই নয়। নেটওয়ার্কে পৌঁছানো অ্যাপ্লিকেশনের অনুমতি নয়। এনক্রিপশন পরিচয় যাচাই নয়। একটি ফায়ারওয়াল বাকি ঝুঁকি শেষ করে না।

## ছয় সিজন

| সিজন | অধ্যায় | লক্ষ্য |
| --- | --- | --- |
| [১. একটি Request-এর যাত্রা](series/season-1-request-journey/README.md) | ১–৬ | ক্লায়েন্ট থেকে সার্ভার পর্যন্ত মানসিক মডেল |
| [২. DNS, Routing ও Addressing](series/season-2-dns-routing/README.md) | ৭–১২ | নাম, ব্লক, গেটওয়ে, NAT |
| [৩. TLS ও নিরাপদ যোগাযোগ](series/season-3-tls-secure-communication/README.md) | ১৩–১৮ | চ্যানেল, সার্টিফিকেট, টানেল |
| [৪. Network Security ও Guest Wi-Fi](series/season-4-network-security/README.md) | ১৯–২৪ | অবিশ্বস্ত যন্ত্র ও সীমানা |
| [৫. Production Networking ও Scaling](series/season-5-production-networking/README.md) | ২৫–৩০ | প্রক্সি, একাধিক সার্ভার, ক্লাউড |
| [৬. Operations ও Network Architecture](series/season-6-operations-architecture/README.md) | ৩১–৩৬ | দেখা, খোঁজা, পুরো নকশা |

### সিজন ১

| # | অধ্যায় | অবস্থা |
| --- | --- | --- |
| ১ | [ব্রাউজার থেকে সার্ভার: একটি Request-এর যাত্রা](series/season-1-request-journey/01-request-journey/README.md) | draft |
| ২ | [OSI Model ও TCP/IP Model: Layer দিয়ে ভাবা](docs/curriculum.md#ch-02) | planned |
| ৩ | [Ethernet, MAC Address, ARP ও Network Interface](docs/curriculum.md#ch-03) | planned |
| ৪ | [IP Address: Private Network, Public IP ও IPv6](docs/curriculum.md#ch-04) | planned |
| ৫ | [TCP, UDP, Port, Socket ও Connection](docs/curriculum.md#ch-05) | planned |
| ৬ | [HTTP Request, Response ও Encapsulation](docs/curriculum.md#ch-06) | planned |

### সিজন ২

| # | অধ্যায় | অবস্থা |
| --- | --- | --- |
| ৭ | [DNS Resolution: নাম থেকে IP Address](docs/curriculum.md#ch-07) | planned |
| ৮ | [Recursive Resolver, Root, TLD ও Authoritative DNS](docs/curriculum.md#ch-08) | planned |
| ৯ | [DNS Record, Caching, TTL ও প্রচলিত ভুল](docs/curriculum.md#ch-09) | planned |
| ১০ | [Subnet, CIDR ও Subnet Mask](docs/curriculum.md#ch-10) | planned |
| ১১ | [Routing Table, Gateway, NAT ও Port Forwarding](docs/curriculum.md#ch-11) | planned |
| ১২ | [DHCP, IPv6-এর ভিত্তি ও নেটওয়ার্ক Troubleshooting](docs/curriculum.md#ch-12) | planned |

### সিজন ৩

| # | অধ্যায় | অবস্থা |
| --- | --- | --- |
| ১৩ | [HTTP বনাম HTTPS: কী বদলায়?](docs/curriculum.md#ch-13) | planned |
| ১৪ | [Cryptography-এর ভিত্তি: Key, Hash ও Digital Signature](docs/curriculum.md#ch-14) | planned |
| ১৫ | [TLS Handshake: নিরাপদ Connection](docs/curriculum.md#ch-15) | planned |
| ১৬ | [Certificate, Certificate Authority ও Trust Chain](docs/curriculum.md#ch-16) | planned |
| ১৭ | [Certificate Validation, Expiry ও TLS-এর ব্যর্থতা](docs/curriculum.md#ch-17) | planned |
| ১৮ | [VPN, Encrypted Tunnel ও Mutual TLS](docs/curriculum.md#ch-18) | planned |

### সিজন ৪

| # | অধ্যায় | অবস্থা |
| --- | --- | --- |
| ১৯ | [দোকানের Guest Wi-Fi: Trust Boundary](docs/curriculum.md#ch-19) | planned |
| ২০ | [Wi-Fi Security, Client Isolation ও Rogue Access Point](docs/curriculum.md#ch-20) | planned |
| ২১ | [VLAN, Subnet ও Network Segmentation](docs/curriculum.md#ch-21) | planned |
| ২২ | [Firewall, ACL, Ingress, Egress ও Stateful Filtering](docs/curriculum.md#ch-22) | planned |
| ২৩ | [IP Whitelisting, NAT ও IP-ভিত্তিক বিশ্বাসের সীমা](docs/curriculum.md#ch-23) | planned |
| ২৪ | [Network Access Control, Zero Trust ও Threat Modeling](docs/curriculum.md#ch-24) | planned |

### সিজন ৫

| # | অধ্যায় | অবস্থা |
| --- | --- | --- |
| ২৫ | [Reverse Proxy ও Load Balancer](docs/curriculum.md#ch-25) | planned |
| ২৬ | [Layer 4 বনাম Layer 7 Load Balancing ও Health Check](docs/curriculum.md#ch-26) | planned |
| ২৭ | [একাধিক Application Server, Clustering ও High Availability](docs/curriculum.md#ch-27) | planned |
| ২৮ | [Service Discovery, Timeout, Retry ও Cascading Failure](docs/curriculum.md#ch-28) | planned |
| ২৯ | [CDN, Rate Limiting, DDoS Protection ও Traffic Management](docs/curriculum.md#ch-29) | planned |
| ৩০ | [Cloud VPC/VNet, Public ও Private Subnet, Private Service](docs/curriculum.md#ch-30) | planned |

### সিজন ৬

| # | অধ্যায় | অবস্থা |
| --- | --- | --- |
| ৩১ | [Observability: Network Log, Metric ও Packet Capture](docs/curriculum.md#ch-31) | planned |
| ৩২ | [Troubleshooting: DNS, Routing, TCP ও TLS](docs/curriculum.md#ch-32) | planned |
| ৩৩ | [নিরাপদ Administrative Access: VPN ও Bastion Host](docs/curriculum.md#ch-33) | planned |
| ৩৪ | [Incident Response, Failure Isolation ও Disaster Recovery](docs/curriculum.md#ch-34) | planned |
| ৩৫ | [KenaKata-র Production Network Architecture](docs/curriculum.md#ch-35) | planned |
| ৩৬ | [Capstone: Request আগাগোড়া Trace, Secure ও Troubleshoot](docs/curriculum.md#ch-36) | planned |

## অবস্থা

`draft` মানে অধ্যায়ের খসড়া লেখা আছে। প্রকাশিত বলে ঘোষণা করা হয়নি। `planned` মানে কারিকুলামে জায়গা আছে, খসড়া এখনো নেই।

এই মুহূর্তে শুধু অধ্যায় ১ `draft`। বাকি ৩৫টি `planned`।

## আরও

| জায়গা | কী আছে |
| --- | --- |
| [product/](product/README.md) | দোকান, চরিত্র, টাইমলাইন, আর্কিটেকচার, ইনভেন্টরি, থ্রেট মডেল |
| [docs/](docs/README.md) | কারিকুলাম, অধ্যায়ের টেমপ্লেট, লেখা, ডায়াগ্রাম, ল্যাব, সূত্রের নিয়ম |
| [references/](references/README.md) | RFC ও অন্যান্য সূত্র |
| [notes/glossary.md](notes/glossary.md) | ছোট শব্দকোষ |
| [notes/misconceptions.md](notes/misconceptions.md) | যে ধারণাগুলো অধ্যায় ভাঙে |
| [CONTRIBUTING.md](CONTRIBUTING.md) | অধ্যায় যোগ করার নিয়ম |
| [LICENSE](LICENSE) | MIT |

শুরু করতে [অধ্যায় ১](series/season-1-request-journey/01-request-journey/README.md)।
