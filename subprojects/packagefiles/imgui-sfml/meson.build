project('imgui-sfml', 'cpp',
        version: '2.5',
        license: 'MIT')

imgui_dep = dependency('imgui')
sfml_dep = dependency('sfml')
opengl_dep = dependency('gl')

# We do not look up sfml here because there are many different
# names for the .pc files and others and it is unclear which
# ones we should use. Thus users of this wrap must look up sfml
# by themselves and add it to their targets.
#
# This is suboptimal, hopefully this can be fixed once we have
# more usage experience.

is_lib = library('imgui-sfml', 'imgui-SFML.cpp',
    dependencies: [sfml_dep, imgui_dep, opengl_dep])

imgui_sfml_dep = declare_dependency(include_directories: '.',
                                    dependencies: imgui_dep,
                                    link_with: is_lib)
