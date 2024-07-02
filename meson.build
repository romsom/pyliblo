project('pyliblo', 'cython', default_options: {'warning_level': '3'})
add_project_arguments(
  '-fno-strict-aliasing',
  '-Werror-implicit-function-declaration',
  '-Wfatal-errors',
  language: 'c'
)
lo = dependency('liblo', required: true)
py = import('python').find_installation('python3', pure: false)
dep_py = py.dependency()
subdir('src')
subdir('scripts')
#subdir('liblo')
