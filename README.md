# ha-elk-helm
Kinda production ready ELK(Elasticsearch, Kibana) helm package with nginx ingress output parsing support. All changes must be made in yaml files first, if values config not explicitly indicated in. Use this only for configuration assistance, if you are responsible.

Do not forget set some PVC settings, ingress settings(by default it uses cert-manager), change password(default is ChangeMeNow123), change replica values. 

Kibana creds u/p: elastic ChangeMeNow123

Default setup: 4 elk master, 2 data, 2 ingest, filebeat -> logstash -> ELK. By defult logtrail is included.

helm install elk . -n elk
