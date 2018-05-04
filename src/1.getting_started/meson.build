executable('1.2.hello_world_clear'
	,'1.2.helloworld_clear/hello_world_clear.cpp'
	,dependencies : my_dep
	,include_directories : my_inc
)

executable('3.3.shaders_class'
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

executable('4.2.textures_combined'
	,'4.2.textures_combined/textures_combined.cpp'
	,dependencies : my_dep
	,include_directories : my_inc
)

conf_data = configuration_data()
configure_file(input: '4.2.textures_combined/4.2.texture.fs',
               output: '4.2.texture.fs',
               configuration : conf_data)
configure_file(input: '4.2.textures_combined/4.2.texture.vs',
               output: '4.2.texture.vs',
               configuration : conf_data)

executable('5.1.transformations'
	,'5.1.transformations/transformations.cpp'
	,dependencies : my_dep
	,include_directories : my_inc
)

conf_data = configuration_data()
configure_file(input: '5.1.transformations/5.1.transform.fs',
               output: '5.1.transform.fs',
               configuration : conf_data)
configure_file(input: '5.1.transformations/5.1.transform.vs',
               output: '5.1.transform.vs',
               configuration : conf_data)