executable('hello_world_clear'
	,'1.2.helloworld_clear/hello_world_clear.cpp'
	,dependencies : my_dep
	,include_directories : my_inc
)

executable('shaders_class'
	,'3.3.shaders_class/shaders_class.cpp'
	,dependencies : my_dep
	,include_directories : my_inc
)

conf_data = configuration_data()
configure_file(input: '3.3.shaders_class/3.3.shader.fs',
               output: '3.3.shader.fs',
               configuration : conf_data)
configure_file(input: '3.3.shaders_class/3.3.shader.vs',
               output: '3.3.shader.vs',
               configuration : conf_data)