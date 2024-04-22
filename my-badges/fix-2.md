<img src="https://github.com/my-badges/my-badges/blob/master/src/all-badges/fix-commit/fix-2.png?raw=true" alt="I did 2 sequential fixes." title="I did 2 sequential fixes." width="128">
<strong>I did 2 sequential fixes.</strong>
<br><br>

Commits:

- <a href="https://github.com/Neptunium931/Csystem/commit/048ea7392733c701c333b5a2b0d73bc9fe749e0b">048ea73</a>: fix(delFruit): fix memory leak and not pointer to free memory
- <a href="https://github.com/Neptunium931/Csystem/commit/eed73e778867f5df92cb21256aaaa68d38f05b8b">eed73e7</a>: fix(fruit): not final refactor for linked lists

nead fix delete
=================================================================
==133976==ERROR: AddressSanitizer: SEGV on unknown address 0x000000000018 (pc 0x55709a6aff27 bp 0x5040000513a8 sp 0x7ffec699e4a0 T0)
==133976==The signal is caused by a WRITE memory access.
==133976==Hint: address points to the zero page.
f->nextFuit 0x5040000513d0
AddressSanitizer:DEADLYSIGNAL
=================================================================
==133973==ERROR: AddressSanitizer: SEGV on unknown address 0x000000000018 (pc 0x56774bfc8f27 bp 0x5040000513a8 sp 0x7ffc43f2bf50 T0)
==133973==The signal is caused by a WRITE memory access.
==133973==Hint: address points to the zero page.
    #0 0x56774bfc8f27 in delFruit src/protopeach.c:45
    #1 0x56774bfc6ea5 in fruitGestion_createMultipleFruit_impl tests/server.c:135
    #2 0x729b4275d690 in criterion_internal_test_main ../src/core/test.c:94
    #3 0x56774bfc2d54 in fruitGestion_createMultipleFruit_jmp tests/server.c:125
    #4 0x729b4275c95a in run_test_child ../src/core/runner_coroutine.c:230
    #5 0x729b4276a20e in bxfi_main ../subprojects/boxfort/src/sandbox.c:57
    #6 0x729b41e43ccf  (/usr/lib/libc.so.6+0x25ccf) (BuildId: 6542915cee3354fbcf2b3ac5542201faec43b5c9)
    #7 0x729b41e43d89 in __libc_start_main (/usr/lib/libc.so.6+0x25d89) (BuildId: 6542915cee3354fbcf2b3ac5542201faec43b5c9)
    #8 0x56774bfc24a4 in _start (/home/neptunium/l3/C/Csystem/criterion_tests_server+0x64a4) (BuildId: 4bd0f0a2be6a7823b1d5aa11567d105187171193)

AddressSanitizer can not provide additional info.
SUMMARY: AddressSanitizer: SEGV src/protopeach.c:45 in delFruit


Created by <a href="https://github.com/my-badges/my-badges">My Badges</a>