project( project_cml )
find_package( OpenCV REQUIRED )

add_executable( project_cml main.cpp PhotoMontage.cpp graph.cpp LinkedBlockList.cpp LoadLib.cpp ConjGrad.cpp maxflow.cpp stdafx.cpp GCoptimization.cpp)
target_link_libraries( project_cml ${OpenCV_LIBS} )

set( CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11 -march=native -O3 -pthread" )