CMAKE_MINIMUM_REQUIRED(VERSION 2.6)

PROJECT(HelloWorld)

# List all source files
SET(SOURCE_FILES
    HelloWorld.cpp)

# library path
INCLUDE_DIRECTORIES(${Example_SOURCE_DIR}/Library)
LINK_DIRECTORIES(${Example_BINARY_DIR}/Library)

# Create the executable target
ADD_EXECUTABLE(${PROJECT_NAME} ${SOURCE_FILES})

TARGET_LINK_LIBRARIES(${PROJECT_NAME} ExampleLibrary)

