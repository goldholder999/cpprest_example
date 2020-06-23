cmake_minimum_required (VERSION 3.8)



add_executable (hello-cpprest "hello-cpprest.cpp" "hello-cpprest.h")

target_link_libraries(hello-cpprest PRIVATE
	cpprestsdk::cpprest 
	cpprestsdk::cpprestsdk_zlib_internal 
	cpprestsdk::cpprestsdk_boost_internal 
	cpprestsdk::cpprestsdk_brotli_internal
)
