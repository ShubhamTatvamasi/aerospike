# aerospike

### AeroLab

Install aerolab on macOS:
```bash
brew install aerospike/tools/aerolab
```

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
