conf_data = configuration_data()
conf_data.set('MESON_SOURCE_DIR',meson.source_root())
configure_file(input: 'root_directory.h.in',
               output: 'root_directory.h',
               configuration : conf_data)
conf = include_directories('.')