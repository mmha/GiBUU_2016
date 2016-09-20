add_library(gibuu_run
	checks.f90
	povray.f90
)

target_link_libraries(gibuu_run
	PUBLIC
		gibuu_database
)