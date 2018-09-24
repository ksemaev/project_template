For ES 6.x:

```console
$ helm install stable/elastalert --set writebackIndex=elastalert

# Open Dev Tools on Kibana and send the below.
# Otherwise elastalert ends up with errors like "RequestError: TransportError(400, u'search_phase_execution_exception', u'No mapping found for [alert_time] in order to sort on')"
PUT /elastalert/_mapping/elastalert
{
  "properties": {
      "alert_time": {"type": "date"}
  }
}
```

See the comment in the default `values.yaml` to know why `writebackIndex` is required for ES 6.x.
