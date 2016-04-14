cmake_minimum_required(VERSION 3.3)
project(Halide_NN)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

set(SOURCE_FILES
    dataloaders/common.hpp
    dataloaders/data.pb.cc
    dataloaders/data.pb.h
    dataloaders/db.cpp
    dataloaders/db.hpp
    dataloaders/io.cpp
    dataloaders/io.hpp
    dataloaders/test_io.cpp
    conv_bench.cpp
    layer_test.cpp
    layers.h
    train_test_conv_net.cpp
    utils.cpp
    utils.h
    vgg_forward.cpp)

add_executable(Halide_NN ${SOURCE_FILES})