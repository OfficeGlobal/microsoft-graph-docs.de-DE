---
title: Ressourcentyp bitLockerSystemDrivePolicy
description: BitLocker-Verschlüsselung Basis Richtlinien.
author: tfitzmac
ms.openlocfilehash: ba1199970099bb841fc363a747abb5b8dcac2ec1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332284"
---
# <a name="bitlockersystemdrivepolicy-resource-type"></a><span data-ttu-id="43148-103">Ressourcentyp bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="43148-103">bitLockerSystemDrivePolicy resource type</span></span>

> <span data-ttu-id="43148-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="43148-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="43148-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="43148-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="43148-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="43148-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="43148-107">BitLocker-Verschlüsselung Basis Richtlinien.</span><span class="sxs-lookup"><span data-stu-id="43148-107">BitLocker Encryption Base Policies.</span></span>
## <a name="properties"></a><span data-ttu-id="43148-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="43148-108">Properties</span></span>
|<span data-ttu-id="43148-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="43148-109">Property</span></span>|<span data-ttu-id="43148-110">Typ</span><span class="sxs-lookup"><span data-stu-id="43148-110">Type</span></span>|<span data-ttu-id="43148-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="43148-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43148-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="43148-112">encryptionMethod</span></span>|[<span data-ttu-id="43148-113">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="43148-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="43148-114">Wählen Sie die Verschlüsselungsmethode für Betriebssystemlaufwerke.</span><span class="sxs-lookup"><span data-stu-id="43148-114">Select the encryption method for operating system drives.</span></span> <span data-ttu-id="43148-115">Mögliche Werte: sind `aesCbc128`, `aesCbc256`, `xtsAes128` und `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="43148-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="43148-116">startupAuthenticationRequired</span><span class="sxs-lookup"><span data-stu-id="43148-116">startupAuthenticationRequired</span></span>|<span data-ttu-id="43148-117">Boolesch</span><span class="sxs-lookup"><span data-stu-id="43148-117">Boolean</span></span>|<span data-ttu-id="43148-118">Erfordert zusätzliche Authentifizierung beim Start.</span><span class="sxs-lookup"><span data-stu-id="43148-118">Require additional authentication at startup.</span></span>|
|<span data-ttu-id="43148-119">startupAuthenticationBlockWithoutTpmChip</span><span class="sxs-lookup"><span data-stu-id="43148-119">startupAuthenticationBlockWithoutTpmChip</span></span>|<span data-ttu-id="43148-120">Boolesch</span><span class="sxs-lookup"><span data-stu-id="43148-120">Boolean</span></span>|<span data-ttu-id="43148-121">Gibt an, ob BitLocker ohne kompatibles TPM zulassen (erfordert ein Kennwort oder einen Startschlüssel auf einem USB flash-Laufwerk).</span><span class="sxs-lookup"><span data-stu-id="43148-121">Indicates whether to allow BitLocker without a compatible TPM (requires a password or a startup key on a USB flash drive).</span></span>|
|<span data-ttu-id="43148-122">startupAuthenticationTpmUsage</span><span class="sxs-lookup"><span data-stu-id="43148-122">startupAuthenticationTpmUsage</span></span>|[<span data-ttu-id="43148-123">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="43148-123">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="43148-124">Gibt an, ob TPM Start zulässig/erforderlich/nicht zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="43148-124">Indicates if TPM startup is allowed/required/disallowed.</span></span> <span data-ttu-id="43148-125">Mögliche Werte sind: `blocked`, `required` und `allowed`.</span><span class="sxs-lookup"><span data-stu-id="43148-125">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="43148-126">startupAuthenticationTpmPinUsage</span><span class="sxs-lookup"><span data-stu-id="43148-126">startupAuthenticationTpmPinUsage</span></span>|[<span data-ttu-id="43148-127">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="43148-127">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="43148-128">Gibt an, ob TPM Startup Pin zulässig/erforderlich/nicht zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="43148-128">Indicates if TPM startup pin is allowed/required/disallowed.</span></span> <span data-ttu-id="43148-129">Mögliche Werte sind: `blocked`, `required` und `allowed`.</span><span class="sxs-lookup"><span data-stu-id="43148-129">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="43148-130">startupAuthenticationTpmKeyUsage</span><span class="sxs-lookup"><span data-stu-id="43148-130">startupAuthenticationTpmKeyUsage</span></span>|[<span data-ttu-id="43148-131">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="43148-131">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="43148-132">Gibt an, ob TPM zum Starten des Schlüssel zulässig/erforderlich/nicht zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="43148-132">Indicates if TPM startup key is allowed/required/disallowed.</span></span> <span data-ttu-id="43148-133">Mögliche Werte sind: `blocked`, `required` und `allowed`.</span><span class="sxs-lookup"><span data-stu-id="43148-133">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="43148-134">startupAuthenticationTpmPinAndKeyUsage</span><span class="sxs-lookup"><span data-stu-id="43148-134">startupAuthenticationTpmPinAndKeyUsage</span></span>|[<span data-ttu-id="43148-135">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="43148-135">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="43148-136">Gibt an, ob TPM Start anheften und Schlüssel sind zulässig/erforderlich/nicht zulässig.</span><span class="sxs-lookup"><span data-stu-id="43148-136">Indicates if TPM startup pin key and key are allowed/required/disallowed.</span></span> <span data-ttu-id="43148-137">Mögliche Werte sind: `blocked`, `required` und `allowed`.</span><span class="sxs-lookup"><span data-stu-id="43148-137">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="43148-138">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="43148-138">minimumPinLength</span></span>|<span data-ttu-id="43148-139">Int32</span><span class="sxs-lookup"><span data-stu-id="43148-139">Int32</span></span>|<span data-ttu-id="43148-140">Gibt die minimale Länge des Startup Pin an.</span><span class="sxs-lookup"><span data-stu-id="43148-140">Indicates the minimum length of startup pin.</span></span> <span data-ttu-id="43148-141">Gültige Werte 4 bis 20</span><span class="sxs-lookup"><span data-stu-id="43148-141">Valid values 4 to 20</span></span>|
|<span data-ttu-id="43148-142">recoveryOptions</span><span class="sxs-lookup"><span data-stu-id="43148-142">recoveryOptions</span></span>|[<span data-ttu-id="43148-143">bitLockerRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="43148-143">bitLockerRecoveryOptions</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|<span data-ttu-id="43148-144">BitLocker verschlüsselt Betriebssystemlaufwerke in Abwesenheit der erforderlichen Startup Schlüsselinformationen wiederherstellen können.</span><span class="sxs-lookup"><span data-stu-id="43148-144">Allows to recover BitLocker encrypted operating system drives in the absence of the required startup key information.</span></span> <span data-ttu-id="43148-145">Diese Einstellung wird angewendet, wenn Sie BitLocker aktivieren.</span><span class="sxs-lookup"><span data-stu-id="43148-145">This policy setting is applied when you turn on BitLocker.</span></span>|
|<span data-ttu-id="43148-146">prebootRecoveryEnableMessageAndUrl</span><span class="sxs-lookup"><span data-stu-id="43148-146">prebootRecoveryEnableMessageAndUrl</span></span>|<span data-ttu-id="43148-147">Boolesch</span><span class="sxs-lookup"><span data-stu-id="43148-147">Boolean</span></span>|<span data-ttu-id="43148-148">Aktivieren Sie vor dem Start Recovery Nachrichten- und Url.</span><span class="sxs-lookup"><span data-stu-id="43148-148">Enable pre-boot recovery message and Url.</span></span> <span data-ttu-id="43148-149">Wenn RequireStartupAuthentication auf false festgelegt ist, wirkt sich dieser Wert nicht.</span><span class="sxs-lookup"><span data-stu-id="43148-149">If requireStartupAuthentication is false, this value does not affect.</span></span>|
|<span data-ttu-id="43148-150">prebootRecoveryMessage</span><span class="sxs-lookup"><span data-stu-id="43148-150">prebootRecoveryMessage</span></span>|<span data-ttu-id="43148-151">String</span><span class="sxs-lookup"><span data-stu-id="43148-151">String</span></span>|<span data-ttu-id="43148-152">Definiert eine benutzerdefinierte Wiederherstellung Nachricht.</span><span class="sxs-lookup"><span data-stu-id="43148-152">Defines a custom recovery message.</span></span>|
|<span data-ttu-id="43148-153">prebootRecoveryUrl</span><span class="sxs-lookup"><span data-stu-id="43148-153">prebootRecoveryUrl</span></span>|<span data-ttu-id="43148-154">String</span><span class="sxs-lookup"><span data-stu-id="43148-154">String</span></span>|<span data-ttu-id="43148-155">Definiert eine benutzerdefinierte Wiederherstellung-URL.</span><span class="sxs-lookup"><span data-stu-id="43148-155">Defines a custom recovery URL.</span></span>|

## <a name="relationships"></a><span data-ttu-id="43148-156">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="43148-156">Relationships</span></span>
<span data-ttu-id="43148-157">Keine</span><span class="sxs-lookup"><span data-stu-id="43148-157">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="43148-158">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="43148-158">JSON Representation</span></span>
<span data-ttu-id="43148-159">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="43148-159">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerSystemDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerSystemDrivePolicy",
  "encryptionMethod": "String",
  "startupAuthenticationRequired": true,
  "startupAuthenticationBlockWithoutTpmChip": true,
  "startupAuthenticationTpmUsage": "String",
  "startupAuthenticationTpmPinUsage": "String",
  "startupAuthenticationTpmKeyUsage": "String",
  "startupAuthenticationTpmPinAndKeyUsage": "String",
  "minimumPinLength": 1024,
  "recoveryOptions": {
    "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
    "blockDataRecoveryAgent": true,
    "recoveryPasswordUsage": "String",
    "recoveryKeyUsage": "String",
    "hideRecoveryOptions": true,
    "enableRecoveryInformationSaveToStore": true,
    "recoveryInformationToStore": "String",
    "enableBitLockerAfterRecoveryInformationToStore": true
  },
  "prebootRecoveryEnableMessageAndUrl": true,
  "prebootRecoveryMessage": "String",
  "prebootRecoveryUrl": "String"
}
```





