# Run

## Run scheduler

Get current IP

```bash
ip route get 8.8.8.8 | head -1 | cut -d' ' -f7
```

Run scheduler

```bash
dask-scheduler
```

## Run worker

```bash
SHEDULERIP=$(ip route get 8.8.8.8 | head -1 | cut -d' ' -f7)
dask-worker $SHEDULERIP:8786
```