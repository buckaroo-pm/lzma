load('//:buckaroo_macros.bzl', 'buckaroo_deps')
load('//:subdir_glob.bzl', 'subdir_glob')

cxx_library(
  name = 'lzma',
  header_namespace = '',
  exported_headers = subdir_glob([
    ('src', '**/*.h'),
  ]),
  headers = {
    'config.h': 'config-generic.h',
  },
  srcs = glob([
    'src/lzma/**/*.c',
    'src/lzma/**/*.cpp',
  ]),
  licenses = glob([
    'COPYING.*',
  ]),
  deps = buckaroo_deps(),
  visibility = [
    'PUBLIC',
  ],
)
