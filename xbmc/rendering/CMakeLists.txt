find_all_sources(. rendering_SRCS)
if(TARGET_POSIX)
  find_all_sources(gl system_SRCS)
elseif(TARGET_WIN32)
  find_all_sources(dx system_SRCS)
endif()
add_sources(${rendering_SRCS} ${system_SRCS})
