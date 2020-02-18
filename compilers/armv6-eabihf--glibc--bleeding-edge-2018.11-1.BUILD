package(default_visibility = ['//visibility:public'])

filegroup(
  name = 'gcc',
  srcs = [
    'bin/armv6-linux-gcc',
  ],
)

filegroup(
  name = 'ar',
  srcs = [
    'bin/armv6-linux-ar',
  ],
)

filegroup(
  name = 'ld',
  srcs = [
    'bin/armv6-linux-ld',
  ],
)

filegroup(
  name = 'nm',
  srcs = [
    'bin/armv6-linux-nm',
  ],
)

filegroup(
  name = 'objcopy',
  srcs = [
    'bin/armv6-linux-objcopy',
  ],
)

filegroup(
  name = 'objdump',
  srcs = [
    'bin/armv6-linux-objdump',
  ],
)

filegroup(
  name = 'strip',
  srcs = [
    'bin/armv6-linux-strip',
  ],
)

filegroup(
  name = 'as',
  srcs = [
    'bin/armv6-linux-as',
  ],
)

filegroup(
  name = 'compiler_pieces',
  srcs = glob([
    'armv6-buildroot-linux-gnu/**',
    'libexec/**',
    'lib/gcc/armv6-buildroot-linux-gnu/**',
    'include/**',
  ]),
)

filegroup(
  name = 'compiler_components',
  srcs = [
    ':gcc',
    ':ar',
    ':ld',
    ':nm',
    ':objcopy',
    ':objdump',
    ':strip',
    ':as',
  ],
)

