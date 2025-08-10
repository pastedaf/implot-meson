project(
  'ImGui Plotting Library',
  'cpp',
  license : 'MIT',
  version : '0.16',
)

imgui_dep = dependency('imgui-docking', fallback : ['imgui-docking', 'imgui_dep'])

implot_inc = include_directories('.')
implot_src = files(
  'implot.cpp',
  'implot_items.cpp'
)

implot_lib = library(
  'implot',
  implot_src,
  dependencies: imgui_dep
)

implot_dep = declare_dependency(
  link_with : implot_lib,
  include_directories : implot_inc
)
