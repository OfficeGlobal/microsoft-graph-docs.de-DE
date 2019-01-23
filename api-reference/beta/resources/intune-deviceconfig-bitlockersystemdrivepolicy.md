---
title: Ressourcentyp bitLockerSystemDrivePolicy
description: BitLocker-Verschlüsselung Basis Richtlinien.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9b63d075538508941d012df1e44f7cb563fed20d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425708"
---
# <a name="bitlockersystemdrivepolicy-resource-type"></a><span data-ttu-id="cfe5c-103">Ressourcentyp bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="cfe5c-103">bitLockerSystemDrivePolicy resource type</span></span>

> <span data-ttu-id="cfe5c-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="cfe5c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cfe5c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cfe5c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cfe5c-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cfe5c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cfe5c-107">BitLocker-Verschlüsselung Basis Richtlinien.</span><span class="sxs-lookup"><span data-stu-id="cfe5c-107">BitLocker Encryption Base Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="cfe5c-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="cfe5c-108">Properties</span></span>
|<span data-ttu-id="cfe5c-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cfe5c-109">Property</span></span>|<span data-ttu-id="cfe5c-110">Typ</span><span class="sxs-lookup"><span data-stu-id="cfe5c-110">Type</span></span>|<span data-ttu-id="cfe5c-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cfe5c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfe5c-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="cfe5c-112">encryptionMethod</span></span>|[<span data-ttu-id="cfe5c-113">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="cfe5c-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="cfe5c-114">Wählen Sie die Verschlüsselungsmethode für Betriebssystemlaufwerke.</span><span class="sxs-lookup"><span data-stu-id="cfe5c-114">Select the encryption method for operating system drives.</span></span> <span data-ttu-id="cfe5c-115">Mögliche Werte: sind `aesCbc128`, `aesCbc256`, `xtsAes128` und `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="cfe5c-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="cfe5c-116">startupAuthenticationRequired</span><span class="sxs-lookup"><span data-stu-id="cfe5c-116">startupAuthenticationRequired</span></span>|<span data-ttu-id="cfe5c-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="cfe5c-117">Boolean</span></span>|<span data-ttu-id="cfe5c-118">Erfordert zusätzliche Authentifizierung beim Start.</span><span class="sxs-lookup"><span data-stu-id="cfe5c-118">Require additional authentication at startup.</span></span>|
|<span data-ttu-id="cfe5c-119">startupAuthenticationBlockWithoutTpmChip</span><span class="sxs-lookup"><span data-stu-id="cfe5c-119">startupAuthenticationBlockWithoutTpmChip</span></span>|<span data-ttu-id="cfe5c-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="cfe5c-120">Boolean</span></span>|<span data-ttu-id="cfe5c-121">Gibt an, ob BitLocker ohne kompatibles TPM zulassen (erfordert ein Kennwort oder einen Startschlüssel auf einem USB flash-Laufwerk).</span><span class="sxs-lookup"><span data-stu-id="cfe5c-121">Indicates whether to allow BitLocker without a compatible TPM (requires a password or a startup key on a USB flash drive).</span></span>|
|<span data-ttu-id="cfe5c-122">startupAuthenticationTpmUsage</span><span class="sxs-lookup"><span data-stu-id="cfe5c-122">startupAuthenticationTpmUsage</span></span>|[<span data-ttu-id="cfe5c-123">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="cfe5c-123">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="cfe5c-124">Gibt an, ob TPM Start zulässig/erforderlich/nicht zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="cfe5c-124">Indicates if TPM startup is allowed/required/disallowed.</span></span> <span data-ttu-id="cfe5c-125">Mögliche Werte sind: `blocked`, `required` und `allowed`.</span><span class="sxs-lookup"><span data-stu-id="cfe5c-125">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="cfe5c-126">startupAuthenticationTpmPinUsage</span><span class="sxs-lookup"><span data-stu-id="cfe5c-126">startupAuthenticationTpmPinUsage</span></span>|[<span data-ttu-id="cfe5c-127">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="cfe5c-127">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="cfe5c-128">Gibt an, ob TPM Startup Pin zulässig/erforderlich/nicht zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="cfe5c-128">Indicates if TPM startup pin is allowed/required/disallowed.</span></span> <span data-ttu-id="cfe5c-129">Mögliche Werte sind: `blocked`, `required` und `allowed`.</span><span class="sxs-lookup"><span data-stu-id="cfe5c-129">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="cfe5c-130">startupAuthenticationTpmKeyUsage</span><span class="sxs-lookup"><span data-stu-id="cfe5c-130">startupAuthenticationTpmKeyUsage</span></span>|[<span data-ttu-id="cfe5c-131">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="cfe5c-131">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="cfe5c-132">Gibt an, ob TPM zum Starten des Schlüssel zulässig/erforderlich/nicht zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="cfe5c-132">Indicates if TPM startup key is allowed/required/disallowed.</span></span> <span data-ttu-id="cfe5c-133">Mögliche Werte sind: `blocked`, `required` und `allowed`.</span><span class="sxs-lookup"><span data-stu-id="cfe5c-133">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="cfe5c-134">startupAuthenticationTpmPinAndKeyUsage</span><span class="sxs-lookup"><span data-stu-id="cfe5c-134">startupAuthenticationTpmPinAndKeyUsage</span></span>|[<span data-ttu-id="cfe5c-135">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="cfe5c-135">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="cfe5c-136">Gibt an, ob TPM Start anheften und Schlüssel sind zulässig/erforderlich/nicht zulässig.</span><span class="sxs-lookup"><span data-stu-id="cfe5c-136">Indicates if TPM startup pin key and key are allowed/required/disallowed.</span></span> <span data-ttu-id="cfe5c-137">Mögliche Werte sind: `blocked`, `required` und `allowed`.</span><span class="sxs-lookup"><span data-stu-id="cfe5c-137">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="cfe5c-138">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="cfe5c-138">minimumPinLength</span></span>|<span data-ttu-id="cfe5c-139">Int32</span><span class="sxs-lookup"><span data-stu-id="cfe5c-139">Int32</span></span>|<span data-ttu-id="cfe5c-140">Gibt die minimale Länge des Startup Pin an.</span><span class="sxs-lookup"><span data-stu-id="cfe5c-140">Indicates the minimum length of startup pin.</span></span> <span data-ttu-id="cfe5c-141">Gültige Werte 4 bis 20</span><span class="sxs-lookup"><span data-stu-id="cfe5c-141">Valid values 4 to 20</span></span>|
|<span data-ttu-id="cfe5c-142">recoveryOptions</span><span class="sxs-lookup"><span data-stu-id="cfe5c-142">recoveryOptions</span></span>|[<span data-ttu-id="cfe5c-143">bitLockerRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="cfe5c-143">bitLockerRecoveryOptions</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|<span data-ttu-id="cfe5c-144">BitLocker verschlüsselt Betriebssystemlaufwerke in Abwesenheit der erforderlichen Startup Schlüsselinformationen wiederherstellen können.</span><span class="sxs-lookup"><span data-stu-id="cfe5c-144">Allows to recover BitLocker encrypted operating system drives in the absence of the required startup key information.</span></span> <span data-ttu-id="cfe5c-145">Diese Einstellung wird angewendet, wenn Sie BitLocker aktivieren.</span><span class="sxs-lookup"><span data-stu-id="cfe5c-145">This policy setting is applied when you turn on BitLocker.</span></span>|
|<span data-ttu-id="cfe5c-146">prebootRecoveryEnableMessageAndUrl</span><span class="sxs-lookup"><span data-stu-id="cfe5c-146">prebootRecoveryEnableMessageAndUrl</span></span>|<span data-ttu-id="cfe5c-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="cfe5c-147">Boolean</span></span>|<span data-ttu-id="cfe5c-148">Aktivieren Sie vor dem Start Recovery Nachrichten- und Url.</span><span class="sxs-lookup"><span data-stu-id="cfe5c-148">Enable pre-boot recovery message and Url.</span></span> <span data-ttu-id="cfe5c-149">Wenn RequireStartupAuthentication auf false festgelegt ist, wirkt sich dieser Wert nicht.</span><span class="sxs-lookup"><span data-stu-id="cfe5c-149">If requireStartupAuthentication is false, this value does not affect.</span></span>|
|<span data-ttu-id="cfe5c-150">prebootRecoveryMessage</span><span class="sxs-lookup"><span data-stu-id="cfe5c-150">prebootRecoveryMessage</span></span>|<span data-ttu-id="cfe5c-151">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cfe5c-151">String</span></span>|<span data-ttu-id="cfe5c-152">Definiert eine benutzerdefinierte Wiederherstellung Nachricht.</span><span class="sxs-lookup"><span data-stu-id="cfe5c-152">Defines a custom recovery message.</span></span>|
|<span data-ttu-id="cfe5c-153">prebootRecoveryUrl</span><span class="sxs-lookup"><span data-stu-id="cfe5c-153">prebootRecoveryUrl</span></span>|<span data-ttu-id="cfe5c-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cfe5c-154">String</span></span>|<span data-ttu-id="cfe5c-155">Definiert eine benutzerdefinierte Wiederherstellung-URL.</span><span class="sxs-lookup"><span data-stu-id="cfe5c-155">Defines a custom recovery URL.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cfe5c-156">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="cfe5c-156">Relationships</span></span>
<span data-ttu-id="cfe5c-157">Keine</span><span class="sxs-lookup"><span data-stu-id="cfe5c-157">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cfe5c-158">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="cfe5c-158">JSON Representation</span></span>
<span data-ttu-id="cfe5c-159">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="cfe5c-159">Here is a JSON representation of the resource.</span></span>
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




