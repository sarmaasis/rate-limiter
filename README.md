# Rate Limiter 

A simple rate limiter using Redis


## USAGE

```python
    from rate_limiter import RateLimiter

    rate_limiter = RateLimiter(redis_host='localhost', redis_port=6379, redis_db=0, bucket_capacity=10 refill_rate=1)

    if rate_limiter.is_allowed("user123"):
        print("Request allowed")
    else:
        print("Rate limit exceeded")

```


