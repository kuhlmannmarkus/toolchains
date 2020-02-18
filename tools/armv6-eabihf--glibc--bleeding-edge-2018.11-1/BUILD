package(default_visibility = ["//visibility:public"])

cc_toolchain_suite(
    name = "toolchain",
    # target_cpu | compiler
    toolchains = {
        "armv6-eabihf|gcc": "bootlin-armv6-eabihf",
        "armv6-eabihf": "bootlin-armv6-eabihf",
    },
)

filegroup(
    name = "linux_all_files",
    srcs = [
        "//tools/armv6-eabihf--glibc--bleeding-edge-2018.11-1/armv6-linux:tool-wrappers",
        "@bootlin_armv6_toolchain//:compiler_pieces",
    ],
)

filegroup(
    name = "linux_linker_files",
    srcs = [
        "//tools/armv6-eabihf--glibc--bleeding-edge-2018.11-1/armv6-linux:ar",
        "//tools/armv6-eabihf--glibc--bleeding-edge-2018.11-1/armv6-linux:gcc",
        "//tools/armv6-eabihf--glibc--bleeding-edge-2018.11-1/armv6-linux:ld",
        "@bootlin_armv6_toolchain//:compiler_pieces",
    ],
)

filegroup(
    name = "linux_compiler_files",
    srcs = [
        "//tools/armv6-eabihf--glibc--bleeding-edge-2018.11-1/armv6-linux:as",
        "//tools/armv6-eabihf--glibc--bleeding-edge-2018.11-1/armv6-linux:gcc",
        "//tools/armv6-eabihf--glibc--bleeding-edge-2018.11-1/armv6-linux:ld",
    ],
)

# Here we'll keep things simple by including all files ditributed in archives.
filegroup(
    name = "all",
    srcs = glob(["**/*"]),
)

filegroup(
    name = "empty",
    srcs = [],
)

cc_toolchain(
    name = "bootlin-armv6-eabihf",
    all_files = ":linux_all_files",
    ar_files = "//tools/armv6-eabihf--glibc--bleeding-edge-2018.11-1/armv6-linux:ar",
    as_files = "//tools/armv6-eabihf--glibc--bleeding-edge-2018.11-1/armv6-linux:as",
    compiler_files = ":linux_compiler_files",
    cpu = "armv6-eabihf",
    dwp_files = ":empty",
    dynamic_runtime_lib = ":empty",
    linker_files = ":linux_linker_files",
    objcopy_files = "//tools/armv6-eabihf--glibc--bleeding-edge-2018.11-1/armv6-linux:objcopy",
    static_runtime_lib = ":empty",
    strip_files = "//tools/armv6-eabihf--glibc--bleeding-edge-2018.11-1/armv6-linux:strip",
    supports_param_files = 1,
    visibility = ["//visibility:public"],
)
