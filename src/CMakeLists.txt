add_library(ctc
  printer.cpp
  ${ROOT_DIR}/include/ctc/printer.hpp
)

find_package(glm CONFIG REQUIRED)
target_link_libraries(ctc PUBLIC glm::glm)

target_include_directories(ctc PUBLIC
  $<BUILD_INTERFACE:${ROOT_DIR}/include>
  $<INSTALL_INTERFACE:include>
)