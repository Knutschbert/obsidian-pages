---
title: AHorse
type: class
aliases: AHorse
share: true

---

# AHorse





Inherits from [ASiegeEngine](/docs/SDK/Source/Classes/classASiegeEngine.md), [ATBLCharacterBase](/docs/SDK/Source/Classes/classATBLCharacterBase.md), [IReplicatedSubobjectInterface](/docs/SDK/Source/Classes/classIReplicatedSubobjectInterface.md), [IDamagerInterface](/docs/SDK/Source/Classes/classIDamagerInterface.md), ACharacter, [ISignificanceInterface](/docs/SDK/Source/Classes/classISignificanceInterface.md)

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[[AHorse]]**() |
| void | **[[EventUsePressed]]**(APawn * InPawn, [UInteractableComponent](/docs/SDK/Source/Classes/classUInteractableComponent.md) * InInteractable) |
| void | **[[ForceRun]]**(float Time) |
| FVector | **[[GetCurveValueBySpeed]]**(UCurveVector * Curve, float RelativeSpeed) |
| FName | **[[GetHorseCollisionProfile]]**() |
| virtual void | **[[GetLifetimeReplicatedProps]]**(TArray< FLifetimeProperty > & OutLifetimeProps) const override |
| TArray< UPrimitiveComponent * > | **[[GetPushingCollision]]**() |
| float | **[[GetRelativeSpeed]]**(AActor * OtherActor) |
| ECollisionResponse | **[[GetRiderToWorldCollision]]**() |
| FVector | **[[GetThirdPersonCameraAttachPoint]]**() |
| TArray< UPrimitiveComponent * > | **[[GetWorldCollisionBack]]**() |
| TArray< UPrimitiveComponent * > | **[[GetWorldCollisionFront]]**() |
| void | **[[GetWorldCollisionLegs]]**(UCapsuleComponent *& FrontLegs, UCapsuleComponent *& BackLegs) |
| UCapsuleComponent * | **[[GetWorldCollisionRider]]**() |
| bool | **[[HasSpeedForAttack]]**(FName AttackName) |
| void | **[[HorseToCharacterImpact]]**([ATBLCharacter](/docs/SDK/Source/Classes/classATBLCharacter.md) * TargetCharacter, EHorseImpactLocation ImpactLocation, EHorseToCharacterImpactType ImpactType, FName ImpactCombatState, float ImpactSpeed) |
| void | **[[HorseToHorseImpact]]**([AHorse](/docs/SDK/Source/Classes/classAHorse.md) * TargetHorse, EHorseImpactLocation ImpactLocation, EHorseToHorseImpactType ImpactType, FName ImpactCombatState, float ImpactSpeed) |
| void | **[[HorseToWorldImpact]]**(FHitResult Hit, EHorseImpactLocation ImpactLocation, EHorseToWorldImpactType ImpactType, FName ImpactCombatState, float ImpactSpeed) |
| void | **[[Horse_ClientAdjustPosition]]**(float Timestamp, FVector NewLoc, FVector NewVel, UPrimitiveComponent * NewBase, FName NewBaseBoneName, bool bHasBase, bool bBaseRelativePosition, uint8 ServerMovementMode, const [FHorseMovementCorrection](/docs/SDK/Source/Classes/structFHorseMovementCorrection.md) & HorseCorrection) |
| void | **[[InitiateKick]]**(FName AttackName) |
| bool | **[[IsDead]]**() const |
| bool | **[[IsExhausted]]**() const |
| void | **[[KickNoDriver]]**() |
| void | **[[KnockRiderOffHorse]]**() |
| void | **[[MaintainSpeedOnImpact]]**() |
| void | **[[NetMulticastFastSharedReplication]]**(const [FFastSharedProperties_Horse](/docs/SDK/Source/Classes/structFFastSharedProperties__Horse.md) & Properties) |
| void | **[[OnHorseDamaged]]**(const [FDamageTakenEvent](/docs/SDK/Source/Classes/structFDamageTakenEvent.md) & Event) |
| void | **[[OnKilled]]**(const [FDeathDamageTakenEvent](/docs/SDK/Source/Classes/structFDeathDamageTakenEvent.md) & DamageEvent) |
| void | **[[OnProcessPlayerInput]]**() |
| void | **[[PostHorseFxEvent]]**(FName EventName, float EventScale, const TArray< FName > & EventTags) |
| void | **[[RiderToWorldImpact]]**(FHitResult Hit) |
| void | **[[ServerHorseMove]]**(float Timestamp, FVector_NetQuantize10 InAccel, FVector ClientLoc, uint8 CompressedMoveFlags, uint32 View, UPrimitiveComponent * ClientMovementBase, uint8 ClientMovementMode, float InRotationYaw, int16 ForwardSpeed) |
| void | **[[ServerHorseMoveDual]]**(float TimeStamp0, FVector_NetQuantize10 InAccel0, uint8 PendingFlags, uint32 View0, float Timestamp, FVector_NetQuantize10 InAccel, FVector ClientLoc, uint8 NewFlags, uint32 View, UPrimitiveComponent * ClientMovementBase, uint8 ClientMovementMode, float InRotationYaw, int16 ForwardSpeed) |
| void | **[[ServerHorseMoveDualHybridRootMotion]]**(float TimeStamp0, FVector_NetQuantize10 InAccel0, uint8 PendingFlags, uint32 View0, float Timestamp, FVector_NetQuantize10 InAccel, FVector ClientLoc, uint8 NewFlags, uint32 View, UPrimitiveComponent * ClientMovementBase, uint8 ClientMovementMode, float InRotationYaw, int16 ForwardSpeed) |
| bool | **[[ShouldPushBackOnTurnAgainstWall]]**() |
| bool | **[[TrySlowdownForKick]]**(FName AttackName) |

## Protected Functions

|                | Name           |
| -------------- | -------------- |
| void | **[[BroadcastPlayDismountAnimation]]**(FName AnimationName) |
| void | **[[BroadcastPostHorseFxEvent]]**(FName EventName, float EventScale, const TArray< FName > & EventTags) |
| void | **[[BroadcastRandomSeed]]**(int32 Seed) |
| void | **[[BroadcastSetFaction]]**(EFaction Faction) |
| void | **[[OnCinematicControlAllowed]]**([ATBLCharacter](/docs/SDK/Source/Classes/classATBLCharacter.md) * Character) |
| void | **[[OnCinematicControlRestricted]]**([ATBLCharacter](/docs/SDK/Source/Classes/classATBLCharacter.md) * Character) |
| void | **[[OnCombatStateChanged]]**(AActor * Actor, FName PreviousState, FName NewState, const [FAttackInfo](/docs/SDK/Source/Classes/structFAttackInfo.md) & EventAttackInfo, [UCombatState](/docs/SDK/Source/Classes/classUCombatState.md) * CombatState) |
| void | **[[OnDismountSetAttached]]**(bool bAttached) |
| void | **[[OnPlayerMeshChanged]]**(USkeletalMeshComponent * OldMesh, USkeletalMeshComponent * NewMesh) |
| void | **[[OnRiderStartAttack]]**() |
| void | **[[StartInterpToMountLocation]]**() |
| void | **[[WantsToGallop]]**(bool bWantsToGallop) |

## Public Attributes

|                | Name           |
| -------------- | -------------- |
| FVector | **[[BackLegsTargetLocation]]**  |
| USceneComponent * | **[[CollisionRoot]]**  |
| [UCombatStateComponent](/docs/SDK/Source/Classes/classUCombatStateComponent.md) * | **[[CombatStateComponent]]**  |
| [UCombatStateQueue](/docs/SDK/Source/Classes/classUCombatStateQueue.md) * | **[[CombatStateQueue]]**  |
| TSubclassOf< [UCombatStateSet](/docs/SDK/Source/Classes/classUCombatStateSet.md) > | **[[CombatStateSet]]**  |
| [UCombatStateSynchronization](/docs/SDK/Source/Classes/classUCombatStateSynchronization.md) * | **[[CombatStateSynchronization]]**  |
| [UConditionsComponent](/docs/SDK/Source/Classes/classUConditionsComponent.md) * | **[[ConditionsComponent]]**  |
| TArray< [FTimeStampedDamageTakenEvent](/docs/SDK/Source/Classes/structFTimeStampedDamageTakenEvent.md) > | **[[DamageTakenEvents]]**  |
| float | **[[ExpireTime]]**  |
| FTimerHandle | **[[ExpireTimerHandle]]**  |
| float | **[[FXImpactSpeedThreshold]]**  |
| FVector | **[[FrontLegsTargetLocation]]**  |
| [UHorseMovement](/docs/SDK/Source/Classes/classUHorseMovement.md) * | **[[HorseMovement]]**  |
| [UInteractableComponent](/docs/SDK/Source/Classes/classUInteractableComponent.md) * | **[[Interactable]]**  |
| float | **[[KnockdownBlendOutTime]]**  |
| float | **[[LastClientForwardSpeed]]**  |
| FName | **[[LastClientMovementState]]**  |
| float | **[[LastClientRotationYaw]]**  |
| [UMovementModifierComponent](/docs/SDK/Source/Classes/classUMovementModifierComponent.md) * | **[[MovementModifiers]]**  |
| FOnHorseBump | **[[OnHorseBump]]**  |
| FHorseFxEvent | **[[OnHorseFxEvent]]**  |
| FOnHorseToCharacterImpact | **[[OnHorseToCharacterImpact]]**  |
| FOnHorseToHorseImpact | **[[OnHorseToHorseImpact]]**  |
| FOnHorseToWorldImpact | **[[OnHorseToWorldImpact]]**  |
| FHorseOnInterpToMountLocation | **[[OnInterpToMountLocation]]**  |
| FOnKickNoDriver | **[[OnKickNoDriver]]**  |
| FLanceChargeEnabled | **[[OnLanceChargeEnabled]]**  |
| FLanceChargeFailed | **[[OnLanceChargeFailed]]**  |
| FHorsePlayLandedAnimation | **[[OnLandedAnimation]]**  |
| FOnHorseRootMotionChanged | **[[OnRootMotionChanged]]**  |
| FOnHorseSpeedRequirementFailed | **[[OnSpeedRequirementFailed]]**  |
| FOnHorseStartAttack | **[[OnStartAttack]]**  |
| FHorsePlayDismountAnimation | **[[PlayDismountAnimation]]**  |
| FHorsePlayMountAnimation | **[[PlayMountAnimation]]**  |
| float | **[[PushSpeed]]**  |
| TArray< UPrimitiveComponent * > | **[[PushingCollision]]**  |
| [UPushingComponent](/docs/SDK/Source/Classes/classUPushingComponent.md) * | **[[PushingComponent]]**  |
| int32 | **[[PushingPriority]]**  |
| FVector | **[[RelativeLocation_BackLegs]]**  |
| FVector | **[[RelativeLocation_FrontLegs]]**  |
| uint8 | **[[ReplicatedServerFrame]]**  |
| float | **[[RotationLimit]]**  |
| [UTeamOwnershipComponent](/docs/SDK/Source/Classes/classUTeamOwnershipComponent.md) * | **[[TeamOwnershipComponent]]**  |
| float | **[[ThirdPersonCameraOffsetZ]]**  |
| [FThirdPersonCameraParams](/docs/SDK/Source/Classes/structFThirdPersonCameraParams.md) | **[[ThirdPersonCameraParams]]**  |
| TArray< UPrimitiveComponent * > | **[[WorldCollision_Back]]**  |
| UCapsuleComponent * | **[[WorldCollision_BackLegs]]**  |
| TArray< UPrimitiveComponent * > | **[[WorldCollision_Both]]**  |
| TArray< UPrimitiveComponent * > | **[[WorldCollision_Front]]**  |
| UCapsuleComponent * | **[[WorldCollision_FrontLegs]]**  |
| UCapsuleComponent * | **[[WorldCollision_Rider]]**  |
| bool | **[[bEmergencyBrakeExhausted]]**  |
| bool | **[[bGallopExhausted]]**  |
| bool | **[[bRiderUseControllerRotationYaw]]**  |
| bool | **[[bSpawnOnHorse]]**  |

## Protected Attributes

|                | Name           |
| -------------- | -------------- |
| UDataTable * | **[[AbilitiesDataTable]]**  |
| bool | **[[HasAccelerateVoBeenPlayed]]**  |
| int32 | **[[HorizLockId]]**  |
| [FHorseAiming](/docs/SDK/Source/Classes/structFHorseAiming.md) | **[[HorseAiming]]**  |
| FName | **[[HorseCollisionPreset]]**  |
| bool | **[[IsGalloping]]**  |
| [FDataTableRowSelection](/docs/SDK/Source/Classes/structFDataTableRowSelection.md) | **[[LanceCharge]]**  |
| [UAbilitySpec](/docs/SDK/Source/Classes/classUAbilitySpec.md) * | **[[LanceChargeSpec]]**  |
| FVector | **[[LastDriverRootLocation]]**  |
| float | **[[LastHorseMountTime]]**  |
| EFaction | **[[LastMountedFaction]]**  |
| FName | **[[MountDirection]]**  |
| bool | **[[PreviousIsPlayingRootMotion]]**  |
| FTimerHandle | **[[QueuedAccelerateVoTimerHandle]]**  |
| FTimerHandle | **[[QueuedDeccelerateVoTimerHandle]]**  |
| bool | **[[bHorseGallopVoIgnoredOnce]]**  |
| bool | **[[bIsDead]]**  |
| bool | **[[bLanceChargeEnabled]]**  |

-------------------------------

Updated on 2023-07-04 at 02:30:58 +0200