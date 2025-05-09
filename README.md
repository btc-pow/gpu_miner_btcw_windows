# gpu_miner_btcw_windows
CUDA GPU miner for BTCW on native Windows

You can use the same wallet.dat for all GPUs. You must tell the GPU to use a different stage2 selection number to ensure unique stage2 hashing when using the same stage1 keys.

GPU miner works on Windows10 and Windows11.


Start Bitcoin-Pow-QT
```
bitcoin-pow-qt.exe -emergencymining=1
```

Have at least 1 utxo in your wallet. 
Go to Window->Console  and  type the following command and hit the enter button on keyboard
```
generate
```


DO NOT start the BTCW GPU miner until the BTCW node has started its mining process.

# Make sure the kernel.ptx file is in the same folder as the exe
start the gpu miner for gpu number 1
```
BTCW_CUDA_MINER.exe 1
```

start the gpu miner for gpu number 2
```
BTCW_CUDA_MINER.exe 2
```

start the gpu miner for gpu number 3
```
BTCW_CUDA_MINER.exe 3
```

Here is a typical output when running
```
====GOING to STAGE2 NOW====:11774
====GOING to STAGE2 NOW====:11775
STAGE2 BLOCK DATA UPDATED - DEVICE
STAGE2 BLOCK DATA - CPU SIDE
STAGE2 BLOCK DATA - CPU SIDE
STAGE2 BLOCK DATA - CPU SIDE
STAGE2 BLOCK DATA - CPU SIDE
STAGE2 BLOCK DATA - CPU SIDE
STAGE2 BLOCK DATA - CPU SIDE
STAGE2 BLOCK DATA UPDATED - DEVICE
STAGE2 BLOCK DATA - CPU SIDE
STAGE2 BLOCK DATA - CPU SIDE
STAGE2 BLOCK DATA - CPU SIDE
STAGE2 BLOCK DATA - CPU SIDE
STAGE2 BLOCK DATA - CPU SIDE
STAGE2 BLOCK DATA - CPU SIDE
STAGE2 BLOCK DATA UPDATED - DEVICE
STAGE2 BLOCK DATA - CPU SIDE
STAGE2 BLOCK DATA - CPU SIDE
STAGE2 BLOCK DATA - CPU SIDE
STAGE2 BLOCK DATA - CPU SIDE
STAGE2 BLOCK DATA - CPU SIDE
========================PoW BLOCK FOUND========================
THREAD: 000000000000044d
NONCE: 8044d14000017afc
============OUTPUT HASH============
FA01128B45CF6B61349580F12631389BD1D68AFCD9A24EFD2701ADD700000000

STAGE2 BLOCK DATA - CPU SIDE
STAGE2 BLOCK DATA UPDATED - DEVICE

STAGE2 BLOCK DATA - CPU SIDE
STAGE2 BLOCK DATA - CPU SIDE
STAGE2 BLOCK DATA - CPU SIDE
STAGE2 BLOCK DATA - CPU SIDE
STAGE2 BLOCK DATA - CPU SIDE
STAGE2 BLOCK DATA - CPU SIDE
STAGE2 BLOCK DATA UPDATED - DEVICE
STAGE2 BLOCK DATA - CPU SIDE
STAGE2 BLOCK DATA - CPU SIDE


```