python_opt = get_option('with-python')
if python_opt == '3'
  python_dep = dependency('python3', version: '>= 3.3')
else
  python_dep = dependency('python2', version: '>= 2.7')
endif

shared_module('python', 'python.c',
  dependencies: [libgio_dep, hexchat_plugin_dep, python_dep],
  install: true,
  install_dir: plugindir,
  name_prefix: '',
)
