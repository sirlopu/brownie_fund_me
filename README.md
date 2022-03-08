# Brownie Fund Me Project



## Notes

Run on rinkeby test network
```bash
brownie run scripts/deploy.py --network rinkeby
```

Adding local network to brownie networks

```bash
brownie networks add Ethereum ganache-local host=http://127.0.0.1:7545 chainid=1337

*Sample output:

Brownie v1.18.1 - Python development framework for Ethereum
    SUCCESS: A new network 'ganache-local' has been added
    └─ganache-local
        ├─id: ganache-local
        ├─chainid: 1337
        └─host: http://127.0.0.1:7545
```


```bash
brownie test -k test_only_owner_can_withdraw --network rinkeby
```