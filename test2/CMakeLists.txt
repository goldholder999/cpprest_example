cmake_minimum_required (VERSION 3.8)



add_executable (test2 "test2.cpp" "test2.h")

target_link_libraries(test2 PRIVATE
	cpprestsdk::cpprest 
	cpprestsdk::cpprestsdk_zlib_internal 
	cpprestsdk::cpprestsdk_boost_internal 
	cpprestsdk::cpprestsdk_brotli_internal
)
