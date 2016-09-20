add_library(gibuu_rmf
	RMF.f90
)

target_link_libraries(gibuu_rmf
	PUBLIC
		gibuu_database
)