project(hello)
set(CMAKE_CXX_FLAGS "-march=armv7-a -mfloat-abi=hard")
#[[set(CMAKE_EXE_LINKER_FLAGS "-march=armv7-a -mfloat-abi=hard")]]
SET (CMAKE_CXX_COMPILER_WORKS 1)
SET (CMAKE_C_COMPILER_WORKS 1)
add_executable(hello hello.cpp)
install(TARGETS hello DESTINATION bin)
