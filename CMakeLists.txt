cmake_minimum_required(VERSION 3.26)
project(Final_Project)

set(CMAKE_CXX_STANDARD 17)

set(Boost_INCLUDE_DIR /opt/homebrew/Cellar/boost/1.83.0/include)
set(Boost_LIBRARY_DIR /opt/homebrew/Cellar/boost/1.83.0/lib)
find_package(Boost COMPONENTS system filesystem REQUIRED)
include_directories(${Boost_INCLUDE_DIR})

add_executable(Final_Project main.cpp
        soa.hpp
        products.hpp
        inquiryservice.hpp
        tradebookingservice.hpp
        positionservice.hpp
        riskservice.hpp
        streamingservice.hpp
        marketdataservice.hpp
        historicaldataservice.hpp
        executionservice.hpp
        pricingservice.hpp
        functions.hpp
        algostreamingservice.hpp
        algoexecutionservice.hpp
        guiservice.hpp
        datageneration.hpp
)
