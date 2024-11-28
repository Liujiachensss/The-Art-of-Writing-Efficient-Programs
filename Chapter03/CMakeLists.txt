add_executable(ch03-01-superscalar 01_superscalar.C)
target_link_libraries(ch03-01-superscalar PRIVATE ${Benchmark_LIB})

add_executable(ch03-02-branch 02_branch.C 02_branch_func.C)
target_link_libraries(ch03-02-branch PRIVATE ${Benchmark_LIB})