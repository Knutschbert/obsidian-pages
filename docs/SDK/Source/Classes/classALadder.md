---
title: ALadder
type: class
aliases: ALadder
share: true

---

# ALadder





Inherits from [ATBLActor](/docs/SDK/Source/Classes/classATBLActor.md), INavRelevantInterface, [IReplicatedSubobjectInterface](/docs/SDK/Source/Classes/classIReplicatedSubobjectInterface.md)

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[[ALadder]]**() |
| bool | **[[CanMountLadder]]**(APawn * Pawn) |
| void | **[[DisableLadder]]**() |
| void | **[[EnableLadder]]**() |
| virtual void | **[[GetLifetimeReplicatedProps]]**(TArray< FLifetimeProperty > & OutLifetimeProps) const override |
| bool | **[[IsLadderEnabled]]**() const |
| bool | **[[WantsDismountOnThisEnd]]**(bool bTop) const |

## Protected Functions

|                | Name           |
| -------------- | -------------- |
| void | **[[BeginJumpOverlap]]**(UPrimitiveComponent * OverlappedComponent, AActor * Other, UPrimitiveComponent * OtherComp, int32 OtherBodyIndex, bool bFromSweep, const FHitResult & OverlapInfo) |
| void | **[[EndJumpOverlap]]**(UPrimitiveComponent * OverlappedComponent, AActor * Other, UPrimitiveComponent * OtherComp, int32 OtherBodyIndex) |
| void | **[[EventMountLadder]]**(APawn * Pawn) |
| void | **[[MountLadder]]**(APawn * Pawn, bool bIsJumping) |
| void | **[[OnMovementChangedInJumpCollider]]**(FName MovementState) |
| void | **[[OnRep_LadderEnabled]]**() |
| void | **[[OnUseSyncFailed]]**(APawn * Pawn, [UInteractableComponent](/docs/SDK/Source/Classes/classUInteractableComponent.md) * InteractableComponent) |
| void | **[[UsePressed]]**(APawn * Pawn, [UInteractableComponent](/docs/SDK/Source/Classes/classUInteractableComponent.md) * InteractableComponent) |

## Public Attributes

|                | Name           |
| -------------- | -------------- |
| [FBlendParams](/docs/SDK/Source/Classes/structFBlendParams.md) | **[[LadderDismountBlend]]**  |
| [FBlendParams](/docs/SDK/Source/Classes/structFBlendParams.md) | **[[LadderMountBlend]]**  |
| FLadderStateChangedSignature | **[[OnLadderStateChanged]]**  |

## Protected Attributes

|                | Name           |
| -------------- | -------------- |
| FVector | **[[AttachOffset]]**  |
| FRotator | **[[AttachRotation]]**  |
| FVector | **[[DismountPointBottom]]**  |
| FVector | **[[DismountPointTop]]**  |
| [UInteractableComponent](/docs/SDK/Source/Classes/classUInteractableComponent.md) * | **[[Interactable]]**  |
| UBoxComponent * | **[[JumpCollider]]**  |
| TArray< [ATBLCharacter](/docs/SDK/Source/Classes/classATBLCharacter.md) * > | **[[JumpOverlappingCharacters]]**  |
| FVector | **[[LadderBottom]]**  |
| float | **[[LadderHeight]]**  |
| UAnimMontage * | **[[LadderMontage]]**  |
| FVector | **[[LadderTop]]**  |
| float | **[[MaxMountAngle]]**  |
| float | **[[MaxMountDist]]**  |
| FVector | **[[MountPointBottom]]**  |
| FVector | **[[MountPointTop]]**  |
| float | **[[MoveDownAngle]]**  |
| TArray< APawn * > | **[[PawnList]]**  |
| APawn * | **[[PawnToIgnoreJump]]**  |
| FTimerHandle | **[[PawnToIgnoreJumpHandle]]**  |
| USceneComponent * | **[[SceneComponent]]**  |
| USceneComponent * | **[[SmartLinkBottom]]**  |
| UNavLinkCustomComponent * | **[[SmartLinkComp]]**  |
| TEnumAsByte< ENavLinkDirection::Type > | **[[SmartLinkDirection]]**  |
| USceneComponent * | **[[SmartLinkTop]]**  |
| float | **[[TurnLimit]]**  |
| bool | **[[bCanDismountOffBottom]]**  |
| bool | **[[bCanDismountOffTop]]**  |
| [FReplicated_Bool](/docs/SDK/Source/Classes/structFReplicated__Bool.md) | **[[bLadderEnabled]]**  |
| bool | **[[bSmartLinkIsRelevant]]**  |
| bool | **[[bStartEnabled]]**  |

-------------------------------

Updated on 2023-07-04 at 02:30:58 +0200