project('softfloat', ['c'],
  # license_files: ['LICENSE.txt'],
  version: '2c',
  meson_version: '>=0.47.0')

softfloat_files = [
  'src/softfloat.c',
]

softfloat_inc = [include_directories('include')]

librzsoftfloat = library('softfloat', softfloat_files,
  include_directories: softfloat_inc,
  implicit_include_directories: false,
  install: false,
)

softfloat_dep = declare_dependency(
  link_with: librzsoftfloat,
  include_directories: softfloat_inc,
)
