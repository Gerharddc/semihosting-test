# Semihosting Test

This is a simple test project aiming to get semihosting debug working for Rust code running on a Cortex-M CPU emulated by Renode. It is based on what is presented in https://docs.rust-embedded.org/book/ to achieve something similar with QEMU.

This project is based on a DevContainer which includes Rust and Renode. It should also work on a system which has these natively installed.

The application can be compiled using:

    cargo build

After this, it can be run using:

    renode --net semi-test.resc

Ideally, the "uartSemihosting" console should now show "Hello, world!". Unfortunately, this does not work yet.