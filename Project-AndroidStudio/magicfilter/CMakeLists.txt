cmake_minimum_required(VERSION 3.4.1)

add_library(
    magic
    SHARED
    src/main/jni/MagicJni.cpp
    src/main/jni/bitmap/BitmapOperation.cpp
    src/main/jni/bitmap/Conversion.cpp
    src/main/jni/bitmap/JniBitmap.h
    src/main/jni/beautify/MagicBeautify.cpp)

target_link_libraries(
    magic
    log
    jnigraphics)