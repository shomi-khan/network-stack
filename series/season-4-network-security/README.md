# সিজন ৪ — Network Security ও Guest Wi-Fi

অধ্যায় ১৯–২৪। লক্ষ্য: দোকানের অবিশ্বস্ত ফোন নেটওয়ার্কে ঢুকলেও কর্মীর যন্ত্র, অ্যাপ্লিকেশন সার্ভার, ও ডেটাবেস তার নাগালের বাইরে থাকে।

## আগে কী লাগবে

ঠিকানা, সাবনেট, ও রাউটিং। সিজন ৩-এর চ্যানেল। পৌঁছানো যে অনুমতি নয়, সেই পার্থক্য।

ভৌত দোকান ব্যবসা হিসেবে আগে থেকে আছে। তার ওয়াই-ফাই ও জোন এই সিজনে নকশা হয়। আগের অধ্যায় সেই নকশা ধরে নেয় না। [টাইমলাইন](../../product/timeline.md)। ইনভেন্টরির গেস্ট ও অফিস প্রিফিক্স এই সিজনের জন্য রাখা। [network-inventory.md](../../product/network-inventory.md)।

## অধ্যায়

| # | অধ্যায় | অবস্থা |
| --- | --- | --- |
| ১৯ | [দোকানের Guest Wi-Fi: Trust Boundary](../../docs/curriculum.md#ch-19) | planned |
| ২০ | [Wi-Fi Security, Client Isolation ও Rogue Access Point](../../docs/curriculum.md#ch-20) | planned |
| ২১ | [VLAN, Subnet ও Network Segmentation](../../docs/curriculum.md#ch-21) | planned |
| ২২ | [Firewall, ACL, Ingress, Egress ও Stateful Filtering](../../docs/curriculum.md#ch-22) | planned |
| ২৩ | [IP Whitelisting, NAT ও IP-ভিত্তিক বিশ্বাসের সীমা](../../docs/curriculum.md#ch-23) | planned |
| ২৪ | [Network Access Control, Zero Trust ও Threat Modeling](../../docs/curriculum.md#ch-24) | planned |

## শেষে কী ব্যাখ্যা করতে পারবে

- গেস্ট ওয়াই-ফাই ইন্টারনেট দিতে পারে, অফিস বা ডেটাবেসের চাবি হয়ে নয়।
- আইসোলেশন ও VLAN কনফিগারেশন ছাড়া নিজে থেকে সীমানা নয়।
- ফায়ারওয়াল পথ সীমিত করে। অ্যাপ্লিকেশনের অনুমতি আলাদা থাকে।
- IP whitelist মানুষের পরিচয় নয়।

আগের সিজন [TLS](../season-3-tls-secure-communication/README.md)। পরের সিজন [স্কেলিং](../season-5-production-networking/README.md)।
