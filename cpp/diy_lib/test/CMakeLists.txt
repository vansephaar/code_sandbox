# Includes Catch in the project:
include_directories(/Users/sreeram/Tools/catch_cpp)
# include_directories(${CATCH_INCLUDE_DIR} ${COMMON_INCLUDES})
enable_testing(true)  # Enables unit-testing.

file(GLOB SRCS *.cpp)             # Attache all unit test sources
add_executable(unittest ${SRCS})  # Generate executable
