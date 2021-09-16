project('utfcpp', 'cpp',
  version : '0.1',
  default_options : ['warning_level=3', 'cpp_std=c++17'])


utfcpp_dep = declare_dependency(
	include_directories : include_directories('./source')
)

host_system = host_machine.system()

if host_system == 'windows'
  # add_global_link_arguments('/utf-8', language : 'cpp')
  add_global_arguments('/utf-8', language : 'cpp')
  add_global_arguments('/DUTF_CPP_CPLUSPLUS=201703L', language : 'cpp')
endif


