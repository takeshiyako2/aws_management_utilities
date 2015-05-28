Amazon EBS Snapshot tool


# Installation

```
$ bundle install --path ./
```

# How to use

Edit config file.
```
$ cat config/manage_snapshot.yml
---
app_name: manage_snapshot
aws:
  access_key: xxxxxxxxxxxxxxxxxxxxxxx
  secret_key: xxxxxxxxxxxxxxxxxxxxxxxxxxxx
  owner_id: 0123456789
  region: ap-northeast-1
ec2:
  description: manage_snapshot
  instance_names:
    - instance_name1
    - instance_name2
    - instance_name3
gmail:
  from: test-to@example.jp
  to: test-from@gmail.com
  password: password
```

Run script.
```
$ ruby aws/manage_snapshot.rb
```

# TODO

Write test.
