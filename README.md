## Result:

| Framework  | Throughput |
|------------|------------|
| Blacksheep | 5,339      |
| Muffin     | 5,320      |
| Panther    | 5,112      |
| Sanic      | 3,660      |
| FastAPI    | 3,260      |
| Tornado    | 2,081      |
| Bottle     | 2,045      |
| Django     | 821        |
| Flask      | 749        |


## Environment:

#### OS: `Ubuntu 20.04.6 LTS x86_64`

#### Kernel: `5.15.0-1036-aws`

#### CPU: `Intel(R) Xeon(R) E5-2676 v3 @ 2.399,827 GHz`

#### Memory: `966 MiB`

#### Python: `3.11.5`

## Tools

We used `nakabonne/ali` for benchmarking

#### Installation: [https://github.com/nakabonne/ali#installation](https://github.com/nakabonne/ali#installation)

#### Command:

```bash
ali --rate 5500  "http://127.0.0.1:8000/users/2/records/10?name=ali&age=26" --method=PUT -H "Authorization: Token" -H "content-type: application/json" -b "{\"text\": \"hello\"}"
```

## Keep That In Mind

We tried to get the best performance from frameworks, If you think you can make them better, your contributions are
welcome.
