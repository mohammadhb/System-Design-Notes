# Gateway
### Responsiblities:
- Routing External Requests ( Mapping Request to Services )
  
Routing table:

| API Endpoints | Handler     |
| :---:         | :---:       |
| register      | AuthService |
| get-mails     | MailService |

- Blacklist IPs (With rate limiting)

Rate limiting table:

| Sender IP | Request Count |
| :---:     | :---:         |
| 10.10.1.2 | 12            |
| 10.10.2.3 | 324           |
