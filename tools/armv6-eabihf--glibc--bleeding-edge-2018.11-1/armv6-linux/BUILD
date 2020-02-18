package(default_visibility = ["//tools/armv6-eabihf--glibc--bleeding-edge-2018.11-1:__pkg__"])

filegroup(
    name = "gcc",
    srcs = [
        "armv6-linux-gcc",
        "@bootlin_armv6_toolchain//:gcc",
    ],
)

filegroup(
    name = "ar",
    srcs = [
        "armv6-linux-ar",
        "@bootlin_armv6_toolchain//:ar",
    ],
)

filegroup(
    name = "ld",
    srcs = [
        "armv6-linux-ld",
        "@bootlin_armv6_toolchain//:ld",
    ],
)

filegroup(
    name = "nm",
    srcs = [
        "armv6-linux-nm",
        "@bootlin_armv6_toolchain//:nm",
    ],
)

filegroup(
    name = "objcopy",
    srcs = [
        "armv6-linux-objcopy",
        "@bootlin_armv6_toolchain//:objcopy",
    ],
)

filegroup(
    name = "objdump",
    srcs = [
        "armv6-linux-objdump",
        "@bootlin_armv6_toolchain//:objdump",
    ],
)

filegroup(
    name = "strip",
    srcs = [
        "armv6-linux-strip",
        "@bootlin_armv6_toolchain//:strip",
    ],
)

filegroup(
    name = "as",
    srcs = [
        "armv6-linux-as",
        "@bootlin_armv6_toolchain//:as",
    ],
)

filegroup(
    name = "tool-wrappers",
    srcs = [
        ":ar",
        ":as",
        ":gcc",
        ":ld",
        ":nm",
        ":objcopy",
        ":objdump",
        ":strip",
    ],
)
