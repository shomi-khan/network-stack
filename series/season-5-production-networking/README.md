# সিজন ৫ — Production Networking ও Scaling

অধ্যায় ২৫–৩০। লক্ষ্য: এক সার্ভারের দোকান যখন একাধিক সার্ভার, এজ, ও ক্লাউড জোন হয়, তখন কোন ব্যর্থতা সামলানো হয় এবং কোনটি থাকে।

## আগে কী লাগবে

সিজন ১-এর যাত্রা, সিজন ২-এর নাম ও রাউট, সিজন ৪-এর সীমানা। অধ্যায় ২৫-এর আগে ক্রেতা সরাসরি একটি সার্ভারে যায়। [টাইমলাইন](../../product/timeline.md)।

## অধ্যায়

| # | অধ্যায় | অবস্থা |
| --- | --- | --- |
| ২৫ | [Reverse Proxy ও Load Balancer](../../docs/curriculum.md#ch-25) | planned |
| ২৬ | [Layer 4 বনাম Layer 7 Load Balancing ও Health Check](../../docs/curriculum.md#ch-26) | planned |
| ২৭ | [একাধিক Application Server, Clustering ও High Availability](../../docs/curriculum.md#ch-27) | planned |
| ২৮ | [Service Discovery, Timeout, Retry ও Cascading Failure](../../docs/curriculum.md#ch-28) | planned |
| ২৯ | [CDN, Rate Limiting, DDoS Protection ও Traffic Management](../../docs/curriculum.md#ch-29) | planned |
| ৩০ | [Cloud VPC/VNet, Public ও Private Subnet, Private Service](../../docs/curriculum.md#ch-30) | planned |

## শেষে কী ব্যাখ্যা করতে পারবে

- প্রক্সি ও ব্যালেন্সার ক্লায়েন্টের দৃশ্য বদলায়। অ্যাপের বাগ মুছে দেয় না।
- পোর্ট খোলা আর অ্যাপ সুস্থ এক কথা নয়।
- একাধিক অ্যাপ সার্ভার একটি ডেটাবেসের ব্যর্থতা সামলায় না।
- প্রাইভেট সাবনেট সরাসরি পথ কমায়। ভিতরের পথ ও অনুমতি থেকে যায়।

আগের সিজন [নেটওয়ার্ক সিকিউরিটি](../season-4-network-security/README.md)। পরের সিজন [অপারেশন](../season-6-operations-architecture/README.md)।
