# Producer Consumer

Attempt at implementing [Lab: Concurrency in C](https://www.classes.cs.uchicago.edu/archive/2018/spring/12300-1/lab6.html) which writes an instance of the [Producer–consumer problem](https://en.wikipedia.org/wiki/Producer%E2%80%93consumer_problem).

Status: WIP (Haven't started, just setup)

## Build and Run

```
clang -lpthread producer_consumer.c -o producer_consumer
for i in {1..1000}; do ./producer_consumer; done | sort | uniq -c
```

Should return:
```
1000 Net: 0
```
Rather than:
```
 496 Net: 0
   1 Net: 456
 503 Net: 500
```
for example
