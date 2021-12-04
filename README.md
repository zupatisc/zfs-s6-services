# zfs-s6-services
Personal Artix s6 service files for running (encrypted) zfs pools.
Be mindful of what other services will rely on this, for example the `mount-filesystem` service might require zfs-load-keys if you mount a pool via fstab.
There is no logging component here so any output will land in `/run/uncaught-logs/`
