set(LibHashLibrary hash_lib)

add_library(${LibHashLibrary} STATIC
    sha256.h
    sha256.cpp) #Note: Only Need to add sha256 for now...

set_target_properties(${LibHashLibrary} PROPERTIES
    WINDOWS_EXPORT_ALL_SYMBOLS OFF
    POSITION_INDEPENDENT_CODE ON
    CXX_STANDARD 17
    CXX_STANDARD_REQUIRED ON)