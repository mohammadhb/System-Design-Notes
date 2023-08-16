# Gateway
### Responsiblities:
- Routing External Requests ( Mapping Request to Services )
  
Routing table: (Can be later decoupled to `Service Registry`)

| API Endpoints | Handler        |
| :---:         | :---:          |
| register      | AuthService    |
| updateProfile | ProfileService |

- Blacklist IPs (With rate limiting)

Rate limiting table:

| Sender IP | Request Count |
| :---:     | :---:         |
| 10.10.1.2 | 12            |
| 10.10.2.3 | 324           |
