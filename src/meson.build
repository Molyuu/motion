motion_sources = [
  'main.c',
  'motion-application.c',
  'motion-window.c',
]

motion_deps = [
  dependency('gtk4'),
  dependency('libadwaita-1', version: '>= 1.4'),
]

motion_sources += gnome.compile_resources('motion-resources',
  'motion.gresource.xml',
  c_name: 'motion'
)

executable('motion', motion_sources,
  dependencies: motion_deps,
       install: true,
)
