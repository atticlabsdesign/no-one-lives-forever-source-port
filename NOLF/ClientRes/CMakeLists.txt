set(PROJECT_NAME ClientRes)

################################################################################
# Source groups
################################################################################
set(no_group_source_files
    "arrow.cur"
    "credits.txt"
    "intro.txt"
)
source_group("" FILES ${no_group_source_files})

set(Headers
    "resource.h"
)
source_group("Headers" FILES ${Headers})

set(Sources
    "main.cpp"
)
source_group("Sources" FILES ${Sources})

set(ALL_FILES
    ${no_group_source_files}
    ${Headers}
    ${Sources}
)

################################################################################
# Target
################################################################################
add_library(${PROJECT_NAME} SHARED ${ALL_FILES})

use_props(${PROJECT_NAME} "${CMAKE_CONFIGURATION_TYPES}" "${DEFAULT_CXX_PROPS}")
################################################################################
# Target name
################################################################################
set_target_properties(${PROJECT_NAME} PROPERTIES
    TARGET_NAME_DEBUG        "CRes"
    TARGET_NAME_FINALDEBUG   "CRes"
    TARGET_NAME_FINALRELEASE "CRes"
    TARGET_NAME_RELEASE      "CRes"
    TARGET_NAME_TEMPLATE     "CRes"
)
################################################################################
# Output directory
################################################################################
set_target_properties(${PROJECT_NAME} PROPERTIES
    OUTPUT_DIRECTORY_DEBUG        "${CMAKE_CURRENT_SOURCE_DIR}/debug"
    OUTPUT_DIRECTORY_FINALDEBUG   "${CMAKE_CURRENT_SOURCE_DIR}/debug"
    OUTPUT_DIRECTORY_FINALRELEASE "${CMAKE_CURRENT_SOURCE_DIR}/release"
    OUTPUT_DIRECTORY_RELEASE      "${CMAKE_CURRENT_SOURCE_DIR}/release"
    OUTPUT_DIRECTORY_TEMPLATE     "${CMAKE_CURRENT_SOURCE_DIR}/debug"
)
set_target_properties(${PROJECT_NAME} PROPERTIES
    ARCHIVE_OUTPUT_DIRECTORY_DEBUG        "${CMAKE_CURRENT_SOURCE_DIR}/./Debug"
    ARCHIVE_OUTPUT_DIRECTORY_FINALDEBUG   "${CMAKE_CURRENT_SOURCE_DIR}/./Debug"
    ARCHIVE_OUTPUT_DIRECTORY_FINALRELEASE "${CMAKE_CURRENT_SOURCE_DIR}/./Release"
    ARCHIVE_OUTPUT_DIRECTORY_RELEASE      "${CMAKE_CURRENT_SOURCE_DIR}/./Release"
    ARCHIVE_OUTPUT_DIRECTORY_TEMPLATE     "${CMAKE_CURRENT_SOURCE_DIR}/./Debug"
)
set_target_properties(${PROJECT_NAME} PROPERTIES
    ARCHIVE_OUTPUT_NAME_DEBUG        "CRes"
    ARCHIVE_OUTPUT_NAME_FINALDEBUG   "CRes"
    ARCHIVE_OUTPUT_NAME_FINALRELEASE "CRes"
    ARCHIVE_OUTPUT_NAME_RELEASE      "CRes"
    ARCHIVE_OUTPUT_NAME_TEMPLATE     "CRes"
)
################################################################################
# MSVC runtime library
################################################################################
get_property(MSVC_RUNTIME_LIBRARY_DEFAULT TARGET ${PROJECT_NAME} PROPERTY MSVC_RUNTIME_LIBRARY)
string(CONCAT "MSVC_RUNTIME_LIBRARY_STR"
    $<$<CONFIG:Debug>:
        MultiThreadedDebug
    >
    $<$<CONFIG:FinalDebug>:
        MultiThreadedDebug
    >
    $<$<CONFIG:FinalRelease>:
        MultiThreaded
    >
    $<$<CONFIG:Release>:
        MultiThreaded
    >
    $<$<CONFIG:Template>:
        MultiThreadedDebug
    >
    $<$<NOT:$<OR:$<CONFIG:Debug>,$<CONFIG:FinalDebug>,$<CONFIG:FinalRelease>,$<CONFIG:Release>,$<CONFIG:Template>>>:${MSVC_RUNTIME_LIBRARY_DEFAULT}>
)
set_target_properties(${PROJECT_NAME} PROPERTIES MSVC_RUNTIME_LIBRARY ${MSVC_RUNTIME_LIBRARY_STR})

################################################################################
# Include directories
################################################################################
target_include_directories(${PROJECT_NAME} PUBLIC
    "${CMAKE_CURRENT_SOURCE_DIR}/../Shared"
)

################################################################################
# Compile definitions
################################################################################
target_compile_definitions(${PROJECT_NAME} PRIVATE
    "$<$<CONFIG:Debug>:"
        "_DEBUG"
    ">"
    "$<$<CONFIG:FinalDebug>:"
        "_DEBUG"
    ">"
    "$<$<CONFIG:FinalRelease>:"
        "NDEBUG"
    ">"
    "$<$<CONFIG:Release>:"
        "NDEBUG"
    ">"
    "$<$<CONFIG:Template>:"
        "_DEBUG"
    ">"
    "WIN32;"
    "_WINDOWS"
)

################################################################################
# Compile and link options
################################################################################
if(MSVC)
    target_compile_options(${PROJECT_NAME} PRIVATE
        $<$<CONFIG:Debug>:
            /Gm;
            /Od;
            /Gy-
        >
        $<$<CONFIG:FinalDebug>:
            /Gm;
            /Od;
            /Gy-
        >
        $<$<CONFIG:FinalRelease>:
            /O2;
            /GF;
            /Gy
        >
        $<$<CONFIG:Release>:
            /O2;
            /GF;
            /Gy
        >
        $<$<CONFIG:Template>:
            /Gm;
            /Od;
            /Gy-
        >
        /W3;
        ${DEFAULT_CXX_DEBUG_INFORMATION_FORMAT};
        ${DEFAULT_CXX_EXCEPTION_HANDLING}
    )
    target_link_options(${PROJECT_NAME} PRIVATE
        $<$<CONFIG:Debug>:
            /DEBUG;
            /INCREMENTAL
        >
        $<$<CONFIG:FinalDebug>:
            /DEBUG;
            /INCREMENTAL
        >
        $<$<CONFIG:FinalRelease>:
            /DEBUG:FULL;
            /INCREMENTAL:NO
        >
        $<$<CONFIG:Release>:
            /DEBUG:FULL;
            /INCREMENTAL:NO
        >
        $<$<CONFIG:Template>:
            /DEBUG;
            /INCREMENTAL
        >
        /NOLOGO;
        /SUBSYSTEM:WINDOWS
    )
endif()

################################################################################
# Post build events
################################################################################
add_custom_command_if(
    TARGET ${PROJECT_NAME}
    POST_BUILD
    COMMANDS
    COMMAND        $<CONFIG:Debug> copy debug\\cres.dll $ENV{NOLF_BUILD_DIR}
    COMMAND   $<CONFIG:FinalDebug> copy debug\\cres.dll $ENV{NOLF_BUILD_DIR}
    COMMAND $<CONFIG:FinalRelease> copy release\\cres.dll $ENV{NOLF_BUILD_DIR}
    COMMAND      $<CONFIG:Release> copy release\\cres.dll $ENV{NOLF_BUILD_DIR}
    COMMAND     $<CONFIG:Template> copy debug\\cres.dll $ENV{NOLF_BUILD_DIR}
)

################################################################################
# Dependencies
################################################################################
set(ADDITIONAL_LIBRARY_DEPENDENCIES
    "odbc32;"
    "odbccp32"
)
target_link_libraries(${PROJECT_NAME} PUBLIC "${ADDITIONAL_LIBRARY_DEPENDENCIES}")

