cmake_minimum_required(VERSION 3.21)
project(CppGithubAction
	LANGUAGES
		CXX
)

find_package(fmt CONFIG REQUIRED)

add_executable(CppGithubAction
	src/main.cpp
)

target_link_libraries(CppGithubAction
	PRIVATE
		fmt::fmt-header-only
)

set_target_properties(CppGithubAction
	PROPERTIES
		CXX_STANDARD 17
		CXX_STANDARD_REQUIRED YES
		CXX_EXTENSIONS NO
)
