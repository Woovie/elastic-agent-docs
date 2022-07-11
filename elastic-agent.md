# Elastic Agent Standalone

This contains information about configuration options that apply to the Elastic Agent agent itself and not the integrations.

## inputs and outputs

#### Description

Both of these take a YAMl style list, either being named keys or a normal list.

#### Examples

```yaml
outputs:
  - name: my_output
    type: elasticsearch
```

or

```yaml
outputs:
  my_output:
    type: elasticsearch
```

## outputs

### type

#### Description

known supported options:
* elasticsearch

### hosts

#### Description

A list of hosts

#### Examples

```yaml
hosts: [127.0.0.1:9200]
```

```yaml
hosts:
- 127.0.0.1:9200
- another-host-here:9200
```

### api-key, username, password

#### Description

Typical, expected credential fields

## inputs

### Description

Inputs are handled as Integrations. Please see the Integrations document to better understand this.

