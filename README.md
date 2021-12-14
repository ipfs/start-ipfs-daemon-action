# Start IPFS Daemon Action

The action starts IPFS daemon and waits for it to become ready.

## Inputs

| Name | Description | Default |
| --- | --- | --- |
| args | Arguments that should be passed to the ipfs daemon command | --init --init-profile server |

## Example

```
- uses: ipfs/download-ipfs-distribution-action@master
- uses: ipfs/start-ipfs-daemon-action@master
```

```
- uses: actions/setup-go@v2
  with:
    go-version: '1.16.x'
- uses: protocol/cache-go-action@master
- run: go install github.com/ipfs/go-ipfs/cmd/ipfs@latest
  shell: bash
- uses: ipfs/start-ipfs-daemon-action@master
```
