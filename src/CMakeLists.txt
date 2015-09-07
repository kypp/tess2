set (MODULE_NAME tess2)

# Get all compilation units.
file (GLOB ${MODULE_NAME}_SRCS *.c)

# Create the library.
add_library (${MODULE_NAME} ${${MODULE_NAME}_SRCS})

install (TARGETS ${MODULE_NAME} 
		ARCHIVE DESTINATION lib 
		LIBRARY DESTINATION lib)