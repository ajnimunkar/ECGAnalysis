#cmake_minimum_required(VERSION 3.6)
#project(ECGAnalyzer)
#
#set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")
#
#set(SOURCE_FILES main.cpp)
#add_executable(ECGAnalyzer ${SOURCE_FILES})

############################ Modified
cmake_minimum_required(VERSION 3.6)
project(ECGAnalysis)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")
set(SOURCE_FILES main.cpp bdac.c analbeat.c inputs.h noisechk.c postclas.c qrsdet.c qrsfilt.c rythmchk.c match.c classify.c  )
add_executable(ECGAnalysis ${SOURCE_FILES})

TARGET_LINK_LIBRARIES(ECGAnalysis wfdb)


########################
#cmake_minimum_required(VERSION 2.8.4)
#project(example)
#set(SOURCE_FILES main.c)
