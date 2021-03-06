# gcs_dir

Uploads directories from local machine to GCP Cloud Storage buckets.

## Configuration

| Name        | Default | Required | Description              |
|-------------|---------|----------|--------------------------|
| dest_bucket |         | ✓        | Destination bucket name  |
| dir         |         | ✓        | Path to source directory |


Please read [Common Configuration](../../README.md#common-configuration) as well.

## Example

```YAML
---
- name: Example playbook
  hosts: local
  roles:
    - role: lazyninjas.gcp.gcs_dir
      gcp_region: europe-west3
      dest_bucket: my-bucket-name
      dir: ../dist/docs
```

## Roadmap

* Specify destination path
