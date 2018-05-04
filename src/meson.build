l = shared_library('stb_image', 'stb_image.cpp', include_directories: inc, install : true)
stb_image = declare_dependency(include_directories:inc, link_with : l)

my_dep += stb_image

subdir('1.getting_started')