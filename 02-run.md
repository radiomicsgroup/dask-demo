# Run

## Run scheduler

Get current IP

```bash
SHEDULERIP=$(ip route get 8.8.8.8 | head -1 | cut -d' ' -f7)
echo $SHEDULERIP
```

Run scheduler

```bash
dask-scheduler
```

After run open a browser in <i>SHEDULERIP:8787</i> to see the scheduler web interface

## Run worker

```bash
dask-worker $SHEDULERIP:8786
```