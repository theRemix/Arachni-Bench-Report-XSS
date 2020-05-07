# Arachni Bench Report XSS

Arachni report of owasp benchmark xss

## Live report

[https://theremix.github.io/Arachni-Bench-Report-XSS/](https://theremix.github.io/Arachni-Bench-Report-XSS/)

## OWASP Benchmark

https://owasp.org/www-project-benchmark/

## Arachni

https://www.arachni-scanner.com/

```
docker run -d \
  -p 7331:7331 \
  -p 9292:9292 \
  --name arachni \
  --link bench \
  arachni/arachni:latest
```

inside container
```
/usr/local/arachni/bin/arachni https://bench:8443/benchmark/xss-Index.html
/usr/local/arachni/bin/arachni_reporter --reporter html *.afr
```
