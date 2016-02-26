Cloud.gov Common Concourse Resource
===================================

Get common concourse files needed for most pipelines.


If you want to use this resource just add the following to your pipeline:

```
- name: common
  type: cg-common
  source:
    bucket_name: {{private-bucket}}
    access_key_id: {{private-access-key-id}}
    secret_access_key: {{private-secret-access-key}}
    secrets_file: something.yml
    secrets_passphrase: {{private-passphrase}}
    bosh_cert: bosh.pem
```

This will get you a secrets file decrypted and a bosh UAA certificate.

