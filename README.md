# libc-db (A libc database)

# Project

This project was made in 2014, the goal was to grab all libc from debian and ubuntu for use in exploit.

This repository hosts only metadata of each libc (file in packages, hash, package files, symbols), for raw binary libc, see [libc-bin](https://github.com/BestPig/libc-bin)

There is no reason to keep the database private

## Structure

The `filename` is the md5 hash of the libc

```
elf64-x86-64/
└── linux
    ├── debian
    │   ├── bullseye
    │   │   └── libc
    │   │       ├── libc6
    │   │       │   └── e63efc14f34504f4ac4cf7d63ed229ca
```

A sample file (truncated for the README.md)
```json
{
  "date": [
    "2019-05-02 15:24:41"
  ], 
  "md5": "e63efc14f34504f4ac4cf7d63ed229ca", 
  "name": "libc.so.6", 
  "package_files": [
    "lib/x86_64-linux-gnu/libnss_nisplus-2.28.so", 
    "lib/x86_64-linux-gnu/ld-2.28.so", 
  ],
  "package_name": "data", 
  "syms": {
      "fgets": 458560,
      "system": 281024
  }, 
  "tags": [
    "elf64-x86-64", 
    "linux", 
    "debian", 
    "sid", 
    "libc"
  ]
}

```

## Authors

**BestPig**

- Twitter: [@BestPig](https://twitter.com/BestPig)
- Github: [@BestPig](https://github.com/BestPig)

**WapiFlapi**

- Twitter: [@wapiflapi](https://twitter.com/wapiflapi)
- Github: [@wapiflapi](https://github.com/wapiflapi)
