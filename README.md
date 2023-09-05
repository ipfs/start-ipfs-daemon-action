# Start IPFS Daemon Action

The action starts IPFS daemon and waits for it to become ready.

## Inputs

| Name | Description | Default |
| --- | --- | --- |
| args | Arguments that should be passed to the ipfs daemon command | --init --init-profile server |
| wait-for-addrs | Whether waits for addresses to be assigned to the daemon | true |

## Example

```
- uses: ipfs/download-ipfs-distribution-action@v1
- uses: ipfs/start-ipfs-daemon-action@v1
```

```
- uses: actions/setup-go@v4
  with:
    go-version: 'stable'
- run: go install github.com/ipfs/go-ipfs/cmd/ipfs@latest
  shell: bash
- uses: ipfs/start-ipfs-daemon-action@v1
```
