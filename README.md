# karasawa-on-tv
Karasawa Takahiro(39) on TV.

# How to decrypt

Add `com.github.nao20010128nao:Cryptorage:1d24df7` on (jitpack.io)[https://jitpack.io] as a dependency.

## Kotlin

```
URL("https://github.com/AnKoushinist/karasawa-on-tv/raw/master/data")
    .asFileSource()
    .withV1Encryption('karasawaOnTv')
```

