# Containers

Boot all containers with
```sh
docker-compose -f elk.yaml up
```

copy invoices into logstash/data

connect to localhost:5601 to see Kibana and load/create dashboards

folders and files
```sh
.
├── elasticsearch
│   ├── config
│   │   └── elasticsearch.yml
│   └── Dockerfile
├── elk.yaml
├── kibana
│   ├── config
│   │   └── kibana.yml
│   └── Dockerfile
├── logstash
│   ├── config
│   │   ├── logstash.yml
│   │   └── pipelines.yml
│   ├── data                   <<< invoices here
│   │   ├── loaded.since
│   │   └── phone2name.csv     <<< replace with you phones and names
│   ├── Dockerfile
│   └── pipeline
│       └── telecom
│           └── telecom.conf
└── README.md
```
