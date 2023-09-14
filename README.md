## Result:

| Framework  | Throughput (Request/Second)                                                                                |
|------------|------------------------------------------------------------------------------------------------------------|
| Blacksheep | [5,339](https://raw.githubusercontent.com/PantherPy/frameworks-benchmark/master/blacksheep/blacksheep.png) |
| Muffin     | [5,320](https://raw.githubusercontent.com/PantherPy/frameworks-benchmark/master/muffin/muffin.png)         |
| Panther    | [5,112](https://raw.githubusercontent.com/PantherPy/frameworks-benchmark/master/panther/panther.png)       |
| Sanic      | [3,660](https://raw.githubusercontent.com/PantherPy/frameworks-benchmark/master/sanic/sanic.png)           |
| FastAPI    | [3,260](https://raw.githubusercontent.com/PantherPy/frameworks-benchmark/master/fastapi/fastapi.png)       |
| Tornado    | [2,081](https://raw.githubusercontent.com/PantherPy/frameworks-benchmark/master/tornado/tornado.png)       |
| Bottle     | [2,045](https://raw.githubusercontent.com/PantherPy/frameworks-benchmark/master/bottle/bottle.png)         |
| Django     | [821](https://raw.githubusercontent.com/PantherPy/frameworks-benchmark/master/django/django.png)           |
| Flask      | [749](https://raw.githubusercontent.com/PantherPy/frameworks-benchmark/master/flask/flask.png)             |

## Scenario:

- Check Method
- Check Authorization Header
- Read Body
- Read Query Params
- Read Path Variables
- Read Request Payload
- Return All of Them as Json in Response

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

## FYI

We tried to get the best performance from frameworks, If you think you can make them better, your contributions are
welcome.
