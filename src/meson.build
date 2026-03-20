template_sources = [
  'main.vala',
  'application.vala',
  'window.vala',
]

template_deps = [
  config_dep,
  dependency('gtk4'),
  dependency('libadwaita-1', version: '>= 1.4'),
]

template_sources += gnome.compile_resources('template-resources',
  'template.gresource.xml',
  c_name: 'template'
)

executable('template', template_sources,
  dependencies: template_deps,
  include_directories: config_inc,
       install: true,
)
