icomet
======

A C1000K comet server built with libevent

## Usage

```shell
make
./icomet

curl -v "http://127.0.0.1:8100/sub?id=12"
# open another terminal
curl -v "http://127.0.0.1:8000/pub?id=12&content=hi"
```

## Memory Usage

| Connections | VIRT | RES |
| ----------- | ---- | --- |
| 0 | 39m | 24m |
| 100,000 | 302m | 288m |
| 200,000 | 579m |565m |
| 500,000 | 1441m | 1427m |
| 1,000,000 | 2734m | 2720m |

2.7KB per connection.
