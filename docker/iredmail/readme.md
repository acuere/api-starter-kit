## DNS Records for example.com

### Current Records
| Type | Name               | Value                              |
|------|--------------------|------------------------------------|
| A    | example.com        | `<IP>` (replace with your actual IP) |
| A    | mail               | `<IP>` (replace with your mail server's IP) |
| MX   | mail               | `<Priority>` mail.example.com (replace with the appropriate priority and mail server) |
| MX   | @                  | `<Priority>` autoconfig.example.com (replace with the appropriate priority and autoconfig server) |
| MX   | @                  | `<Priority>` autodiscover.example.com (replace with the appropriate priority and autodiscover server) |
| TXT  | dkim._domainkey    | v=DKIM1; p=<key> (replace with your actual DKIM key) |
| TXT  | _dmarc              | "v=DMARC1; p=none; sp=none; rua=mailto:spam-reports@example.com" |
| TXT  | mail               | v=spf1 ip4:<IP> include:example.com ~all (replace with your actual mail server IP) |

### Updated Records
| Type | Name               | Value                              |
|------|--------------------|------------------------------------|
| A    | example.com        | 192.168.1.1 (replace with your actual IP) |
| A    | mail               | 192.168.1.2 (replace with your mail server's IP) |
| MX   | mail               | 10 mail.example.com (replace with the appropriate priority and mail server) |
| MX   | @                  | 20 autoconfig.example.com (replace with the appropriate priority and autoconfig server) |
| MX   | @                  | 30 autodiscover.example.com (replace with the appropriate priority and autodiscover server) |
| TXT  | dkim._domainkey    | v=DKIM1; p=your_actual_dkim_key (replace with your actual DKIM key) |
| TXT  | _dmarc              | "v=DMARC1; p=none; sp=none; rua=mailto:spam-reports@example.com" |
| TXT  | mail               | v=spf1 ip4:192.168.1.2 include:example.com ~all (replace with your actual mail server IP) |
