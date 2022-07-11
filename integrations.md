# Integrations

## Fields

### id

Unique identifier for this input, this probably auto-generates?

### name

the name of this input.

### revision

Simple revision tracker, unknown purpose.

### type

The integration this stream comes from, see the `manifest.yaml` of each integration within `integration/packages` folder of the `elastic/Integrations` repository.

### data_stream

Contains just one child field, `namespace`. (this may be wrong, please check source code first of agent's config!) More information from Elastic example configuration files:

* Namespace name must conform to the naming conventions for Elasticsearch indices, cannot contain dashes (-), and cannot exceed 100 bytes
* For index naming restrictions, see https://www.elastic.co/guide/en/elasticsearch/reference/current/indices-create-index.html#indices-create-api-path-params

### use_output

#### Description

The name of the output object defined you wish to use.

```yaml
use_output: my_output
```

### meta

What integration package and version of said package to use.

```yaml
meta:
  package:
    name: kubernetes
    version: 0.2.8
```

### streams

Streams are their own unique objects, see Streams documentation due to complexity.