cmake_minimum_required(VERSION 3.3)
project(ECGAnalysis)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")
set(SOURCE_FILES Qrsdet.cpp Qrsdet2.cpp Qrsfilt.cpp Qrsdet.h Picqrs.c Analbeat.cpp Analbeat.h Bdac.cpp Bdac.h Classify.cpp Match.cpp Match.h Noisechk.cpp Postclas.cpp Rythmchk.cpp Rythmchk.h Easytest.cpp Bxb.cpp)
add_executable(ECGAnalysis ${SOURCE_FILES})


