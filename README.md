python-gcm-dummy
======================
Dummy server that simulates apple APNS feedback service, it is designed to easy make an integration test in order to verify if tokens are
properly managed 

At this point timestamp is not correctly sended

Responses
-------------
By default server will output ok responses but a results file can be defined.

Example file:
```
someapplepushtoken1
someapplepushtoken2
```

Server will automatically load any resuts.csv file in the working dir.

Usage
--------------
```
pip install gevent
python server.py
Starting server on 0.0.0.0:8081
```

Options
--------------
```
python server.py --help
Usage: server.py [options]

Options:
  -h, --help            show this help message and exit
  -p PORT, --port=PORT  Server port [8081]
  -b BIND, --bind_address=BIND
                        Bind addreess [0.0.0.0]
  -r RFILE, --results_file=RFILE
                        Results file [results.csv]
```

