add_executable(ch02-substring_sort-01 01a_substring_sort.C 01a_substring_sort_a.C 01a_substring_sort_b.C 01a_substring_sort_c.C)

# int 和 unsigned 时间差不多
add_executable(ch02-int_unsigned 05_compare_timer.C)
add_executable(ch02-int_unsigned_2 05a_compare_timer.C)
add_executable(ch02-int_unsigned_3 06_compare_timer.C)
add_executable(ch02-int_unsigned_4 07_compare_timer.C)
add_executable(ch02-int_unsigned_5 08_compare_timer.C)
add_executable(ch02-int_unsigned_6 09_compare_timer.C)


add_executable(ch02-int_unsigned_7 10_compare_mbm.C)
target_link_libraries(ch02-int_unsigned_7 ${Benchmark_LIB})

add_executable(ch02-int_unsigned_long_8 10a_compare_mbm.C)
target_link_libraries(ch02-int_unsigned_long_8 ${Benchmark_LIB})

add_executable(ch02-int_unsigned_long_9 11_compare_mbm.C 11_compare_mbm_a.C 11_compare_mbm_b.C 11_compare_mbm_c.C)
target_link_libraries(ch02-int_unsigned_long_9 ${Benchmark_LIB})

add_executable(ch02-12a-int_unsigned_long 12_compare_mbm_a.C)
target_link_libraries(ch02-12a-int_unsigned_long ${Benchmark_LIB})

add_executable(ch02-12b-int_unsigned_long 12_compare_mbm_b.C)
target_link_libraries(ch02-12b-int_unsigned_long ${Benchmark_LIB})

add_executable(ch02-12c-int_unsigned_long 12_compare_mbm_c.C)
target_link_libraries(ch02-12c-int_unsigned_long ${Benchmark_LIB})

add_executable(ch02-12d-int_unsigned_long 12_compare_mbm_d.C)
target_link_libraries(ch02-12d-int_unsigned_long ${Benchmark_LIB})

add_executable(ch02-12e-int_unsigned_long 12_compare_mbm_e.C)
target_link_libraries(ch02-12e-int_unsigned_long ${Benchmark_LIB})

add_executable(ch02-12f-int_unsigned_long 12_compare_mbm_f.C)
target_link_libraries(ch02-12f-int_unsigned_long ${Benchmark_LIB})

add_executable(ch02-12g-int_unsigned_long 12_compare_mbm_g.C)
target_link_libraries(ch02-12g-int_unsigned_long ${Benchmark_LIB})
