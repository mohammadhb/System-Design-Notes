# Always set a rate limit for inner messaging
### If you want to know if your services are in trouble look at `3` things:
1. Average `Response Time`
2. Age of `Message` in the `Queue`
3. Dead letter `Queue`
    - Requests that has failed goes in this `Queue`
    - Send notification afterwards
    - Let other services `subscribe` to this `Queue`

### Deal with bad `Actors`:


### Optimization:

- Request Collapsing
- Exponentioal Backoff
    - 1,2,4,8,... `2^n`
    - After certain `threshold(t)` client will return an error
