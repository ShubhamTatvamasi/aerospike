# aerospike


## AeroLab

Install aerolab on macOS:
```bash
brew install aerospike/tools/aerolab
```

---

### AeroLab Config

Check the aerolab config:
```bash
aerolab config backend
```

Check aerolab default config:
```bash
aerolab config defaults
```

Configure aerolab for aws
```bash
aerolab config backend \
  --type aws \
  --region ap-south-1 \
  --aws-profile default
```

Allow public IP to create cluster:
```bash
aerolab config defaults \
  --key Cluster.Create.Aws.PublicIP \
  --value true
```

---

### AeroLab Cluster Setup

List the current clusters:
```bash
aerolab cluster list
```

Create a new cluster:
```bash
aerolab cluster create \
  --name aerospike-cluster \
  --count 2 \
  --instance-type t4g.medium \
  --distro amazon \
  --distro-version 2023 \
  --aws-disk "type=gp3,size=50"
```

Delete cluster:
```bash
aerolab cluster destroy \
  --name aerospike-cluster \
  --force
```


