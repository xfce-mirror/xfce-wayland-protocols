project(
  'xfce-wayland-protocols',
  version: '0.1.0-dev',
  license: 'MIT',
)

pkgdatadir = get_option('prefix') / get_option('datadir') / 'xfce4' / 'xfce-wayland-protocols'
install_data(
  'xfce-foreign-toplevel-management-private-v1.xml',
  'xfce-output-management-private-v1.xml',
  'xfce-output-private-v1.xml',
  install_dir: pkgdatadir,
)

pc = import('pkgconfig')
pc.generate(
  name: 'xfce-wayland-protocols',
  description: 'Private Xfce Wayland protocol descriptions',
  filebase: 'xfce-wayland-protocols',
  install_dir: get_option('prefix') / get_option('datadir') / 'pkgconfig',
  variables: [
    'pkgdatadir=${datadir}/xfce4/xfce-wayland-protocols',
  ],
)
