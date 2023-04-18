# knowledgebase

echo -n | openssl s_client -connect 20.104.109.112:443 -servername QA.MyGroceryOffers.Ca -verify 3 | sed -n '/---\nCertificate chain/,/---\nServer certificate/p'

echo -n | openssl s_client -connect 104.198.133.59:443 -servername www.MyGroceryOffers.Ca -verify 3 | sed -n '/---\nCertificate chain/,/---\nServer certificate/p'