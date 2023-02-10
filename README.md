# CloudflareDDNS

API token
https://dash.cloudflare.com/profile/api-tokens

wget https://raw.githubusercontent.com/Westwall98/CloudflareDDNS/main/cloudflareddns.sh -O /sbin/cloudflareddns.sh

chmod +x /sbin/cloudflareddns.sh

cat >> /etc.defaults/ddns_provider.conf << EOF
[Cloudflare]
        modulepath=/sbin/cloudflareddns.sh
        queryurl=https://www.cloudflare.com
        website=https://www.cloudflare.com
EOF


API区域ID&Zoom ID
API Token
