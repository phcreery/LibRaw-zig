# LibRaw

This is [LibRaw](https://www.libraw.org/) 0.21.4, packaged for [Zig](https://ziglang.org/).

## How to use it

First, update your `build.zig.zon`:

```
zig fetch --save=libraw  git+https://github.com/phcreery/LibRaw-zig
```

Next, add this snippet to your `build.zig` script:

```zig
const dep_libraw = b.dependency("libraw", .{
    .target = target,
    .optimize = optimize,
});
```

This will provide libraw as a static library to `your_compilation`.

## Creating

```
zig fetch --save=libraw https://github.com/LibRaw/LibRaw/archive/refs/tags/0.21.4.tar.gz
```
