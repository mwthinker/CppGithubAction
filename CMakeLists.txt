cmake_minimum_required(VERSION 3.21)
project(CppGithubAction
	LANGUAGES
		CXX
)

add_executable(CppGithubAction
	src/main.cpp
)

set_target_properties(CppGithubAction
	PROPERTIES
		CXX_STANDARD 20
		CXX_STANDARD_REQUIRED YES
		CXX_EXTENSIONS NO
)
