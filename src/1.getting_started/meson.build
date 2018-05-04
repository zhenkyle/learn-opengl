progs = [
	['1.2.hello_world_clear',''],
	['3.3.shaders_class','shader'],
	['4.2.textures_combined','texture'],
	['5.1.transformations','transform'],
	['6.1.coordinate_systems','coordinate_systems'],
	['6.2.coordinate_systems_depth','coordinate_systems'],
	['6.3.coordinate_systems_multiple','coordinate_systems'],
	['7.1.camera_circle','camera'],
	['7.2.camera_keyboard_dt','camera'],
	['7.3.camera_mouse_zoom','camera'],
	['7.4.camera_class','camera'],
]

conf_data = configuration_data()

foreach p : progs
	executable(p[0],
		join_paths(p[0], p[0].split('.')[-1] + '.cpp'),
		dependencies : my_dep,
		include_directories : my_inc,
	)

	if p[1] != ''
		q = p[0].split('.')

		configure_file(input: join_paths(p[0],q[0]+'.'+q[1]+'.'+ p[1] + '.vs'),
	       output: q[0]+'.'+q[1]+'.'+ p[1] + '.vs',
	       configuration : conf_data)

		configure_file(input: join_paths(p[0],q[0]+'.'+q[1]+'.'+ p[1] + '.fs'),
	       output: q[0]+'.'+q[1]+'.'+ p[1] + '.fs',
	       configuration : conf_data)
	endif

endforeach