## ProxyChains
Setup
- `sudo nano /etc/proxychains.conf`
- Uncomment `random_chain`
- comment `dynamic_chain` and `strict_chain`
- uncomment `chain_len` make number higher the better
- comment `127.0.0.1 9050` if not using tor
- add proxys