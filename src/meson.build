plugin_src = files([
    'binding.cpp',
    'grab.cpp',
    'swayfire.cpp',
])

all_src += plugin_src
all_src += files([
    'grab.hpp',
    'swayfire.hpp',
])

pms = shared_module('swayfire', plugin_src,
    dependencies: [wayfire, wlroots],
    install: true, install_dir: join_paths(get_option('libdir'), 'wayfire'))
