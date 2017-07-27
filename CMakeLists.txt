cmake_minimum_required(VERSION 2.8)
project(InstParser)

set(HEADER_FILES
    ./InstrumentsParserApp.h
    ./PFTTrackSegment.h
    ./UIARun.h
    ./Utils.h
    ./XRActivityInstrumentRun.h
    ./XRObjectAllocRun.h
    ./XRRun.h
    ./XRStreamedPowerRun.h
    ./XRVideoCardRun.h
)

set(SOURCE_FILES
    ./InstrumentsParserApp.m
    ./PFTTrackSegment.m
    ./UIARun.m
    ./Utils.m
    ./XRActivityInstrumentRun.m
    ./XRObjectAllocRun.m
    ./XRRun.m
    ./XRStreamedPowerRun.m
    ./XRVideoCardRun.m
    ./main.m
)
		
include_directories(
	${CMAKE_CURRENT_SOURCE_DIR}
)

add_executable(${PROJECT_NAME} ${HEADER_FILES} ${INLINE_FILES} ${SOURCE_FILES})

