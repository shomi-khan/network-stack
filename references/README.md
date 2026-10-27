# সূত্র

অধ্যায় লেখার সময় খুলতে হয় এমন নথি। স্পেসিফিকেশন এখানে কপি করা হয়নি। কোন বাক্যটি একটি অধ্যায়ের দাবির ভিত্তি, সেটা অধ্যায় স্থির করে, এই পাতা নয়।

নীতি [source-policy.md](../docs/source-policy.md)। একটি RFC পরে obsolete হলে অধ্যায় পুরোনো নথিটিকে বর্তমান বলে বসায় না। তালিকা ২০২৬-১০-২৭ তারিখে rfc-editor.org, ITU, NIST CSRC, MDN, curl, man7, OpenSSL, ও BIND-এর পাতা খুলে মিলিয়ে দেখা হয়েছে, যেখানে নিচে লিঙ্ক আছে।

IEEE 802.3, IEEE 802.11, ও IEEE 802.1Q-এর বর্তমান সংস্করণ এই সূচনায় মিলিয়ে লিঙ্ক দেওয়া হয়নি। ওই অধ্যায় লেখার সময় standards.ieee.org থেকে সংস্করণ দেখে নিতে হয়। ওয়াই-ফাই অ্যালায়েন্সের WPA নথিও একইভাবে অধ্যায়ের সময় মিলিয়ে নিতে হয়। এখানে সেগুলো নিশ্চিত উদ্ধৃতি নয়।

## নাম, ঠিকানা, পথ

| নথি | কী জন্য |
| --- | --- |
| [RFC 1034](https://www.rfc-editor.org/rfc/rfc1034) | DNS-এর ধারণা। TTL কতক্ষণ ক্যাশ করা যায় |
| [RFC 1035](https://www.rfc-editor.org/rfc/rfc1035) | DNS-এর বার্তা ও রেকর্ড |
| [RFC 2181](https://www.rfc-editor.org/rfc/rfc2181) | DNS-এর স্পষ্টীকরণ, TTL |
| [RFC 2308](https://www.rfc-editor.org/rfc/rfc2308) | নেতিবাচক উত্তর ক্যাশ |
| [RFC 2782](https://www.rfc-editor.org/rfc/rfc2782) | SRV রেকর্ড। সার্ভিস ডিসকভারির একটি মান |
| [RFC 2606](https://www.rfc-editor.org/rfc/rfc2606) | `.example` ও `example.com` ডকুমেন্টেশনের জন্য |
| [RFC 3986](https://www.rfc-editor.org/rfc/rfc3986) | URI |
| [RFC 791](https://www.rfc-editor.org/rfc/rfc791) | IPv4-এর ভিত্তি। পরে অনেক RFC একে আপডেট করেছে |
| [RFC 8200](https://www.rfc-editor.org/rfc/rfc8200) | IPv6 |
| [RFC 4291](https://www.rfc-editor.org/rfc/rfc4291) | IPv6 ঠিকানার গঠন |
| [RFC 1918](https://www.rfc-editor.org/rfc/rfc1918) | প্রাইভেট IPv4 |
| [RFC 4193](https://www.rfc-editor.org/rfc/rfc4193) | সাইটের ভিতরে ব্যবহারের ইউনিক লোকাল IPv6 ঠিকানা |
| [RFC 5737](https://www.rfc-editor.org/rfc/rfc5737) | ডকুমেন্টেশনের IPv4 ব্লক |
| [RFC 3849](https://www.rfc-editor.org/rfc/rfc3849) | ডকুমেন্টেশনের IPv6 প্রিফিক্স |
| [RFC 1122](https://www.rfc-editor.org/rfc/rfc1122) | হোস্টের লিংক, ইন্টারনেট, ও ট্রান্সপোর্ট স্তর |
| [RFC 1123](https://www.rfc-editor.org/rfc/rfc1123) | হোস্টের অ্যাপ্লিকেশন ও সাপোর্ট |
| [RFC 826](https://www.rfc-editor.org/rfc/rfc826) | ARP |
| [RFC 4861](https://www.rfc-editor.org/rfc/rfc4861) | IPv6 Neighbor Discovery |
| [RFC 950](https://www.rfc-editor.org/rfc/rfc950) | পুরোনো সাবনেটিং পদ্ধতি। একা আজকের CIDR নয় |
| [RFC 4632](https://www.rfc-editor.org/rfc/rfc4632) | CIDR |
| [RFC 2131](https://www.rfc-editor.org/rfc/rfc2131) | DHCP |
| [RFC 8415](https://www.rfc-editor.org/rfc/rfc8415) | DHCPv6 |

## ট্রান্সপোর্ট ও HTTP

| নথি | কী জন্য |
| --- | --- |
| [RFC 768](https://www.rfc-editor.org/rfc/rfc768) | UDP |
| [RFC 9293](https://www.rfc-editor.org/rfc/rfc9293) | বর্তমান TCP। RFC 793-কে obsolete করে |
| [RFC 9110](https://www.rfc-editor.org/rfc/rfc9110) | HTTP semantics। `https` স্কিম। পুরোনো RFC 2818-কে obsolete করে |
| [RFC 9112](https://www.rfc-editor.org/rfc/rfc9112) | HTTP/1.1। কানেকশন আবার ব্যবহার |
| [RFC 9113](https://www.rfc-editor.org/rfc/rfc9113) | HTTP/2 |
| [RFC 9114](https://www.rfc-editor.org/rfc/rfc9114) | HTTP/3 |
| [RFC 9000](https://www.rfc-editor.org/rfc/rfc9000) | QUIC |
| [MDN: HTTP](https://developer.mozilla.org/en-US/docs/Web/HTTP) | ব্রাউজারের HTTP। স্পেসিফিকেশনের বদলি নয় |

## TLS ও পরিচয়

| নথি | কী জন্য |
| --- | --- |
| [RFC 8446](https://www.rfc-editor.org/rfc/rfc8446) | TLS 1.3 |
| [RFC 5246](https://www.rfc-editor.org/rfc/rfc5246) | TLS 1.2। RFC 8446 এটিকে obsolete করে, তবু ডিপ্লয়মেন্টে দেখা যায় |
| [RFC 9325](https://www.rfc-editor.org/rfc/rfc9325) | TLS ব্যবহারে সুপারিশ। SSL ও TLS 1.0/1.1 নিয়ে নিষেধ |
| [RFC 8996](https://www.rfc-editor.org/rfc/rfc8996) | TLS 1.0 ও 1.1 অবসান |
| [RFC 7568](https://www.rfc-editor.org/rfc/rfc7568) | SSL 3.0 ব্যবহার না করা |
| [RFC 6101](https://www.rfc-editor.org/rfc/rfc6101) | SSL 3.0-এর ঐতিহাসিক বর্ণনা |
| [RFC 9001](https://www.rfc-editor.org/rfc/rfc9001) | QUIC-এ TLS |
| [RFC 5280](https://www.rfc-editor.org/rfc/rfc5280) | X.509 সার্টিফিকেট ও CRL প্রোফাইল |
| [RFC 9525](https://www.rfc-editor.org/rfc/rfc9525) | TLS-এ সার্ভিসের পরিচয় যাচাই |
| [RFC 4033](https://www.rfc-editor.org/rfc/rfc4033), [4034](https://www.rfc-editor.org/rfc/rfc4034), [4035](https://www.rfc-editor.org/rfc/rfc4035) | DNSSEC |
| [FIPS 180-4](https://csrc.nist.gov/pubs/fips/180-4/upd1/final) | Secure Hash Standard |
| [FIPS 186-5](https://csrc.nist.gov/pubs/fips/186-5/final) | Digital Signature Standard |
| [MDN: TLS](https://developer.mozilla.org/en-US/docs/Web/Security/Defenses/Transport_Layer_Security) | ব্রাউজারের TLS আলোচনা |

## NAT, ফিল্টার, অ্যাডমিন পথ

| নথি | কী জন্য |
| --- | --- |
| [RFC 3022](https://www.rfc-editor.org/rfc/rfc3022) | ঐতিহ্যগত NAT। Informational |
| [RFC 4787](https://www.rfc-editor.org/rfc/rfc4787) | UDP-র জন্য NAT-এর আচরণ। সব NAT-এর সম্পূর্ণ বিবরণ নয় |
| [RFC 4301](https://www.rfc-editor.org/rfc/rfc4301) | IP-স্তরের নিরাপত্তা স্থাপত্য, IPsec |
| [RFC 4253](https://www.rfc-editor.org/rfc/rfc4253) | SSH ট্রান্সপোর্ট |
| [ITU-T X.200](https://www.itu.int/rec/T-REC-X.200-199407-I/en) | OSI বেসিক রেফারেন্স মডেল |
| [NIST SP 800-41 Rev. 1](https://csrc.nist.gov/pubs/sp/800/41/r1/final) | ফায়ারওয়াল নীতির গাইড। প্রোটোকল স্পেসিফিকেশন নয়। নতুন NIST নথি আছে কি না, অধ্যায় ২২ লেখার সময় দেখতে হয় |
| [NIST SP 800-207](https://csrc.nist.gov/pubs/sp/800/207/final) | Zero Trust Architecture |
| [NIST SP 800-61 Rev. 3](https://csrc.nist.gov/pubs/sp/800/61/r3/final) | ইনসিডেন্ট রেসপন্স নিয়ে CSF 2.0 কমিউনিটি প্রোফাইল। পুরোনো Rev. 2 হ্যান্ডবুকের নতুন নাম এটি নয় |

ক্লাউড VPC বা VNet লেখার সময় সেই প্রদানকারীর বর্তমান ডকুমেন্টেশন ধরতে হয়। এখানে একটি বিক্রেতাকে মান বানিয়ে রাখা হয়নি। লোড ব্যালেন্সারের একটি সাধারণ RFC নেই। HTTP-তে মধ্যবর্তী উপাদানের ভাষা RFC 9110। একটি সফটওয়্যারের কনফিগারেশন সেই তত্ত্বের জায়গা নেয় না।

## অনুশীলনের সরঞ্জাম

| নথি | কী জন্য |
| --- | --- |
| [curl man page](https://curl.se/docs/manpage.html) | `curl` |
| [ip(8)](https://man7.org/linux/man-pages/man8/ip.8.html) | Linux `ip` |
| [ss(8)](https://man7.org/linux/man-pages/man8/ss.8.html) | সকেট দেখা |
| [OpenSSL s_client](https://docs.openssl.org/master/man1/openssl-s_client/) | TLS ক্লায়েন্ট |
| [BIND manual pages](https://bind9.readthedocs.io/en/stable/manpages.html) | `dig` |

`ping`, `traceroute`, ও `tcpdump`-এর পৃষ্ঠা প্ল্যাটফর্মভেদে আলাদা। অধ্যায় যে কমান্ড দেয়, সেই প্ল্যাটফর্মের বর্তমান ম্যানুয়াল দেখে ফ্ল্যাগ লিখতে হয়।
