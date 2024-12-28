project('{{ cookiecutter.app_name }}', 'cpp')
gtkmm_dep = dependency('gtkmm-4.0', version: '>= 4.6.0')
exe_file = executable('{{ cookiecutter.app_name }}', 'main.cpp', 
  dependencies: gtkmm_dep
  # win_subsystem: 'windows',
)

