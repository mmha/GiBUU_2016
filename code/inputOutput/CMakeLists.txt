add_library(gibuu_callstack CallStack.f90)
add_library(gibuu_output output.f90)

add_library(gibuu_inputOutput
	EventOutputFile.f90
	input.f90
	statistics.f90
)

target_link_libraries(gibuu_output
	PUBLIC
		gibuu_particleDefinition
)

target_link_libraries(gibuu_inputOutput PUBLIC
	gibuu_output
	gibuu_callstack
)