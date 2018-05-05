progs = [
	['1.colors',['1.colors','1.lamp']],
	['2.1.basic_lighting_diffuse',['2.1.basic_lighting','2.1.lamp']],
	['2.2.basic_lighting_specular',['2.2.basic_lighting','2.2.lamp']],
	['3.1.materials',['3.1.materials','3.1.lamp']],
	['3.2.materials_exercise1',['3.2.materials','3.2.lamp']],
	['4.1.lighting_maps_diffuse_map',['4.1.lighting_maps','4.1.lamp']],
	['4.2.lighting_maps_specular_map',['4.2.lighting_maps','4.2.lamp']],
	['4.3.lighting_maps_exercise4',['4.3.lighting_maps','4.3.lamp']],
	['5.1.light_casters_directional',['5.1.light_casters','5.1.lamp']],
	['5.2.light_casters_point',['5.2.light_casters','5.2.lamp']],
	['5.3.light_casters_spot',['5.3.light_casters','5.3.lamp']],
	['5.4.light_casters_spot_soft',['5.4.light_casters','5.4.lamp']],
	['6.multiple_lights',['6.multiple_lights','6.lamp']],
]

conf_data = configuration_data()

foreach p : progs
	executable(p[0],
		join_paths(p[0], p[0].split('.')[-1] + '.cpp'),
		dependencies : my_dep,
		include_directories : my_inc,
	)

	if p[1] != []
		foreach x : p[1]
			configure_file(input: join_paths(p[0], x + '.vs'),
		       output: x + '.vs',
		       configuration : conf_data)

			configure_file(input: join_paths(p[0], x + '.fs'),
		       output: x  + '.fs',
		       configuration : conf_data)
		endforeach
	endif

endforeach