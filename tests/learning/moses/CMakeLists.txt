ADD_CXXTEST(KnobTurningUTest)
TARGET_LINK_LIBRARIES(KnobTurningUTest
	moses
	comboreduct
	cogutil
)

# requires boost::math; don't build if not found.
IF(Boost_MATH_C99_FOUND)
	ADD_CXXTEST(NeighborSamplingUTest)
	TARGET_LINK_LIBRARIES(NeighborSamplingUTest
		moses
		comboreduct
		cogutil
	)
ENDIF(Boost_MATH_C99_FOUND)


ADD_CXXTEST(FieldSetUTest)
TARGET_LINK_LIBRARIES(FieldSetUTest
	moses
	comboreduct
	cogutil
)

ADD_CXXTEST(representationUTest)
TARGET_LINK_LIBRARIES(representationUTest
	moses
	comboreduct
	cogutil
)

ADD_CXXTEST(MOSESUTest)
TARGET_LINK_LIBRARIES(MOSESUTest
	moses_exec
	moses
	comboreduct
	cogutil		
)

ADD_CXXTEST(mixedUTest)
TARGET_LINK_LIBRARIES(mixedUTest
	moses_exec
	moses
	comboreduct
	cogutil		
)

ADD_CXXTEST(optimizationUTest)
TARGET_LINK_LIBRARIES(optimizationUTest
	moses
	comboreduct
	cogutil
)

ADD_CXXTEST(metapopulationUTest)
TARGET_LINK_LIBRARIES(metapopulationUTest
	moses
	comboreduct
	cogutil
)

ADD_CXXTEST(iostream_bscored_combo_treeUTest)
TARGET_LINK_LIBRARIES(iostream_bscored_combo_treeUTest
	moses
	comboreduct
	cogutil
)
