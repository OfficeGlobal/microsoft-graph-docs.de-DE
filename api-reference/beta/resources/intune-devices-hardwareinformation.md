---
title: Ressourcentyp hardwareInformation
description: Hardwareinformationen für ein bestimmtes Gerät.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 32b6d0e637c477265a6d23f39e531ca89c7e490c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394824"
---
# <a name="hardwareinformation-resource-type"></a><span data-ttu-id="ffc9d-103">Ressourcentyp hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="ffc9d-103">hardwareInformation resource type</span></span>

> <span data-ttu-id="ffc9d-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="ffc9d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ffc9d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ffc9d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ffc9d-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ffc9d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ffc9d-107">Hardwareinformationen für ein bestimmtes Gerät.</span><span class="sxs-lookup"><span data-stu-id="ffc9d-107">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="ffc9d-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ffc9d-108">Properties</span></span>
|<span data-ttu-id="ffc9d-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ffc9d-109">Property</span></span>|<span data-ttu-id="ffc9d-110">Typ</span><span class="sxs-lookup"><span data-stu-id="ffc9d-110">Type</span></span>|<span data-ttu-id="ffc9d-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ffc9d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffc9d-112">serialNumber</span><span class="sxs-lookup"><span data-stu-id="ffc9d-112">serialNumber</span></span>|<span data-ttu-id="ffc9d-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ffc9d-113">String</span></span>|<span data-ttu-id="ffc9d-114">Seriennummer.</span><span class="sxs-lookup"><span data-stu-id="ffc9d-114">Serial number.</span></span>|
|<span data-ttu-id="ffc9d-115">totalStorageSpace</span><span class="sxs-lookup"><span data-stu-id="ffc9d-115">totalStorageSpace</span></span>|<span data-ttu-id="ffc9d-116">Int64</span><span class="sxs-lookup"><span data-stu-id="ffc9d-116">Int64</span></span>|<span data-ttu-id="ffc9d-117">Gesamtmenge des Speicherplatzes des Geräts.</span><span class="sxs-lookup"><span data-stu-id="ffc9d-117">Total storage space of the device.</span></span>|
|<span data-ttu-id="ffc9d-118">freeStorageSpace</span><span class="sxs-lookup"><span data-stu-id="ffc9d-118">freeStorageSpace</span></span>|<span data-ttu-id="ffc9d-119">Int64</span><span class="sxs-lookup"><span data-stu-id="ffc9d-119">Int64</span></span>|<span data-ttu-id="ffc9d-120">Freier Speicherplatz des Geräts.</span><span class="sxs-lookup"><span data-stu-id="ffc9d-120">Free storage space of the device.</span></span>|
|<span data-ttu-id="ffc9d-121">imei</span><span class="sxs-lookup"><span data-stu-id="ffc9d-121">imei</span></span>|<span data-ttu-id="ffc9d-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ffc9d-122">String</span></span>|<span data-ttu-id="ffc9d-123">IMEI</span><span class="sxs-lookup"><span data-stu-id="ffc9d-123">IMEI</span></span>|
|<span data-ttu-id="ffc9d-124">meid</span><span class="sxs-lookup"><span data-stu-id="ffc9d-124">meid</span></span>|<span data-ttu-id="ffc9d-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ffc9d-125">String</span></span>|<span data-ttu-id="ffc9d-126">MEID</span><span class="sxs-lookup"><span data-stu-id="ffc9d-126">MEID</span></span>|
|<span data-ttu-id="ffc9d-127">manufacturer</span><span class="sxs-lookup"><span data-stu-id="ffc9d-127">manufacturer</span></span>|<span data-ttu-id="ffc9d-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ffc9d-128">String</span></span>|<span data-ttu-id="ffc9d-129">Hersteller des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="ffc9d-129">Manufacturer of the device</span></span>|
|<span data-ttu-id="ffc9d-130">model</span><span class="sxs-lookup"><span data-stu-id="ffc9d-130">model</span></span>|<span data-ttu-id="ffc9d-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ffc9d-131">String</span></span>|<span data-ttu-id="ffc9d-132">Modell des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="ffc9d-132">Model of the device</span></span>|
|<span data-ttu-id="ffc9d-133">PhoneNumber</span><span class="sxs-lookup"><span data-stu-id="ffc9d-133">phoneNumber</span></span>|<span data-ttu-id="ffc9d-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ffc9d-134">String</span></span>|<span data-ttu-id="ffc9d-135">Telefonnummer des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="ffc9d-135">Phone number of the device</span></span>|
|<span data-ttu-id="ffc9d-136">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="ffc9d-136">subscriberCarrier</span></span>|<span data-ttu-id="ffc9d-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ffc9d-137">String</span></span>|<span data-ttu-id="ffc9d-138">Abonnenten Netzbetreiber des Geräts</span><span class="sxs-lookup"><span data-stu-id="ffc9d-138">Subscriber carrier of the device</span></span>|
|<span data-ttu-id="ffc9d-139">cellularTechnology</span><span class="sxs-lookup"><span data-stu-id="ffc9d-139">cellularTechnology</span></span>|<span data-ttu-id="ffc9d-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ffc9d-140">String</span></span>|<span data-ttu-id="ffc9d-141">Mobilfunk-Technologie des Geräts</span><span class="sxs-lookup"><span data-stu-id="ffc9d-141">Cellular technology of the device</span></span>|
|<span data-ttu-id="ffc9d-142">wifiMac</span><span class="sxs-lookup"><span data-stu-id="ffc9d-142">wifiMac</span></span>|<span data-ttu-id="ffc9d-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ffc9d-143">String</span></span>|<span data-ttu-id="ffc9d-144">WLAN-MAC-Adresse des Geräts</span><span class="sxs-lookup"><span data-stu-id="ffc9d-144">WiFi MAC address of the device</span></span>|
|<span data-ttu-id="ffc9d-145">operatingSystemLanguage</span><span class="sxs-lookup"><span data-stu-id="ffc9d-145">operatingSystemLanguage</span></span>|<span data-ttu-id="ffc9d-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ffc9d-146">String</span></span>|<span data-ttu-id="ffc9d-147">Die Sprache des Betriebssystems des Geräts</span><span class="sxs-lookup"><span data-stu-id="ffc9d-147">Operating system language of the device</span></span>|
|<span data-ttu-id="ffc9d-148">isSupervised</span><span class="sxs-lookup"><span data-stu-id="ffc9d-148">isSupervised</span></span>|<span data-ttu-id="ffc9d-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffc9d-149">Boolean</span></span>|<span data-ttu-id="ffc9d-150">Überwachten Modus des Geräts</span><span class="sxs-lookup"><span data-stu-id="ffc9d-150">Supervised mode of the device</span></span>|
|<span data-ttu-id="ffc9d-151">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="ffc9d-151">isEncrypted</span></span>|<span data-ttu-id="ffc9d-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffc9d-152">Boolean</span></span>|<span data-ttu-id="ffc9d-153">Status der Verschlüsselung des Geräts</span><span class="sxs-lookup"><span data-stu-id="ffc9d-153">Encryption status of the device</span></span>|
|<span data-ttu-id="ffc9d-154">isSharedDevice</span><span class="sxs-lookup"><span data-stu-id="ffc9d-154">isSharedDevice</span></span>|<span data-ttu-id="ffc9d-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffc9d-155">Boolean</span></span>|<span data-ttu-id="ffc9d-156">Freigegebene iPad</span><span class="sxs-lookup"><span data-stu-id="ffc9d-156">Shared iPad</span></span>|
|<span data-ttu-id="ffc9d-157">sharedDeviceCachedUsers</span><span class="sxs-lookup"><span data-stu-id="ffc9d-157">sharedDeviceCachedUsers</span></span>|<span data-ttu-id="ffc9d-158">[SharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="ffc9d-158">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) collection</span></span>|<span data-ttu-id="ffc9d-159">Alle Benutzer auf dem freigegebenen Apple-Gerät</span><span class="sxs-lookup"><span data-stu-id="ffc9d-159">All users on the shared Apple device</span></span>|
|<span data-ttu-id="ffc9d-160">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="ffc9d-160">tpmSpecificationVersion</span></span>|<span data-ttu-id="ffc9d-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ffc9d-161">String</span></span>|<span data-ttu-id="ffc9d-162">Zeichenfolge, die die Spezifikation, Version angibt.</span><span class="sxs-lookup"><span data-stu-id="ffc9d-162">String that specifies the specification version.</span></span>|
|<span data-ttu-id="ffc9d-163">operatingSystemEdition</span><span class="sxs-lookup"><span data-stu-id="ffc9d-163">operatingSystemEdition</span></span>|<span data-ttu-id="ffc9d-164">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ffc9d-164">String</span></span>|<span data-ttu-id="ffc9d-165">Zeichenfolge, die die Betriebssystem Edition angibt.</span><span class="sxs-lookup"><span data-stu-id="ffc9d-165">String that specifies the OS edition.</span></span>|
|<span data-ttu-id="ffc9d-166">deviceFullQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="ffc9d-166">deviceFullQualifiedDomainName</span></span>|<span data-ttu-id="ffc9d-167">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ffc9d-167">String</span></span>|<span data-ttu-id="ffc9d-168">Gibt den vollqualifizierten Domänennamen des Geräts (falls vorhanden).</span><span class="sxs-lookup"><span data-stu-id="ffc9d-168">Returns the fully qualified domain name of the device (if any).</span></span> <span data-ttu-id="ffc9d-169">Wenn das Gerät nicht Mitglied einer Domäne ist, wird eine leere Zeichenfolge zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ffc9d-169">If the device is not domain-joined, it returns an empty string.</span></span> |
|<span data-ttu-id="ffc9d-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="ffc9d-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>|[<span data-ttu-id="ffc9d-171">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="ffc9d-171">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|<span data-ttu-id="ffc9d-172">Virtualisierung-basierte Hardware Anforderung Sicherheitsstatus.</span><span class="sxs-lookup"><span data-stu-id="ffc9d-172">Virtualization-based security hardware requirement status.</span></span> <span data-ttu-id="ffc9d-173">Mögliche Werte sind: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM` und `hyperVNotAvailable`.</span><span class="sxs-lookup"><span data-stu-id="ffc9d-173">Possible values are: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span></span>|
|<span data-ttu-id="ffc9d-174">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="ffc9d-174">deviceGuardVirtualizationBasedSecurityState</span></span>|[<span data-ttu-id="ffc9d-175">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="ffc9d-175">deviceGuardVirtualizationBasedSecurityState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|<span data-ttu-id="ffc9d-176">Virtualisierung-basierte Sicherheitsstatus.</span><span class="sxs-lookup"><span data-stu-id="ffc9d-176">Virtualization-based security status.</span></span> <span data-ttu-id="ffc9d-177">.</span><span class="sxs-lookup"><span data-stu-id="ffc9d-177"></span></span> <span data-ttu-id="ffc9d-178">Mögliche Werte sind: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements` und `other`.</span><span class="sxs-lookup"><span data-stu-id="ffc9d-178">Possible values are: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span></span>|
|<span data-ttu-id="ffc9d-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="ffc9d-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>|[<span data-ttu-id="ffc9d-180">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="ffc9d-180">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|<span data-ttu-id="ffc9d-181">Lokales System Autorität (LSA) Anmeldeinformationen Guard Status.</span><span class="sxs-lookup"><span data-stu-id="ffc9d-181">Local System Authority (LSA) credential guard status.</span></span> <span data-ttu-id="ffc9d-182">.</span><span class="sxs-lookup"><span data-stu-id="ffc9d-182"></span></span> <span data-ttu-id="ffc9d-183">Mögliche Werte sind: `running`, `rebootRequired`, `notLicensed`, `notConfigured` und `virtualizationBasedSecurityNotRunning`.</span><span class="sxs-lookup"><span data-stu-id="ffc9d-183">Possible values are: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ffc9d-184">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ffc9d-184">Relationships</span></span>
<span data-ttu-id="ffc9d-185">Keine</span><span class="sxs-lookup"><span data-stu-id="ffc9d-185">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ffc9d-186">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ffc9d-186">JSON Representation</span></span>
<span data-ttu-id="ffc9d-187">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ffc9d-187">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.hardwareInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hardwareInformation",
  "serialNumber": "String",
  "totalStorageSpace": 1024,
  "freeStorageSpace": 1024,
  "imei": "String",
  "meid": "String",
  "manufacturer": "String",
  "model": "String",
  "phoneNumber": "String",
  "subscriberCarrier": "String",
  "cellularTechnology": "String",
  "wifiMac": "String",
  "operatingSystemLanguage": "String",
  "isSupervised": true,
  "isEncrypted": true,
  "isSharedDevice": true,
  "sharedDeviceCachedUsers": [
    {
      "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
      "userPrincipalName": "String",
      "dataToSync": true,
      "dataQuota": 1024,
      "dataUsed": 1024
    }
  ],
  "tpmSpecificationVersion": "String",
  "operatingSystemEdition": "String",
  "deviceFullQualifiedDomainName": "String",
  "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "String",
  "deviceGuardVirtualizationBasedSecurityState": "String",
  "deviceGuardLocalSystemAuthorityCredentialGuardState": "String"
}
```




