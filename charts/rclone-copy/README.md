# rclone Helm for Kubernetes

## Usage:
- Create `rclone.conf` (either via `rclone configure` or from `rclone.conf.template`)
- Adapt `values.yaml` to contain your values.
- Install helm with: `helm install . -f values.yaml -n "mySource-mySoruceType-myDestType"` in this directory.

## Creating rclone.conf from scratch
- Download `rclone` (on Mac e.g. `brew install rclone`)
- Run the following commands:
```bash 
cd my-repository
rclone config --config "rclone.conf"
```
- Select `n` for "New remote"
- Now continue to follow the outlined steps for the storage provider you chose
