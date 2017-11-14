# karasawa-on-tv
Karasawa Takahiro(39) on TV.

# How to decrypt

- Add `com.github.nao20010128nao:Cryptorage:1d24df7` on [jitpack.io](https://jitpack.io) as a dependency.
- Loading files over the Internet may require faster network. (The following way)

## Kotlin

```kotlin
val crypt = URL("https://github.com/AnKoushinist/karasawa-on-tv/raw/master/data")
    .asFileSource()
    .withV1Encryption("karasawaOnTv")
```

## Groovy

```groovy
@Grab('com.github.nao20010128nao:Cryptorage:1d24df7')
@GrabResolver(name='jitpack',root='https://jitpack.io')
import com.nao20010128nao.Cryptorage.internal.UtilsKt

def dir=UtilsKt.asFileSource(new URL("https://github.com/AnKoushinist/karasawa-on-tv/raw/master/data"))

def crypt=UtilsKt.withV1Encryption(dir,'karasawaOnTv')

```

# Contents
- `karasawa.mp4` - letter-boxed video
- `karasawa.final.webm` - 720p video
- `karasawa.2k.webm` - 2k video

**Note:** WebM files can be streamed over the Internet.
