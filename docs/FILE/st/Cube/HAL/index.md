# HAL库简介

ST公司为方便用户更好的使用STM32系列的MCU,共计推出四种库,目前主流的是`HAL`库

如果想要了解有关四种官方库之间的对比,可以参考[ST官方库的对比](../../other/compare.md#st官方库对比)

`HAL`的全程为`硬件抽象层`,是为了更好的进行不同芯片之间的移植而开发的库,主要包括三部分

- [HAL库](hal)
- [LL库](ll)
- [Core drivers(optional)](cd)