include_directories(.)

add_executable(
  zero_to_hero

  test.cpp
)
target_link_libraries(
  zero_to_hero

  snark
)
target_include_directories(
  zero_to_hero

  PUBLIC
  ${DEPENDS_DIR}/libsnark
  ${DEPENDS_DIR}/libsnark/depends/libfqfft
  ${DEPENDS_DIR}/libsnark/depends/libff
)


add_executable(
  test-gadget

  test-gadget.cpp
)
target_link_libraries(
  test-gadget

  snark
)
target_include_directories(
  test-gadget

  PUBLIC
  ${DEPENDS_DIR}/libsnark
  ${DEPENDS_DIR}/libsnark/depends/libfqfft
  ${DEPENDS_DIR}/libsnark/depends/libff
)
