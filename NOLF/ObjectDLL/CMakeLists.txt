set(PROJECT_NAME Object)

################################################################################
# Source groups
################################################################################
set(no_group_source_files
    "../Attributes/Music.txt"
)
source_group("" FILES ${no_group_source_files})

set(Header_Files
    "../Shared/AssertMgr.h"
    "../Shared/AttachButeMgr.h"
    "../Shared/BareList.h"
    "../Shared/CharacterAlignment.h"
    "../Shared/CheatDefs.h"
    "../Shared/ClientServerShared.h"
    "../Shared/CommandIDs.h"
    "../Shared/CommonUtilities.h"
    "../Shared/ContainerCodes.h"
    "../Shared/CSDefs.h"
    "../Shared/DamageTypes.h"
    "../Shared/DebrisMgr.h"
    "../Shared/DebrisTypes.h"
    "../Shared/DebugMgr.h"
    "../Shared/Factory.h"
    "../Shared/FastHeap.h"
    "../Shared/FastStack.h"
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
    "../Shared/PlayerSummary.h"
    "../Shared/SCDefs.h"
    "../Shared/ServerOptionMgr.h"
    "../Shared/SFXMsgIds.h"
    "../Shared/SharedBaseFXStructs.h"
    "../Shared/SharedFXStructs.h"
    "../Shared/SharedMission.h"
    "../Shared/SharedMovement.h"
    "../Shared/SoundFilterMgr.h"
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
    "AIBrain.h"
    "AINudge.h"
    "AIRegion.h"
    "AIRegionMgr.h"
    "AmmoBox.h"
    "Attachments.h"
    "Body.h"
    "BodyState.h"
    "Bouncer.h"
    "Breakable.h"
    "CachedFiles.h"
    "Camera.h"
    "CDynArray.h"
    "Character.h"
    "CharacterHitBox.h"
    "CharacterMgr.h"
    "CinematicTrigger.h"
    "ClientDeathSFX.h"
    "ClientFX.h"
    "ClientLightFX.h"
    "ClientSFX.h"
    "ClientWeaponSFX.h"
    "CommandMgr.h"
    "Controller.h"
    "CVarTrack.h"
    "DeathScene.h"
    "DebrisFuncs.h"
    "Destructible.h"
    "DestructibleModel.h"
    "DialogueWindow.h"
    "DisplayMeter.h"
    "DisplayTimer.h"
    "Door.h"
    "DoorKnob.h"
    "Editable.h"
    "EventCounter.h"
    "ExitTrigger.h"
    "Explosion.h"
    "Fire.h"
    "Fixture.h"
    "GameBase.h"
    "GameServerShell.h"
    "GameStartPoint.h"
    "GearItems.h"
    "Group.h"
    "HHWeaponModel.h"
    "HingedDoor.h"
    "Intelligence.h"
    "Joint.h"
    "Key.h"
    "KeyData.h"
    "KeyFramer.h"
    "keyframer_light.h"
    "KeyPad.h"
    "LaserTrigger.h"
    "Lightning.h"
    "Lock.h"
    "Mine.h"
    "ModItem.h"
    "MusicMgr.h"
    "NodeLine.h"
    "ObjectiveSprite.h"
    "ObjectMsgs.h"
    "ObjectRemover.h"
    "ParticleSystem.h"
    "PickupItem.h"
    "PlayerButes.h"
    "PlayerObj.h"
    "PlayerVehicle.h"
    "PolyGrid.h"
    "Projectile.h"
    "ProjectileTypes.h"
    "Prop.h"
    "PropType.h"
    "PropTypeMgr.h"
    "RandomSpawner.h"
    "RotatingDoor.h"
    "RotatingWorldModel.h"
    "ScaleSprite.h"
    "Scanner.h"
    "ScreenShake.h"
    "SearchLight.h"
    "SecurityCamera.h"
    "ServerButeMgr.h"
    "ServerMark.h"
    "ServerSoundMgr.h"
    "ServerUtilities.h"
    "SFXFuncs.h"
    "SoundFX.h"
    "Sparam.h"
    "Spawner.h"
    "Speaker.h"
    "Sprinkles.h"
    "Steam.h"
    "Switch.h"
    "TeleportPoint.h"
    "TranslucentWorldModel.h"
    "Trigger.h"
    "TriggerSound.h"
    "Video.h"
    "VolumeBrush.h"
    "VolumeBrushTypes.h"
    "Weapon.h"
    "WeaponItems.h"
    "Weapons.h"
    "WorldModelDebris.h"
    "WorldProperties.h"
    "ZipHook.h"
)
source_group("Header Files" FILES ${Header_Files})

set(Header_Files__AI_Header_Files
    "AI.h"
    "AIAnimal.h"
    "AIAnimalState.h"
    "AIAnimalStrategy.h"
    "AIButeMgr.h"
    "AIDog.h"
    "AIDogReactions.h"
    "AIGroup.h"
    "AIHelicopter.h"
    "AIHuman.h"
    "AIHumanReactions.h"
    "AIHumans.h"
    "AIHumanState.h"
    "AIHumanStrategy.h"
    "AIMovement.h"
    "AINode.h"
    "AINodeMgr.h"
    "AIPath.h"
    "AIPathMgr.h"
    "AIPoodle.h"
    "AIReactions.h"
    "AISense.h"
    "AIShark.h"
    "AISounds.h"
    "AIState.h"
    "AISteering.h"
    "AITarget.h"
    "AIUtils.h"
    "AIVehicle.h"
    "AIVehicleState.h"
    "AIVehicleStrategy.h"
    "AIVolume.h"
    "AIVolumeMgr.h"
)
source_group("Header Files\\AI Header Files" FILES ${Header_Files__AI_Header_Files})

set(Header_Files__Animation_Header_Files
    "../Shared/Animator.h"
    "AnimationLex.h"
    "AnimationLexSymbols.h"
    "AnimationMgr.h"
    "AnimationMgrHuman.h"
    "AnimationParse.h"
    "AnimationParser.h"
    "AnimationStd.h"
    "AnimatorAIAnimal.h"
    "AnimatorAIVehicle.h"
    "AnimatorPlayer.h"
)
source_group("Header Files\\Animation Header Files" FILES ${Header_Files__Animation_Header_Files})

set(SDK
    "../../LT2/sdk/inc/clientheaders.h"
    "../../LT2/sdk/inc/iaggregate.h"
    "../../LT2/sdk/inc/iclientshell.h"
    "../../LT2/sdk/inc/iltclient.h"
    "../../LT2/sdk/inc/iltcommon.h"
    "../../LT2/sdk/inc/iltcsbase.h"
    "../../LT2/sdk/inc/iltcursor.h"
    "../../LT2/sdk/inc/iltcustomdraw.h"
    "../../LT2/sdk/inc/iltdirectmusic.h"
    "../../LT2/sdk/inc/iltlightanim.h"
    "../../LT2/sdk/inc/iltmath.h"
    "../../LT2/sdk/inc/iltmessage.h"
    "../../LT2/sdk/inc/iltmodel.h"
    "../../LT2/sdk/inc/iltphysics.h"
    "../../LT2/sdk/inc/iltprelight.h"
    "../../LT2/sdk/inc/iltserver.h"
    "../../LT2/sdk/inc/iltsoundmgr.h"
    "../../LT2/sdk/inc/iltspritecontrol.h"
    "../../LT2/sdk/inc/iltstream.h"
    "../../LT2/sdk/inc/ilttexmod.h"
    "../../LT2/sdk/inc/ilttransform.h"
    "../../LT2/sdk/inc/iltvideomgr.h"
    "../../LT2/sdk/inc/iobjectplugin.h"
    "../../LT2/sdk/inc/iservershell.h"
    "../../LT2/sdk/inc/lithtech.h"
    "../../LT2/sdk/inc/ltanimtracker.h"
    "../../LT2/sdk/inc/ltassert.h"
    "../../LT2/sdk/inc/ltbasedefs.h"
    "../../LT2/sdk/inc/ltbasetypes.h"
    "../../LT2/sdk/inc/ltbbox.h"
    "../../LT2/sdk/inc/ltbeziercurve.h"
    "../../LT2/sdk/inc/ltcodes.h"
    "../../LT2/sdk/inc/ltengineobjects.h"
    "../../LT2/sdk/inc/ltlink.h"
    "../../LT2/sdk/inc/ltmatrix.h"
    "../../LT2/sdk/inc/ltplane.h"
    "../../LT2/sdk/inc/ltpvalue.h"
    "../../LT2/sdk/inc/ltquatbase.h"
    "../../LT2/sdk/inc/ltrect.h"
    "../../LT2/sdk/inc/ltrotation.h"
    "../../LT2/sdk/inc/ltserverobj.h"
    "../../LT2/sdk/inc/ltvector.h"
    "../../LT2/sdk/inc/serverheaders.h"
)
source_group("SDK" FILES ${SDK})

set(Source_Files
    "../../LT2/sdk/inc/ltquatbase.cpp"
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
    "../Shared/MissionData.cpp"
    "../Shared/MissionMgr.cpp"
    "../Shared/ModelButeMgr.cpp"
    "../Shared/NetDefs.cpp"
    "../Shared/PlayerSummary.cpp"
    "../Shared/ServerOptionMgr.cpp"
    "../Shared/SharedFXStructs.cpp"
    "../Shared/SharedMission.cpp"
    "../Shared/SharedMovement.cpp"
    "../Shared/SoundFilterMgr.cpp"
    "../Shared/SoundMgr.cpp"
    "../Shared/Stdafx.cpp"
    "../Shared/SurfaceFunctions.cpp"
    "../Shared/SurfaceMgr.cpp"
    "../Shared/TeamMgr.cpp"
    "../Shared/TemplateList.cpp"
    "../Shared/VersionMgr.cpp"
    "../Shared/WeaponMgr.cpp"
    "AIBrain.cpp"
    "AINudge.cpp"
    "AIRegion.cpp"
    "AIRegionMgr.cpp"
    "Alarm.cpp"
    "AmmoBox.cpp"
    "Attachments.cpp"
    "Body.cpp"
    "BodyState.cpp"
    "Breakable.cpp"
    "CachedFiles.cpp"
    "Camera.cpp"
    "Character.cpp"
    "CharacterHitBox.cpp"
    "CharacterMgr.cpp"
    "CinematicTrigger.cpp"
    "ClientLightFX.cpp"
    "ClientSFX.cpp"
    "ClientWeaponSFX.cpp"
    "CommandMgr.cpp"
    "Controller.cpp"
    "DebrisFuncs.cpp"
    "Destructible.cpp"
    "DestructibleModel.cpp"
    "DialogueWindow.cpp"
    "DisplayMeter.cpp"
    "DisplayTimer.cpp"
    "Door.cpp"
    "DoorKnob.cpp"
    "Editable.cpp"
    "EventCounter.cpp"
    "ExitTrigger.cpp"
    "Explosion.cpp"
    "Fire.cpp"
    "GameBase.cpp"
    "GameServerShell.cpp"
    "GameStartPoint.cpp"
    "GearItems.cpp"
    "GlobalServerMgr.cpp"
    "Group.cpp"
    "HHWeaponModel.cpp"
    "HingedDoor.cpp"
    "Intelligence.cpp"
    "IntelMgr.cpp"
    "Key.cpp"
    "KeyData.cpp"
    "KeyFramer.cpp"
    "keyframer_light.cpp"
    "KeyPad.cpp"
    "LaserTrigger.cpp"
    "Lightning.cpp"
    "Lock.cpp"
    "Mine.cpp"
    "ModItem.cpp"
    "MusicMgr.cpp"
    "MyGameSpyMgr.cpp"
    "NodeLine.cpp"
    "object_list.cpp"
    "ObjectiveSprite.cpp"
    "ObjectRemover.cpp"
    "ParticleSystem.cpp"
    "PickupItem.cpp"
    "PlayerObj.cpp"
    "PlayerVehicle.cpp"
    "PolyGrid.cpp"
    "Projectile.cpp"
    "ProjectileTypes.cpp"
    "Prop.cpp"
    "PropType.cpp"
    "PropTypeMgr.cpp"
    "RandomSpawner.cpp"
    "RotatingDoor.cpp"
    "RotatingWorldModel.cpp"
    "ScaleSprite.cpp"
    "Scanner.cpp"
    "ScreenShake.cpp"
    "SearchLight.cpp"
    "SecurityCamera.cpp"
    "ServerButeMgr.cpp"
    "ServerMark.cpp"
    "ServerSoundMgr.cpp"
    "ServerUtilities.cpp"
    "SFXFuncs.cpp"
    "SoundFX.cpp"
    "Sparam.cpp"
    "Spawner.cpp"
    "Speaker.cpp"
    "Sprinkles.cpp"
    "Steam.cpp"
    "Switch.cpp"
    "TeleportPoint.cpp"
    "TranslucentWorldModel.cpp"
    "Trigger.cpp"
    "Video.cpp"
    "VolumeBrush.cpp"
    "VolumeBrushTypes.cpp"
    "Weapon.cpp"
    "WeaponItems.cpp"
    "Weapons.cpp"
    "WorldModelDebris.cpp"
    "WorldProperties.cpp"
    "ZipHook.cpp"
)
source_group("Source Files" FILES ${Source_Files})

set(Source_Files__AI_Source_Files
    "AI.cpp"
    "AIAnimal.cpp"
    "AIAnimalState.cpp"
    "AIAnimalStrategy.cpp"
    "AIButeMgr.cpp"
    "AIDog.cpp"
    "AIDogReactions.cpp"
    "AIGroup.cpp"
    "AIHelicopter.cpp"
    "AIHuman.cpp"
    "AIHumanReactions.cpp"
    "AIHumans.cpp"
    "AIHumanState.cpp"
    "AIHumanStrategy.cpp"
    "AIMovement.cpp"
    "AINode.cpp"
    "AINodeMgr.cpp"
    "AIPath.cpp"
    "AIPathMgr.cpp"
    "AIPoodle.cpp"
    "AIReactions.cpp"
    "AISense.cpp"
    "AIShark.cpp"
    "AISounds.cpp"
    "AIState.cpp"
    "AISteering.cpp"
    "AITarget.cpp"
    "AIUtils.cpp"
    "AIVehicle.cpp"
    "AIVehicleState.cpp"
    "AIVehicleStrategy.cpp"
    "AIVolume.cpp"
    "AIVolumeMgr.cpp"
    "Alarm.h"
)
source_group("Source Files\\AI Source Files" FILES ${Source_Files__AI_Source_Files})

set(Source_Files__Animation_Source_Files
    "../Shared/Animator.cpp"
    "AnimationLex.cpp"
    "AnimationLex.l"
    "AnimationMgr.cpp"
    "AnimationMgrHuman.cpp"
    "AnimationParse.cpp"
    "AnimationParse.y"
    "AnimationParser.cpp"
    "AnimatorAIAnimal.cpp"
    "AnimatorAIVehicle.cpp"
    "AnimatorPlayer.cpp"
)
source_group("Source Files\\Animation Source Files" FILES ${Source_Files__Animation_Source_Files})

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
add_sources_if_exist(${PROJECT_NAME} ${no_group_source_files})
add_sources_if_exist(${PROJECT_NAME} ${Header_Files})
add_sources_if_exist(${PROJECT_NAME} ${Header_Files__AI_Header_Files})
add_sources_if_exist(${PROJECT_NAME} ${Header_Files__Animation_Header_Files})
add_sources_if_exist(${PROJECT_NAME} ${SDK})
add_sources_if_exist(${PROJECT_NAME} ${Source_Files})
add_sources_if_exist(${PROJECT_NAME} ${Source_Files__AI_Source_Files})
add_sources_if_exist(${PROJECT_NAME} ${Source_Files__Animation_Source_Files})

target_precompile_headers(${PROJECT_NAME} PRIVATE
    "$<$<COMPILE_LANGUAGE:CXX>:${CMAKE_CURRENT_SOURCE_DIR}/../Shared/Stdafx.h>"
)

use_props(${PROJECT_NAME} "${CMAKE_CONFIGURATION_TYPES}" "${DEFAULT_CXX_PROPS}")
################################################################################
# Target name
################################################################################
set_target_properties(${PROJECT_NAME} PROPERTIES
    TARGET_NAME_DEBUG        "Object"
    TARGET_NAME_FINALDEBUG   "Object"
    TARGET_NAME_FINALRELEASE "Object"
    TARGET_NAME_RELEASE      "Object"
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
    ARCHIVE_OUTPUT_NAME_DEBUG        "Object"
    ARCHIVE_OUTPUT_NAME_FINALDEBUG   "Object"
    ARCHIVE_OUTPUT_NAME_FINALRELEASE "Object"
    ARCHIVE_OUTPUT_NAME_RELEASE      "Object"
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
        "${CMAKE_CURRENT_SOURCE_DIR}/../../LT2/sdk/inc;"
        "${CMAKE_CURRENT_SOURCE_DIR}/../../LT2/lithshared/incs;"
        "${CMAKE_CURRENT_SOURCE_DIR}/../Shared;"
        "${CMAKE_CURRENT_SOURCE_DIR}/."
    ">"
    "$<$<CONFIG:FinalDebug>:"
        "${CMAKE_CURRENT_SOURCE_DIR}/../../LT2/sdk/inc;"
        "${CMAKE_CURRENT_SOURCE_DIR}/../../LT2/lithshared/incs;"
        "${CMAKE_CURRENT_SOURCE_DIR}/../Shared;"
        "${CMAKE_CURRENT_SOURCE_DIR}/."
    ">"
    "$<$<CONFIG:FinalRelease>:"
        "${CMAKE_CURRENT_SOURCE_DIR}/../../LT2/sdk/inc;"
        "${CMAKE_CURRENT_SOURCE_DIR}/../../LT2/lithshared/incs;"
        "${CMAKE_CURRENT_SOURCE_DIR}/../Shared;"
        "${CMAKE_CURRENT_SOURCE_DIR}/."
    ">"
    "$<$<CONFIG:Release>:"
        "${CMAKE_CURRENT_SOURCE_DIR}/../../LT2/sdk/inc;"
        "${CMAKE_CURRENT_SOURCE_DIR}/../../LT2/lithshared/incs;"
        "${CMAKE_CURRENT_SOURCE_DIR}/../Shared;"
        "${CMAKE_CURRENT_SOURCE_DIR}/."
    ">"
)

################################################################################
# Compile definitions
################################################################################
target_compile_definitions(${PROJECT_NAME} PRIVATE
    "$<$<CONFIG:Debug>:"
        "_DEBUG;"
        "WIN32;"
        "_WINDOWS;"
        "NO_PRAGMA_LIBS"
    ">"
    "$<$<CONFIG:FinalDebug>:"
        "_REZFILE;"
        "_FINAL;"
        "_DEBUG;"
        "WIN32;"
        "_WINDOWS;"
        "NO_PRAGMA_LIBS"
    ">"
    "$<$<CONFIG:FinalRelease>:"
        "_REZFILE;"
        "_FINAL;"
        "NDEBUG;"
        "WIN32;"
        "_WINDOWS;"
        "_NOLFBUILD;"
        "NO_PRAGMA_LIBS"
    ">"
    "$<$<CONFIG:Release>:"
        "NDEBUG;"
        "WIN32;"
        "_WINDOWS;"
        "_NOLFBUILD;"
        "NO_PRAGMA_LIBS;"
        "USE_INTEL_COMPILER"
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
            /W3;
            /ZI
        >
        $<$<CONFIG:FinalDebug>:
            /Gm;
            /Od;
            /Gy-;
            /W3;
            /ZI
        >
        $<$<CONFIG:FinalRelease>:
            /O2;
            /GF;
            /Gy;
            /W3;
            ${DEFAULT_CXX_DEBUG_INFORMATION_FORMAT}
        >
        $<$<CONFIG:Release>:
            /O2;
            /GF;
            /Gy;
            /W3;
            ${DEFAULT_CXX_DEBUG_INFORMATION_FORMAT}
        >
        $<$<CONFIG:Template>:
            ${DEFAULT_CXX_DEBUG_INFORMATION_FORMAT}
        >
        ${DEFAULT_CXX_EXCEPTION_HANDLING}
    )
    string(CONCAT FILE_CL_OPTIONS
        "$<$<CONFIG:Debug>:"
            "/Y-"
        ">"
        "$<$<CONFIG:FinalDebug>:"
            "/Y-"
        ">"
        "$<$<CONFIG:FinalRelease>:"
            "/Y-"
        ">"
        "$<$<CONFIG:Release>:"
            "/Y-"
        ">"
    )
    source_file_compile_options(../../LT2/sdk/inc/ltquatbase.cpp ${FILE_CL_OPTIONS})
    string(CONCAT FILE_CL_OPTIONS
        "$<$<CONFIG:Debug>:"
            "/Y-"
        ">"
        "$<$<CONFIG:FinalDebug>:"
            "/Y-"
        ">"
        "$<$<CONFIG:FinalRelease>:"
            "/Y-"
        ">"
        "$<$<CONFIG:Release>:"
            "/Y-"
        ">"
    )
    source_file_compile_options(AnimationLex.cpp ${FILE_CL_OPTIONS})
    string(CONCAT FILE_CL_OPTIONS
        "$<$<CONFIG:Debug>:"
            "/Y-"
        ">"
        "$<$<CONFIG:FinalDebug>:"
            "/Y-"
        ">"
        "$<$<CONFIG:FinalRelease>:"
            "/Y-"
        ">"
        "$<$<CONFIG:Release>:"
            "/Y-"
        ">"
    )
    source_file_compile_options(AnimationParse.cpp ${FILE_CL_OPTIONS})
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
            /NOLOGO;
            /DEBUG:FULL;
            /SUBSYSTEM:WINDOWS;
            /INCREMENTAL:NO
        >
        $<$<CONFIG:Release>:
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
    COMMAND        $<CONFIG:Debug> copy debug\\object.lto $ENV{NOLF_BUILD_DIR}
    COMMAND   $<CONFIG:FinalDebug> copy Final_Debug\\object.lto $ENV{NOLF_BUILD_DIR}
    COMMAND $<CONFIG:FinalRelease> copy Final_Release\\object.lto $ENV{NOLF_BUILD_DIR}
    COMMAND      $<CONFIG:Release> copy release\\object.lto $ENV{NOLF_BUILD_DIR}
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

