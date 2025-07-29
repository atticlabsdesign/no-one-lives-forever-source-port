set(PROJECT_NAME ClientShellDLL)

################################################################################
# Source groups
################################################################################
set(Headers
    "../Shared/AssertMgr.h"
    "../Shared/AttachButeMgr.h"
    "../Shared/BankedList.h"
    "../Shared/BankedList_impl.h"
    "../Shared/BareList.h"
    "../Shared/CharacterAlignment.h"
    "../Shared/CheatDefs.h"
    "../Shared/ClientServerShared.h"
    "../Shared/CommandIDs.h"
    "../Shared/CommonUtilities.h"
    "../Shared/ContainerCodes.h"
    "../Shared/CRC32.h"
    "../Shared/CSDefs.h"
    "../Shared/DamageTypes.h"
    "../Shared/DebrisMgr.h"
    "../Shared/DebrisTypes.h"
    "../Shared/DebugNew_impl.h"
    "../Shared/FXButeMgr.h"
    "../Shared/FXStructs.h"
    "../Shared/GameButeMgr.h"
    "../Shared/GibTypes.h"
    "../Shared/GlobalMgr.h"
    "../Shared/Globals.h"
    "../Shared/MissionData.h"
    "../Shared/MissionMgr.h"
    "../Shared/ModelButeMgr.h"
    "../Shared/MsgIDs.h"
    "../Shared/NetDefs.h"
    "../Shared/Objectives.h"
    "../Shared/SCDefs.h"
    "../Shared/ServerOptionMgr.h"
    "../Shared/SFXMsgIds.h"
    "../Shared/SharedBaseFXStructs.h"
    "../Shared/SharedFXStructs.h"
    "../Shared/SharedMission.h"
    "../Shared/SharedMovement.h"
    "../Shared/SoundMgr.h"
    "../Shared/SoundTypes.h"
    "../Shared/Stdafx.h"
    "../Shared/SurfaceFunctions.h"
    "../Shared/SurfaceMgr.h"
    "../Shared/TeamMgr.h"
    "../Shared/TemplateList.h"
    "../Shared/Timer.h"
    "../Shared/VersionMgr.h"
    "../Shared/WeaponFXTypes.h"
    "../Shared/WeaponMgr.h"
    "BaseFolder.h"
    "BaseLineSystemFX.h"
    "BaseMenu.h"
    "BaseParticleSystemFX.h"
    "BasePolyDrawFX.h"
    "BaseScaleFX.h"
    "BaseSelectionFolder.h"
    "BeamFX.h"
    "BitmapCtrl.h"
    "BodyFX.h"
    "BulletTrailFX.h"
    "CameraFX.h"
    "CameraOffsetMgr.h"
    "CharacterFX.h"
    "client_physics.h"
    "ClientButeMgr.h"
    "ClientInfoMgr.h"
    "ClientSoundMgr.h"
    "ClientUtilities.h"
    "ClientWeaponUtils.h"
    "CMoveMgr.h"
    "Credits.h"
    "CycleCtrl.h"
    "DamageFXMgr.h"
    "DeathFX.h"
    "DebrisFX.h"
    "DynamicLightFX.h"
    "ExplosionFX.h"
    "FastList.h"
    "FireFX.h"
    "FlashLight.h"
    "FolderAdvDisplay.h"
    "FolderAudio.h"
    "FolderAwards.h"
    "FolderBriefing.h"
    "FolderCommands.h"
    "FolderControls.h"
    "FolderCrosshair.h"
    "FolderCustomControls.h"
    "FolderCustomLevel.h"
    "FolderDifficulty.h"
    "FolderDisplay.h"
    "FolderEffects.h"
    "FolderEscape.h"
    "FolderFavoriteLevels.h"
    "FolderGadgets.h"
    "FolderGallery.h"
    "FolderGame.h"
    "FolderGear.h"
    "FolderHost.h"
    "FolderHostLevels.h"
    "FolderHostOptions.h"
    "FolderIntel.h"
    "FolderInventory.h"
    "FolderJoin.h"
    "FolderJoinLAN.h"
    "FolderJoystick.h"
    "FolderKeyboard.h"
    "FolderLoad.h"
    "FolderMain.h"
    "FolderMgr.h"
    "FolderMission.h"
    "FolderMods.h"
    "FolderMouse.h"
    "FolderMulti.h"
    "FolderMultiBriefing.h"
    "FolderMultiSummary.h"
    "FolderNew.h"
    "FolderObjectives.h"
    "FolderOptions.h"
    "FolderPerformance.h"
    "FolderPlayer.h"
    "FolderSave.h"
    "FolderSingle.h"
    "FolderStats.h"
    "FolderSummary.h"
    "FolderSupplies.h"
    "FolderTexture.h"
    "FolderViewInventory.h"
    "FolderWeaponControls.h"
    "FolderWeapons.h"
    "GameButes.h"
    "GameClientShell.h"
    "GameSettings.h"
    "GibFX.h"
    "GroupCtrl.h"
    "HeadBobMgr.h"
    "IntelItemMgr.h"
    "InterfaceMeter.h"
    "InterfaceMgr.h"
    "InterfaceResMgr.h"
    "InterfaceSurfMgr.h"
    "InterfaceTimer.h"
    "IpMgr.h"
    "JoystickAxis.h"
    "KeyFixes.h"
    "LaserBeam.h"
    "LayoutMgr.h"
    "LeashFX.h"
    "LensFlareFX.h"
    "LightFX.h"
    "LightningFX.h"
    "LightScaleMgr.h"
    "LineSystemFX.h"
    "ListCtrl.h"
    "LoadingScreen.h"
    "LTDecisionWnd.h"
    "LTDialogueWnd.h"
    "LTMaskedWnd.h"
    "LTMenuWnd.h"
    "LTMultiWnd.h"
    "LTTextWnd.h"
    "LtWnd.h"
    "LTWndMessages.h"
    "MarkSFX.h"
    "MenuJoystickAxis.h"
    "MessageBox.h"
    "MessageBoxCtrl.h"
    "MessageMgr.h"
    "MineFX.h"
    "MissionText.h"
    "MouseMgr.h"
    "MultiplayerMenu.h"
    "Music.h"
    "MuzzleFlashFX.h"
    "MuzzleFlashParticleFX.h"
    "NetInfo.h"
    "NetStart.h"
    "NodeController.h"
    "NodeLinesFX.h"
    "ObjEditMgr.h"
    "Overlays.h"
    "ParticleExplosionFX.h"
    "ParticleShowerFX.h"
    "ParticleSystemFX.h"
    "ParticleTrailFX.h"
    "ParticleTrailSegmentFX.h"
    "PickupItemFX.h"
    "PlayerCamera.h"
    "PlayerData.h"
    "PlayerSoundFX.h"
    "PlayerStats.h"
    "PlayerVehicleFX.h"
    "PolyDebrisFX.h"
    "PolyGridFX.h"
    "PolyLineFX.h"
    "PopupText.h"
    "ProjectileFX.h"
    "PVFXMgr.h"
    "RandomSparksFX.h"
    "ScreenTintMgr.h"
    "SearchLightFX.h"
    "SFXMgr.h"
    "SharedDefs.h"
    "ShellCasingFX.h"
    "SliderCtrl.h"
    "SmokeFX.h"
    "SoundFX.h"
    "Sparam.h"
    "SpecialFX.h"
    "SpecialFXList.h"
    "sprinklesfx.h"
    "StaticTextCtrl.h"
    "SteamFX.h"
    "Subtitle.h"
    "TracerFX.h"
    "VarTrack.h"
    "VehicleMgr.h"
    "VideoFX.h"
    "VKDefs.h"
    "VolumeBrushFX.h"
    "WeaponChooser.h"
    "WeaponFX.h"
    "WeaponModel.h"
    "WeaponStringDefs.h"
    "WeatherFX.h"
    "WinUtil.h"
)
source_group("Headers" FILES ${Headers})

set(Source
    "../Shared/Animator.cpp"
    "../Shared/AssertMgr.cpp"
    "../Shared/AttachButeMgr.cpp"
    "../Shared/BareList.cpp"
    "../Shared/CommonUtilities.cpp"
    "../Shared/CRC32.cpp"
    "../Shared/DamageTypes.cpp"
    "../Shared/DebrisMgr.cpp"
    "../Shared/DebugNew.cpp"
    "../Shared/FXButeMgr.cpp"
    "../Shared/FXStructs.cpp"
    "../Shared/GameButeMgr.cpp"
    "../Shared/GlobalMgr.cpp"
    "../Shared/MissionMgr.cpp"
    "../Shared/ModelButeMgr.cpp"
    "../Shared/NetDefs.cpp"
    "../Shared/PlayerSummary.cpp"
    "../Shared/ServerOptionMgr.cpp"
    "../Shared/SharedFXStructs.cpp"
    "../Shared/SharedMission.cpp"
    "../Shared/SoundFilterMgr.cpp"
    "../Shared/SoundMgr.cpp"
    "../Shared/Stdafx.cpp"
    "../Shared/SurfaceFunctions.cpp"
    "../Shared/SurfaceMgr.cpp"
    "../Shared/TeamMgr.cpp"
    "../Shared/TemplateList.cpp"
    "../Shared/VersionMgr.cpp"
    "../Shared/WeaponMgr.cpp"
    "BaseLineSystemFX.cpp"
    "BaseMenu.cpp"
    "BaseParticleSystemFX.cpp"
    "BasePolyDrawFX.cpp"
    "BaseScaleFX.cpp"
    "BeamFX.cpp"
    "BodyFX.cpp"
    "BulletTrailFX.cpp"
    "CameraOffsetMgr.cpp"
    "CharacterFX.cpp"
    "client_physics.cpp"
    "ClientButeMgr.cpp"
    "ClientInfoMgr.cpp"
    "ClientSoundMgr.cpp"
    "ClientUtilities.cpp"
    "ClientWeaponUtils.cpp"
    "CMoveMgr.cpp"
    "Credits.cpp"
    "DamageFXMgr.cpp"
    "DeathFX.cpp"
    "DebrisFX.cpp"
    "DynamicLightFX.cpp"
    "ExplosionFX.cpp"
    "FireFX.cpp"
    "FlashLight.cpp"
    "GameClientShell.cpp"
    "GibFX.cpp"
    "GlobalClientMgr.cpp"
    "HeadBobMgr.cpp"
    "IntelItemMgr.cpp"
    "InterfaceMeter.cpp"
    "InterfaceTimer.cpp"
    "IpMgr.cpp"
    "KeyFixes.cpp"
    "LaserBeam.cpp"
    "LaserTriggerFX.cpp"
    "LeashFX.cpp"
    "LensFlareFX.cpp"
    "LightFX.cpp"
    "LightningFX.cpp"
    "LightScaleMgr.cpp"
    "LineSystemFX.cpp"
    "MarkSFX.cpp"
    "MessageBox.cpp"
    "MessageBoxCtrl.cpp"
    "MessageMgr.cpp"
    "MineFX.cpp"
    "MissionText.cpp"
    "MultiplayerMenu.cpp"
    "Music.cpp"
    "MuzzleFlashFX.cpp"
    "MuzzleFlashParticleFX.cpp"
    "NodeController.cpp"
    "NodeLinesFX.cpp"
    "ObjEditMgr.cpp"
    "ObjSpriteFX.cpp"
    "ParticleExplosionFX.cpp"
    "ParticleShowerFX.cpp"
    "ParticleSystemFX.cpp"
    "ParticleTrailFX.cpp"
    "ParticleTrailSegmentFX.cpp"
    "PickupItemFX.cpp"
    "PlayerCamera.cpp"
    "PlayerSoundFX.cpp"
    "PlayerStats.cpp"
    "PlayerVehicleFX.cpp"
    "PolyDebrisFX.cpp"
    "PolyGridFX.cpp"
    "PolyLineFX.cpp"
    "ProjectileFX.cpp"
    "PVFXMgr.cpp"
    "RandomSparksFX.cpp"
    "ScreenTintMgr.cpp"
    "SearchLightFX.cpp"
    "SFXMgr.cpp"
    "ShellCasingFX.cpp"
    "SmokeFX.cpp"
    "SoundFX.cpp"
    "Sparam.cpp"
    "SpecialFXList.cpp"
    "sprinklesfx.cpp"
    "SteamFX.cpp"
    "Subtitle.cpp"
    "TracerFX.cpp"
    "VehicleMgr.cpp"
    "VideoFX.cpp"
    "VKDefs.cpp"
    "WeaponChooser.cpp"
    "WeaponFX.cpp"
    "WeaponModel.cpp"
    "WeatherFX.cpp"
    "WinUtil.cpp"
)
source_group("Source" FILES ${Source})

set(Source__Interface
    "../Shared/MissionData.cpp"
    "BaseFolder.cpp"
    "BaseSelectionFolder.cpp"
    "BitmapCtrl.cpp"
    "CycleCtrl.cpp"
    "FolderAdvDisplay.cpp"
    "FolderAudio.cpp"
    "FolderAwards.cpp"
    "FolderBriefing.cpp"
    "FolderControls.cpp"
    "FolderCrosshair.cpp"
    "FolderCustomControls.cpp"
    "FolderCustomLevel.cpp"
    "FolderDifficulty.cpp"
    "FolderDisplay.cpp"
    "FolderEffects.cpp"
    "FolderEscape.cpp"
    "FolderFavoriteLevels.cpp"
    "FolderGadgets.cpp"
    "FolderGallery.cpp"
    "FolderGame.cpp"
    "FolderGear.cpp"
    "FolderHost.cpp"
    "FolderHostLevels.cpp"
    "FolderHostOptions.cpp"
    "FolderIntel.cpp"
    "FolderInventory.cpp"
    "FolderJoin.cpp"
    "FolderJoinLAN.cpp"
    "FolderJoystick.cpp"
    "FolderKeyboard.cpp"
    "FolderLoad.cpp"
    "FolderMain.cpp"
    "FolderMgr.cpp"
    "FolderMission.cpp"
    "FolderMods.cpp"
    "FolderMouse.cpp"
    "FolderMulti.cpp"
    "FolderMultiBriefing.cpp"
    "FolderMultiSummary.cpp"
    "FolderNew.cpp"
    "FolderObjectives.cpp"
    "FolderOptions.cpp"
    "FolderPerformance.cpp"
    "FolderPlayer.cpp"
    "FolderSave.cpp"
    "FolderSingle.cpp"
    "FolderStats.cpp"
    "FolderSummary.cpp"
    "FolderTexture.cpp"
    "FolderViewInventory.cpp"
    "FolderWeaponControls.cpp"
    "FolderWeapons.cpp"
    "GameSettings.cpp"
    "GroupCtrl.cpp"
    "InterfaceMgr.cpp"
    "InterfaceResMgr.cpp"
    "InterfaceSurfMgr.cpp"
    "JoystickAxis.cpp"
    "LayoutMgr.cpp"
    "ListCtrl.cpp"
    "LoadingScreen.cpp"
    "LTDecisionWnd.cpp"
    "LTDialogueWnd.cpp"
    "LTMaskedWnd.cpp"
    "LTMenuWnd.cpp"
    "LTMultiWnd.cpp"
    "LTTextWnd.cpp"
    "LtWnd.cpp"
    "MouseMgr.cpp"
    "PopupText.cpp"
    "SliderCtrl.cpp"
    "StaticTextCtrl.cpp"
)
source_group("Source\\Interface" FILES ${Source__Interface})

function(add_sources_if_exist TARGET)
    foreach(SOURCE_FILE ${ARGN})
        if(EXISTS "${CMAKE_CURRENT_SOURCE_DIR}/${SOURCE_FILE}")
            target_sources(${TARGET} PRIVATE ${SOURCE_FILE})
        else()
            message(STATUS "Skipping missing file: ${SOURCE_FILE}")
        endif()
    endforeach()
endfunction()

################################################################################
# Target
################################################################################
add_library(${PROJECT_NAME} SHARED)

# Add sources using the conditional function
add_sources_if_exist(${PROJECT_NAME} ${Headers})
add_sources_if_exist(${PROJECT_NAME} ${Source})
add_sources_if_exist(${PROJECT_NAME} ${Source__Interface})

target_precompile_headers(${PROJECT_NAME} PRIVATE
    "$<$<COMPILE_LANGUAGE:CXX>:${CMAKE_CURRENT_SOURCE_DIR}/../Shared/Stdafx.h>"
)

use_props(${PROJECT_NAME} "${CMAKE_CONFIGURATION_TYPES}" "${DEFAULT_CXX_PROPS}")
################################################################################
# Target name
################################################################################
set_target_properties(${PROJECT_NAME} PROPERTIES
    TARGET_NAME_DEBUG        "CShell"
    TARGET_NAME_FINALDEBUG   "CShell"
    TARGET_NAME_FINALRELEASE "CShell"
    TARGET_NAME_RELEASE      "CShell"
)
################################################################################
# Output directory
################################################################################
set_target_properties(${PROJECT_NAME} PROPERTIES
    OUTPUT_DIRECTORY_DEBUG        "${CMAKE_CURRENT_SOURCE_DIR}/debug"
    OUTPUT_DIRECTORY_FINALDEBUG   "${CMAKE_CURRENT_SOURCE_DIR}/Final_Debug"
    OUTPUT_DIRECTORY_FINALRELEASE "${CMAKE_CURRENT_SOURCE_DIR}/Final_Release"
    OUTPUT_DIRECTORY_RELEASE      "${CMAKE_CURRENT_SOURCE_DIR}/release"
)
set_target_properties(${PROJECT_NAME} PROPERTIES
    ARCHIVE_OUTPUT_DIRECTORY_DEBUG        "${CMAKE_CURRENT_SOURCE_DIR}/./Debug"
    ARCHIVE_OUTPUT_DIRECTORY_FINALDEBUG   "${CMAKE_CURRENT_SOURCE_DIR}/./Final_Debug"
    ARCHIVE_OUTPUT_DIRECTORY_FINALRELEASE "${CMAKE_CURRENT_SOURCE_DIR}/./Final_Release"
    ARCHIVE_OUTPUT_DIRECTORY_RELEASE      "${CMAKE_CURRENT_SOURCE_DIR}/./Release"
)
set_target_properties(${PROJECT_NAME} PROPERTIES
    ARCHIVE_OUTPUT_NAME_DEBUG        "CShell"
    ARCHIVE_OUTPUT_NAME_FINALDEBUG   "CShell"
    ARCHIVE_OUTPUT_NAME_FINALRELEASE "CShell"
    ARCHIVE_OUTPUT_NAME_RELEASE      "CShell"
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
    $<$<NOT:$<OR:$<CONFIG:Debug>,$<CONFIG:FinalDebug>,$<CONFIG:FinalRelease>,$<CONFIG:Release>>>:${MSVC_RUNTIME_LIBRARY_DEFAULT}>
)
set_target_properties(${PROJECT_NAME} PROPERTIES MSVC_RUNTIME_LIBRARY ${MSVC_RUNTIME_LIBRARY_STR})

################################################################################
# Include directories
################################################################################
target_include_directories(${PROJECT_NAME} PUBLIC
    "$<$<CONFIG:Debug>:"
        "${CMAKE_CURRENT_SOURCE_DIR}/../Shared;"
        "${CMAKE_CURRENT_SOURCE_DIR}/../../LT2/sdk/inc;"
        "${CMAKE_CURRENT_SOURCE_DIR}/../../LT2/lithshared/incs;"
        "${CMAKE_CURRENT_SOURCE_DIR}/."
    ">"
    "$<$<CONFIG:FinalDebug>:"
        "${CMAKE_CURRENT_SOURCE_DIR}/../Shared;"
        "${CMAKE_CURRENT_SOURCE_DIR}/../../LT2/sdk/inc;"
        "${CMAKE_CURRENT_SOURCE_DIR}/../../LT2/lithshared/incs;"
        "${CMAKE_CURRENT_SOURCE_DIR}/."
    ">"
    "$<$<CONFIG:FinalRelease>:"
        "${CMAKE_CURRENT_SOURCE_DIR}/../Shared;"
        "${CMAKE_CURRENT_SOURCE_DIR}/../../LT2/sdk/inc;"
        "${CMAKE_CURRENT_SOURCE_DIR}/../../LT2/lithshared/incs;"
        "${CMAKE_CURRENT_SOURCE_DIR}/."
    ">"
    "$<$<CONFIG:Release>:"
        "${CMAKE_CURRENT_SOURCE_DIR}/../Shared;"
        "${CMAKE_CURRENT_SOURCE_DIR}/../../LT2/sdk/inc;"
        "${CMAKE_CURRENT_SOURCE_DIR}/../../LT2/lithshared/incs;"
        "${CMAKE_CURRENT_SOURCE_DIR}/."
    ">"
)

################################################################################
# Compile definitions
################################################################################
target_compile_definitions(${PROJECT_NAME} PRIVATE
    "$<$<CONFIG:Debug>:"
        "_DEBUG;"
        "_CLIENTBUILD;"
        "WIN32;"
        "_WINDOWS;"
        "NO_PRAGMA_LIBS"
    ">"
    "$<$<CONFIG:FinalDebug>:"
        "_REZFILE;"
        "_FINAL;"
        "_DEBUG;"
        "_CLIENTBUILD;"
        "WIN32;"
        "_WINDOWS;"
        "NO_PRAGMA_LIBS"
    ">"
    "$<$<CONFIG:FinalRelease>:"
        "_REZFILE;"
        "_FINAL;"
        "NDEBUG;"
        "_CLIENTBUILD;"
        "WIN32;"
        "_WINDOWS;"
        "_NOLFBUILD;"
        "NO_PRAGMA_LIBS"
    ">"
    "$<$<CONFIG:Release>:"
        "NDEBUG;"
        "_CLIENTBUILD;"
        "WIN32;"
        "_WINDOWS;"
        "_NOLFBUILD;"
        "NO_PRAGMA_LIBS"
    ">"
)

################################################################################
# Compile and link options
################################################################################
if(MSVC)
    target_compile_options(${PROJECT_NAME} PRIVATE
        $<$<CONFIG:Debug>:
            /Gm;
            /Od;
            /Gy-;
            /W3
        >
        $<$<CONFIG:FinalDebug>:
            /Gm;
            /Od;
            /Gy-;
            /W3
        >
        $<$<CONFIG:FinalRelease>:
            /O2;
            /GF;
            /Gy;
            /W3
        >
        $<$<CONFIG:Release>:
            /O2;
            /GF;
            /Gy;
            /W3
        >
        ${DEFAULT_CXX_DEBUG_INFORMATION_FORMAT};
        ${DEFAULT_CXX_EXCEPTION_HANDLING}
    )
    target_link_options(${PROJECT_NAME} PRIVATE
        $<$<CONFIG:Debug>:
            /NOLOGO;
            /DEBUG;
            /SUBSYSTEM:WINDOWS;
            /INCREMENTAL
        >
        $<$<CONFIG:FinalDebug>:
            /NOLOGO;
            /DEBUG;
            /SUBSYSTEM:WINDOWS;
            /INCREMENTAL
        >
        $<$<CONFIG:FinalRelease>:
            /NODEFAULTLIB:LIBCMTD;
            /NOLOGO;
            /DEBUG:FULL;
            /SUBSYSTEM:WINDOWS;
            /INCREMENTAL:NO
        >
        $<$<CONFIG:Release>:
            /NODEFAULTLIB:LIBCMTD;
            /NOLOGO;
            /DEBUG:FULL;
            /SUBSYSTEM:WINDOWS;
            /INCREMENTAL:NO
        >
        $<$<CONFIG:Template>:
            /DEBUG:FULL
        >
    )
endif()

################################################################################
# Post build events
################################################################################
add_custom_command_if(
    TARGET ${PROJECT_NAME}
    POST_BUILD
    COMMANDS
    COMMAND        $<CONFIG:Debug> copy debug\\cshell.dll $ENV{NOLF_BUILD_DIR}
    COMMAND   $<CONFIG:FinalDebug> copy Final_Debug\\cshell.dll $ENV{NOLF_BUILD_DIR}
    COMMAND $<CONFIG:FinalRelease> copy Final_Release\\cshell.dll $ENV{NOLF_BUILD_DIR}
    COMMAND      $<CONFIG:Release> copy release\\cshell.dll $ENV{NOLF_BUILD_DIR}
)

################################################################################
# Dependencies
################################################################################
set(ADDITIONAL_LIBRARY_DEPENDENCIES
    "$<$<CONFIG:Debug>:"
        "odbc32;"
        "odbccp32"
    ">"
    "$<$<CONFIG:FinalDebug>:"
        "odbc32;"
        "odbccp32"
    ">"
    "$<$<CONFIG:FinalRelease>:"
        "odbc32;"
        "odbccp32"
    ">"
    "$<$<CONFIG:Release>:"
        "odbc32;"
        "odbccp32"
    ">"
)
target_link_libraries(${PROJECT_NAME} PUBLIC "${ADDITIONAL_LIBRARY_DEPENDENCIES}")

