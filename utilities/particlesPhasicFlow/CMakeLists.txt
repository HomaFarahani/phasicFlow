
set(source_files
particlesPhasicFlow.cpp
positionParticles/positionParticles.cpp 
positionOrdered/positionOrdered.cpp 
positionRandom/positionRandom.cpp
positionFile/positionFile.cpp
empty/empty.cpp
)
#set(link_lib phasicFlow Kokkos::kokkos Interaction Utilities)

set(link_lib phasicFlow Kokkos::kokkos Particles Utilities)

pFlow_make_executable_install(particlesPhasicFlow source_files link_lib)
