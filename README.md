# aerospike

### AeroLab

Install aerolab on macOS:
```bash
brew install aerospike/tools/aerolab
```

#### AeroLab Config

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
  --aws-profile default \
  --aws-nopublic-ip
```

#### AeroLab Cluster Setup

Create a new cluster:
```bash
aerolab cluster create \
  --name aerospike-cluster \
  --count 2
```
