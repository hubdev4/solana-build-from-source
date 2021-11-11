# Solana Test Validator Fail 

These are the steps that I was able to fix the error:

> Incompatible CPU detected: missing AVX2 support. Please build from source on the target


My setup: *Ubuntu 20.04 Intel(R) Core(TM) i7-2670QM*

First install the following packages	
```
sudo apt install libudev-dev  
sudo apt install libssl-dev
sudo apt install clang
```

1. Download and extract [Source code (tar.gz)](https://github.com/solana-labs/solana/releases/latest)
2. In the same directory run: `./scripts/cargo-install-all.sh .` and wait til complile finish.
3. Run `solana-test-validator`


Source:
https://docs.solana.com/cli/install-solana-cli-tools#build-from-source
