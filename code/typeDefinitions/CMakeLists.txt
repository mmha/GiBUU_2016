add_library(gibuu_particleDefinition
	particleDefinition.f90
)

add_library(gibuu_mediumDefinition
	mediumDefinition.f90
)

add_library(gibuu_preevdefinition
	preEventDefinition.f90
	PreEvListDefinition.f90
)

add_library(gibuu_typeDefinitions
	AnaEventDefinition.f90
	dichteDefinition.f90
	MassAssInfoDefinition.f90
	nucleusDefinition.f90
	particlePointerListDefinition.f90
	preEventDefinition.f90
	ValueRangeDefinition.f90
)

target_link_libraries(gibuu_particleDefinition
	PUBLIC
		gibuu_callstack
)

target_link_libraries(gibuu_typeDefinitions
	PUBLIC
		gibuu_particleDefinition
		gibuu_mediumDefinition
		gibuu_preevdefinition
		gibuu_callstack
		gibuu_output
)