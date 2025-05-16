project('Arkanoid', ['c', 'cpp'],
  version : '0.1',
  default_options : ['warning_level=3', 'cpp_std=c++20', 'c_std=c11'])

glfw_dep = dependency('glfw3')

# Specify OpenGL dependency
gl_dep = dependency('gl')

# Thread dependency (covers pthread)
thread_dep = dependency('threads')

# X11 dependencies
x11_dep = dependency('x11', required : false)
xrandr_dep = dependency('xrandr', required : false)
xi_dep = dependency('xi', required : false)

glfw_all_deps = [glfw_dep, thread_dep, x11_dep, xrandr_dep, xi_dep]

subdir('deps/glad')

executable('Arkanoid',
           'helloworl.cpp',
           install : true,
           dependencies: [glfw_all_deps, gl_dep, glad_dep])
