## Change Log

### [Unreleased][unreleased]

### [0.7.1] - 2022-12-12
#### Added
- Support for PHP 8.2

### [0.7.0] - 2022-06-30
#### Added
- Support for predis/predis ^2.0
- Support for zpopmin, zpopmax with predis driver 2.0

### [0.6.0] - 2022-05-24
#### Added
- Sentinels
- Sentinel add write to replicas config
- RedisProxyFactory

### [0.5.0] - 2022-05-05
#### Changed
- Added typehints
- Dropped support for php < 7.4

#### Added
- Added commands zrangebyscore, zpopmin, zpopmax

### [0.4.2] - 2020-06-25
#### Fixed
- Fixed zrem for multiple members

### [0.4.1] - 2019-05-02
#### Fixed
- Fixed typehint for hdel $key

### [0.4.0] - 2018-08-21
#### Changed
- Dropped support for PHP 5.6 and 7.0 [BC break]

#### Added
- Added commands: lset, lrem, zscan, zrem, zrank, zrevrank

### [0.3.1] - 2017-06-01
#### Fixed
- Replaced Redis constants to integers

### [0.3.0] - 2017-06-01
#### Added
- Added commands:
-- exists, type, dump, restore, setex, psetex, expire, pexpire, expireat, pexpireat, ttl, pttl, persist
-- getset, setnx, incr, incrby, incrbyfloat, decr, decrby, decrbyfloat
-- llen, lrange, lpush, rpush, lpop, rpop, lindex
-- zadd, zcard, zrange, zrevrange

#### Fixed
- Fixed connect to not-default host / port with Predis\Client

### [0.2.1] - 2017-01-19
#### Fixed
- Fixed commands select, mget and hmget
 
### [0.2.0] - 2017-01-16
#### Changed
- Return values of some commands (e.g. return null instead of false on get and hget)
- Unified info command for both drivers (inspired by Predis)

#### Added
- Wrapper for \Predis\Client
- Timeout to redis connect
- Possibility to set drivers order
- RedisProxyException - common exception for all drivers

### [0.1.0] - 2016-04-17

#### Added
- Wrapper for \Redis

[unreleased]: https://github.com/lulco/redis-proxy/compare/0.7.1...HEAD
[0.7.1]: https://github.com/lulco/redis-proxy/compare/0.7.0...0.7.1
[0.7.0]: https://github.com/lulco/redis-proxy/compare/0.6.0...0.7.0
[0.6.0]: https://github.com/lulco/redis-proxy/compare/0.5.0...0.6.0
[0.5.0]: https://github.com/lulco/redis-proxy/compare/0.4.2...0.5.0
[0.4.2]: https://github.com/lulco/redis-proxy/compare/0.4.1...0.4.2
[0.4.1]: https://github.com/lulco/redis-proxy/compare/0.4.0...0.4.1
[0.4.0]: https://github.com/lulco/redis-proxy/compare/0.3.1...0.4.0
[0.3.1]: https://github.com/lulco/redis-proxy/compare/0.3.0...0.3.1
[0.3.0]: https://github.com/lulco/redis-proxy/compare/0.2.1...0.3.0
[0.2.1]: https://github.com/lulco/redis-proxy/compare/0.2.0...0.2.1
[0.2.0]: https://github.com/lulco/redis-proxy/compare/0.1.0...0.2.0
[0.1.0]: https://github.com/lulco/redis-proxy/compare/0.0.0...0.1.0
