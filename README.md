# hello-world

hello, world

## PHP

```bash
php hello.php

#dump opcode
php -d opcache.enable_cli=1 -d opcache.opt_debug_level=0x10000 hello.php
```

## PHP FPM

```ini
ping.path = /hello
ping.response = hello, world
```

## nginx

```nginx
http {
    server {
        location = /hello {
            return 200 "hello, world";
        }
    }
}
```

## Assembly

```bash
gcc -c hello.S && ld -o hello hello.o
```
