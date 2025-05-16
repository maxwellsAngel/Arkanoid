glad_sources = ['src/glad.c']

glad_includes = include_directories('include')

glad_lib = static_library('glad',
    glad_sources,
    include_directories: glad_includes)

glad_dep = declare_dependency(
    link_with: glad_lib,
    include_directories: glad_includes
)