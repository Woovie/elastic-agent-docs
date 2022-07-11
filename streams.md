# Streams

## Description

## Fields

### id

Optional, automatically generated

### data_stream

* `dataset`: Dataset name must conform to the naming conventions for Elasticsearch indices, cannot contain dashes (-), and cannot exceed 100 bytes
* `type`: The type of `data_stream`. Check the `input_group` within the chosen Integration's `manifest.json` under the `policy_templates` structure. It may not be listed though. This value is always either `logs` or `metrics`. It may be extremely obvious which is which based on your chosen integration.

### metricsets

The metricset to use from the chosen integration defined in the integrations' meta field.

### bearer_token_file

Optional

### hosts

Optional

### period

Optional

### ssl.certificate_authorities

Optional