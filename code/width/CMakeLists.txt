add_library(gibuu_width
	baryonWidth.f90
	baryonWidthMedium.f90
	baryonWidthMedium_tables.f90
	baryonWidthVacuum.f90
	deltaWidth.f90
	energyDetermination.f90
	mesonWidth.f90
	mesonWidthMedium.f90
	mesonWidthMedium_tables.f90
	mesonWidthVacuum.f90
	offShellPotential.f90
	proton_neutron_width_medium.f90
	relativeVelocity.f90
	rhoABIntegrandVariables.f90
)

target_link_libraries(gibuu_width PUBLIC gibuu_database)