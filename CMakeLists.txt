cmake_minimum_required(VERSION 2.8.4)

project(hmac_sha1_sample)

set(SOURCE_FILES sample.c src/hmac/hmac_sha1.c src/sha/sha1.c)

include_directories("/usr/local/include" ${PROJECT_SOURCE_DIR}/src)

link_directories("/usr/local/lib")

add_executable(hmac_sha1_sample ${SOURCE_FILES})
