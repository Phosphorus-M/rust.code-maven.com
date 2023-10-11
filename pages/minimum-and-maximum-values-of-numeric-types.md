---
title: Minimum and maximum values of Rust numeric types
timestamp: 2023-10-03T07:00:01
description: To avoid overflowing or underflowing the numeric types one can check against the minimum and maximum possible values.
tags:
    - MIN
    - MAX
    - u8
    - i8
    - u128
    - i128
    - f32
    - f64
    - isize
    - usize
---

If you'd like to make sure that your computations don't result in a number that cannot fit into the numeric type you are using,
you can always makes some comparison before the computation to the minimum and maximum values of the numeric types.

Here you can see the MIN and MAX values of most of the numeric types of Rust:

![](examples/min-max-values/src/main.rs)

```
u8::MIN 0
u8::MAX 255

i8::MIN -128
i8::MAX 127

u64::MIN 0
u64::MAX 18446744073709551615

i64::MIN -9223372036854775808
i64::MAX 9223372036854775807

u128::MIN 0
u128::MAX 340282366920938463463374607431768211455

i128::MIN -170141183460469231731687303715884105728
i128::MAX 170141183460469231731687303715884105727

f32::MIN -340282350000000000000000000000000000000
f32::MAX 340282350000000000000000000000000000000

f64::MIN -179769313486231570000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
f64::MAX 179769313486231570000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000

usize::MIN 0
usize::MAX 18446744073709551615

isize::MIN -9223372036854775808
isize::MAX 9223372036854775807
```
