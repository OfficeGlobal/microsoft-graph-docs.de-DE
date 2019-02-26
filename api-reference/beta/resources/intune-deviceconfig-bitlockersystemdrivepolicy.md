---
title: bitLockerSystemDrivePolicy-Ressourcentyp
description: BitLocker-Verschlüsselungs Basisrichtlinien.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 27b4492dd6df2821cfdeb885d3412536c0d3991c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164890"
---
# <a name="bitlockersystemdrivepolicy-resource-type"></a><span data-ttu-id="aae74-103">bitLockerSystemDrivePolicy-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="aae74-103">bitLockerSystemDrivePolicy resource type</span></span>

> <span data-ttu-id="aae74-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="aae74-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aae74-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="aae74-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aae74-106">BitLocker-Verschlüsselungs Basisrichtlinien.</span><span class="sxs-lookup"><span data-stu-id="aae74-106">BitLocker Encryption Base Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="aae74-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="aae74-107">Properties</span></span>
|<span data-ttu-id="aae74-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="aae74-108">Property</span></span>|<span data-ttu-id="aae74-109">Typ</span><span class="sxs-lookup"><span data-stu-id="aae74-109">Type</span></span>|<span data-ttu-id="aae74-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aae74-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aae74-111">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="aae74-111">encryptionMethod</span></span>|[<span data-ttu-id="aae74-112">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="aae74-112">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="aae74-113">Wählen Sie die Verschlüsselungsmethode für Betriebssystemlaufwerke aus.</span><span class="sxs-lookup"><span data-stu-id="aae74-113">Select the encryption method for operating system drives.</span></span> <span data-ttu-id="aae74-114">Mögliche Werte: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="aae74-114">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="aae74-115">startupAuthenticationRequired</span><span class="sxs-lookup"><span data-stu-id="aae74-115">startupAuthenticationRequired</span></span>|<span data-ttu-id="aae74-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="aae74-116">Boolean</span></span>|<span data-ttu-id="aae74-117">Zusätzliche Authentifizierung beim Start erforderlich.</span><span class="sxs-lookup"><span data-stu-id="aae74-117">Require additional authentication at startup.</span></span>|
|<span data-ttu-id="aae74-118">startupAuthenticationBlockWithoutTpmChip</span><span class="sxs-lookup"><span data-stu-id="aae74-118">startupAuthenticationBlockWithoutTpmChip</span></span>|<span data-ttu-id="aae74-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="aae74-119">Boolean</span></span>|<span data-ttu-id="aae74-120">Gibt an, ob BitLocker ohne kompatibles TPM zugelassen werden soll (erfordert ein Kennwort oder einen Systemstartschlüssel auf einem USB-Flashlaufwerk).</span><span class="sxs-lookup"><span data-stu-id="aae74-120">Indicates whether to allow BitLocker without a compatible TPM (requires a password or a startup key on a USB flash drive).</span></span>|
|<span data-ttu-id="aae74-121">startupAuthenticationTpmUsage</span><span class="sxs-lookup"><span data-stu-id="aae74-121">startupAuthenticationTpmUsage</span></span>|[<span data-ttu-id="aae74-122">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="aae74-122">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="aae74-123">Gibt an, ob der TPM-Start zulässig/erforderlich/nicht zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="aae74-123">Indicates if TPM startup is allowed/required/disallowed.</span></span> <span data-ttu-id="aae74-124">Mögliche Werte sind: `blocked`, `required` und `allowed`.</span><span class="sxs-lookup"><span data-stu-id="aae74-124">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="aae74-125">startupAuthenticationTpmPinUsage</span><span class="sxs-lookup"><span data-stu-id="aae74-125">startupAuthenticationTpmPinUsage</span></span>|[<span data-ttu-id="aae74-126">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="aae74-126">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="aae74-127">Gibt an, ob die TPM-Start Pin zulässig/erforderlich/nicht zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="aae74-127">Indicates if TPM startup pin is allowed/required/disallowed.</span></span> <span data-ttu-id="aae74-128">Mögliche Werte sind: `blocked`, `required` und `allowed`.</span><span class="sxs-lookup"><span data-stu-id="aae74-128">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="aae74-129">startupAuthenticationTpmKeyUsage</span><span class="sxs-lookup"><span data-stu-id="aae74-129">startupAuthenticationTpmKeyUsage</span></span>|[<span data-ttu-id="aae74-130">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="aae74-130">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="aae74-131">Gibt an, ob der TPM-Startschlüssel zulässig/erforderlich/nicht zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="aae74-131">Indicates if TPM startup key is allowed/required/disallowed.</span></span> <span data-ttu-id="aae74-132">Mögliche Werte sind: `blocked`, `required` und `allowed`.</span><span class="sxs-lookup"><span data-stu-id="aae74-132">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="aae74-133">startupAuthenticationTpmPinAndKeyUsage</span><span class="sxs-lookup"><span data-stu-id="aae74-133">startupAuthenticationTpmPinAndKeyUsage</span></span>|[<span data-ttu-id="aae74-134">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="aae74-134">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="aae74-135">Gibt an, ob die TPM-Start-PIN und der Schlüssel zulässig/erforderlich/nicht zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="aae74-135">Indicates if TPM startup pin key and key are allowed/required/disallowed.</span></span> <span data-ttu-id="aae74-136">Mögliche Werte sind: `blocked`, `required` und `allowed`.</span><span class="sxs-lookup"><span data-stu-id="aae74-136">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="aae74-137">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="aae74-137">minimumPinLength</span></span>|<span data-ttu-id="aae74-138">Int32</span><span class="sxs-lookup"><span data-stu-id="aae74-138">Int32</span></span>|<span data-ttu-id="aae74-139">Gibt die minimale Länge der Start-PIN an.</span><span class="sxs-lookup"><span data-stu-id="aae74-139">Indicates the minimum length of startup pin.</span></span> <span data-ttu-id="aae74-140">Gültige Werte 4 bis 20</span><span class="sxs-lookup"><span data-stu-id="aae74-140">Valid values 4 to 20</span></span>|
|<span data-ttu-id="aae74-141">recoveryOptions</span><span class="sxs-lookup"><span data-stu-id="aae74-141">recoveryOptions</span></span>|[<span data-ttu-id="aae74-142">bitLockerRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="aae74-142">bitLockerRecoveryOptions</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|<span data-ttu-id="aae74-143">Ermöglicht die Wiederherstellung von BitLocker-verschlüsselten Betriebssystemlaufwerken, wenn die erforderlichen Startschlüssel Informationen fehlen.</span><span class="sxs-lookup"><span data-stu-id="aae74-143">Allows to recover BitLocker encrypted operating system drives in the absence of the required startup key information.</span></span> <span data-ttu-id="aae74-144">Diese Richtlinieneinstellung wird angewendet, wenn Sie BitLocker aktivieren.</span><span class="sxs-lookup"><span data-stu-id="aae74-144">This policy setting is applied when you turn on BitLocker.</span></span>|
|<span data-ttu-id="aae74-145">Prebootrecoveryenablemessageandurl wurden</span><span class="sxs-lookup"><span data-stu-id="aae74-145">prebootRecoveryEnableMessageAndUrl</span></span>|<span data-ttu-id="aae74-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="aae74-146">Boolean</span></span>|<span data-ttu-id="aae74-147">Aktivieren Sie die Vorabstart-Wiederherstellungs Nachricht und-URL.</span><span class="sxs-lookup"><span data-stu-id="aae74-147">Enable pre-boot recovery message and Url.</span></span> <span data-ttu-id="aae74-148">Wenn requireStartupAuthentication auf false festgelegt ist, wirkt sich dieser Wert nicht aus.</span><span class="sxs-lookup"><span data-stu-id="aae74-148">If requireStartupAuthentication is false, this value does not affect.</span></span>|
|<span data-ttu-id="aae74-149">prebootRecoveryMessage</span><span class="sxs-lookup"><span data-stu-id="aae74-149">prebootRecoveryMessage</span></span>|<span data-ttu-id="aae74-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="aae74-150">String</span></span>|<span data-ttu-id="aae74-151">Definiert eine benutzerdefinierte Wiederherstellungs Nachricht.</span><span class="sxs-lookup"><span data-stu-id="aae74-151">Defines a custom recovery message.</span></span>|
|<span data-ttu-id="aae74-152">prebootRecoveryUrl</span><span class="sxs-lookup"><span data-stu-id="aae74-152">prebootRecoveryUrl</span></span>|<span data-ttu-id="aae74-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="aae74-153">String</span></span>|<span data-ttu-id="aae74-154">Definiert eine benutzerdefinierte Wiederherstellungs-URL.</span><span class="sxs-lookup"><span data-stu-id="aae74-154">Defines a custom recovery URL.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aae74-155">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="aae74-155">Relationships</span></span>
<span data-ttu-id="aae74-156">Keine</span><span class="sxs-lookup"><span data-stu-id="aae74-156">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aae74-157">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="aae74-157">JSON Representation</span></span>
<span data-ttu-id="aae74-158">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="aae74-158">Here is a JSON representation of the resource.</span></span>
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




