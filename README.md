# polymorphous-ipdps2025-artifacts

You should try to build cloog-isl yourself by building pluto (tag 0.13.0 or 0.12.0) since the libcloog-isl.so.4.0.0 contains dll that points to other libraries in pluto.

```
(base) amy@mycomputer:~/pluto-0.13.0/cloog-isl$ ldd ./.libs/libcloog-isl.so.4.0.0
        linux-vdso.so.1 (0x00007fff9527b000)
        libisl.so.23 => /home/amy/pluto-0.13.0/isl/.libs/libisl.so.23 (0x00007fd447605000)
        libosl.so.0 => /home/amy/pluto-0.13.0/openscop/.libs/libosl.so.0 (0x00007fd4473d2000)
        libgmp.so.10 => /usr/lib/x86_64-linux-gnu/libgmp.so.10 (0x00007fd447151000)
        libc.so.6 => /lib/x86_64-linux-gnu/libc.so.6 (0x00007fd446d60000)
        /lib64/ld-linux-x86-64.so.2 (0x00007fd447c4f000)
````
