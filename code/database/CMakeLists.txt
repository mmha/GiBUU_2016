add_library(gibuu_database
	constants.f90
	decayChannels.f90
	EventTypes.f90
	leptonicID.f90
	particleProperties.f90
	tabNuclearMass.f90
)

add_library(gibuu_idtable
	IdTable.f90
)

target_link_libraries(gibuu_database
	PUBLIC
		gibuu_constants
		gibuu_inputOutput
		gibuu_idtable
)