[![Build status](https://github.com/twyleg/template_cpp_project/actions/workflows/unit_tests.yaml/badge.svg)]()
[![GitHub latest commit](https://badgen.net/github/last-commit/twyleg/template_cpp_project)](https://GitHub.com/twyleg/template_cpp_project/commit/)

# Template C++ Project

Simple CMake based template for a common C++ project.

## Dependencies

The template is based on the following components:

* CMake
* boost
* googletest
* fmt

For a Debian/Ubuntu system, run the following command to install the dependencies:

	sudo apt install \
		git \
		cmake \
		g++ \
		libfmt-dev \
		libboost-all-dev

GoogleTest is pulled in as a git submodule to avoid problems with missing cmake files in sub distributions.

## Usage

Clone, prepare and build with the following steps:

	git clone git@github.com:twyleg/template_cpp_project.git
	cd template_cpp_project

	git submodule init
	git submodule update
	
	mkdir build/
	cd build/
	cmake ../
	make

