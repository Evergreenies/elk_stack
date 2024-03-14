# elk_stack

These are basic configurations for the ELK stack

TODO:

- Need to update the configuration file of logstash `loastash/config/logstash.conf` as per your requirements.
- Enable autoindexing in elastic search by below elastics each query, this query allows creating indexes with specified patterns as given -
  ```
  PUT /_cluster/settings
  {
    "persistent": {
      "action.auto_create_index": "service-*,service--*,development-*,development--*,qa-*,qa--*,prod-*,prod--*"
    }
  }
  ```
  Feel free to adjust as per your requirements.
