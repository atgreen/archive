# EGCL support

The `egcl` branch uses `EGCL-POSIX` for native pathname metadata.
Run from the repository root:

```sh
egcl --no-init --load tests/egcl-metadata.lisp
```

All seven stat accessors are supported. Integer file descriptors are explicitly
unsupported because EGCL-POSIX does not expose fstat.
