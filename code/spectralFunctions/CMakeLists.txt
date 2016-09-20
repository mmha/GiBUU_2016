add_library(gibuu_spectralFunctions
	spectralFunc.f90
	selfenergy_mesons.f90
	spectralFunc_mesons.f90
	selfenergy_baryons.f90
)

target_link_libraries(gibuu_spectralFunctions
	PUBLIC
	gibuu_inputOutput
)