project('learn-opengl', 'cpp')

gl = dependency('gl')

glfw3 = dependency('glfw3')

glad_sp = subproject('glad')
glad = glad_sp.get_variable('glad_dep')

glm = dependency('glm')

x11 = dependency('x11')
threads = dependency('threads')

cc = meson.get_compiler('c')
dl = cc.find_library('dl', required : false)

my_dep = [gl,glfw3,glad,glm,dl,x11,threads]

subdir('includes')
my_inc = [inc]

subdir('configuration')
my_inc += conf

subdir('src')
