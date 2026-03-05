add_library(studyGroupFinder
    src/groupController.cpp
)

add_executable(studyGroupFinderTest
    src/main.cpp
)

add_executable(studyGroupFinderAutomaticTesting
    tests/main_tests.cpp
)

target_link_libraries(studyGroupFinderTest PRIVATE studyGroupFinder)
target_link_libraries(studyGroupFinderAutomaticTesting PRIVATE studyGroupFinder)
target_link_libraries(studyGroupFinder PUBLIC fmt::fmt)

target_include_directories(studyGroupFinder PUBLIC include)