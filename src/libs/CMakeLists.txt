INCLUDE("../../cmake/macros.cmake")

IF(NOT OPTION_3RDPARTY_EXPAT)
	ADD_SUBDIRECTORY(txml)
ENDIF(NOT OPTION_3RDPARTY_EXPAT)

ADD_SUBDIRECTORY(tgf)
ADD_SUBDIRECTORY(tgfclient)
ADD_SUBDIRECTORY(tgfdata)
ADD_SUBDIRECTORY(robottools)
ADD_SUBDIRECTORY(learning)
ADD_SUBDIRECTORY(math)
ADD_SUBDIRECTORY(portability)

# Work-in-progress 
IF(NOT OPTION_OFFICIAL_ONLY)
	SD_ADD_SUBDIRECTORY(ephemeris)
	#SD_ADD_SUBDIRECTORY(metar)
ENDIF()


