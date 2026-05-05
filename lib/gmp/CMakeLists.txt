if(MSVC)
	set(CMAKE_C_FLAGS_RELEASE "/MD /O2 /Ob2 /D NDEBUG")
endif()

add_library(gmp mini-gmp.c)
target_link_libraries(gmp)

