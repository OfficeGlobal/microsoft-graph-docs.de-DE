---
title: Dem-Ressourcentyp
description: Hardware Informationen eines bestimmten Geräts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: be7d87f1d596a4756b3e964cd57f29da60f1c468
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172877"
---
# <a name="hardwareinformation-resource-type"></a><span data-ttu-id="55b33-103">Dem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="55b33-103">hardwareInformation resource type</span></span>

> <span data-ttu-id="55b33-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="55b33-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55b33-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="55b33-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55b33-106">Hardware Informationen eines bestimmten Geräts.</span><span class="sxs-lookup"><span data-stu-id="55b33-106">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="55b33-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="55b33-107">Properties</span></span>
|<span data-ttu-id="55b33-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="55b33-108">Property</span></span>|<span data-ttu-id="55b33-109">Typ</span><span class="sxs-lookup"><span data-stu-id="55b33-109">Type</span></span>|<span data-ttu-id="55b33-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="55b33-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55b33-111">serialNumber</span><span class="sxs-lookup"><span data-stu-id="55b33-111">serialNumber</span></span>|<span data-ttu-id="55b33-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="55b33-112">String</span></span>|<span data-ttu-id="55b33-113">Seriennummer.</span><span class="sxs-lookup"><span data-stu-id="55b33-113">Serial number.</span></span>|
|<span data-ttu-id="55b33-114">totalStorageSpace</span><span class="sxs-lookup"><span data-stu-id="55b33-114">totalStorageSpace</span></span>|<span data-ttu-id="55b33-115">Int64</span><span class="sxs-lookup"><span data-stu-id="55b33-115">Int64</span></span>|<span data-ttu-id="55b33-116">Der gesamte Speicherplatz des Geräts.</span><span class="sxs-lookup"><span data-stu-id="55b33-116">Total storage space of the device.</span></span>|
|<span data-ttu-id="55b33-117">freeStorageSpace</span><span class="sxs-lookup"><span data-stu-id="55b33-117">freeStorageSpace</span></span>|<span data-ttu-id="55b33-118">Int64</span><span class="sxs-lookup"><span data-stu-id="55b33-118">Int64</span></span>|<span data-ttu-id="55b33-119">Freier Speicherplatz des Geräts.</span><span class="sxs-lookup"><span data-stu-id="55b33-119">Free storage space of the device.</span></span>|
|<span data-ttu-id="55b33-120">imei</span><span class="sxs-lookup"><span data-stu-id="55b33-120">imei</span></span>|<span data-ttu-id="55b33-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="55b33-121">String</span></span>|<span data-ttu-id="55b33-122">IMEI</span><span class="sxs-lookup"><span data-stu-id="55b33-122">IMEI</span></span>|
|<span data-ttu-id="55b33-123">meid</span><span class="sxs-lookup"><span data-stu-id="55b33-123">meid</span></span>|<span data-ttu-id="55b33-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="55b33-124">String</span></span>|<span data-ttu-id="55b33-125">MEID</span><span class="sxs-lookup"><span data-stu-id="55b33-125">MEID</span></span>|
|<span data-ttu-id="55b33-126">manufacturer</span><span class="sxs-lookup"><span data-stu-id="55b33-126">manufacturer</span></span>|<span data-ttu-id="55b33-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="55b33-127">String</span></span>|<span data-ttu-id="55b33-128">Hersteller des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="55b33-128">Manufacturer of the device</span></span>|
|<span data-ttu-id="55b33-129">model</span><span class="sxs-lookup"><span data-stu-id="55b33-129">model</span></span>|<span data-ttu-id="55b33-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="55b33-130">String</span></span>|<span data-ttu-id="55b33-131">Modell des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="55b33-131">Model of the device</span></span>|
|<span data-ttu-id="55b33-132">PhoneNumber</span><span class="sxs-lookup"><span data-stu-id="55b33-132">phoneNumber</span></span>|<span data-ttu-id="55b33-133">String</span><span class="sxs-lookup"><span data-stu-id="55b33-133">String</span></span>|<span data-ttu-id="55b33-134">Telefonnummer des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="55b33-134">Phone number of the device</span></span>|
|<span data-ttu-id="55b33-135">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="55b33-135">subscriberCarrier</span></span>|<span data-ttu-id="55b33-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="55b33-136">String</span></span>|<span data-ttu-id="55b33-137">Teilnehmernetzbetreiber des Geräts</span><span class="sxs-lookup"><span data-stu-id="55b33-137">Subscriber carrier of the device</span></span>|
|<span data-ttu-id="55b33-138">cellularTechnology</span><span class="sxs-lookup"><span data-stu-id="55b33-138">cellularTechnology</span></span>|<span data-ttu-id="55b33-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="55b33-139">String</span></span>|<span data-ttu-id="55b33-140">Mobilfunktechnologie des Geräts</span><span class="sxs-lookup"><span data-stu-id="55b33-140">Cellular technology of the device</span></span>|
|<span data-ttu-id="55b33-141">wifiMac</span><span class="sxs-lookup"><span data-stu-id="55b33-141">wifiMac</span></span>|<span data-ttu-id="55b33-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="55b33-142">String</span></span>|<span data-ttu-id="55b33-143">WiFi-MAC-Adresse des Geräts</span><span class="sxs-lookup"><span data-stu-id="55b33-143">WiFi MAC address of the device</span></span>|
|<span data-ttu-id="55b33-144">operatingSystemLanguage</span><span class="sxs-lookup"><span data-stu-id="55b33-144">operatingSystemLanguage</span></span>|<span data-ttu-id="55b33-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="55b33-145">String</span></span>|<span data-ttu-id="55b33-146">Betriebssystemsprache des Geräts</span><span class="sxs-lookup"><span data-stu-id="55b33-146">Operating system language of the device</span></span>|
|<span data-ttu-id="55b33-147">isSupervised</span><span class="sxs-lookup"><span data-stu-id="55b33-147">isSupervised</span></span>|<span data-ttu-id="55b33-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="55b33-148">Boolean</span></span>|<span data-ttu-id="55b33-149">Überwachter Modus des Geräts</span><span class="sxs-lookup"><span data-stu-id="55b33-149">Supervised mode of the device</span></span>|
|<span data-ttu-id="55b33-150">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="55b33-150">isEncrypted</span></span>|<span data-ttu-id="55b33-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="55b33-151">Boolean</span></span>|<span data-ttu-id="55b33-152">Verschlüsselungsstatus des Geräts</span><span class="sxs-lookup"><span data-stu-id="55b33-152">Encryption status of the device</span></span>|
|<span data-ttu-id="55b33-153">isSharedDevice</span><span class="sxs-lookup"><span data-stu-id="55b33-153">isSharedDevice</span></span>|<span data-ttu-id="55b33-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="55b33-154">Boolean</span></span>|<span data-ttu-id="55b33-155">FreigeGebenes iPad</span><span class="sxs-lookup"><span data-stu-id="55b33-155">Shared iPad</span></span>|
|<span data-ttu-id="55b33-156">Shareddevicecachedusers wurden</span><span class="sxs-lookup"><span data-stu-id="55b33-156">sharedDeviceCachedUsers</span></span>|<span data-ttu-id="55b33-157">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="55b33-157">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) collection</span></span>|<span data-ttu-id="55b33-158">Alle Benutzer auf dem freigegebenen Apple-Gerät</span><span class="sxs-lookup"><span data-stu-id="55b33-158">All users on the shared Apple device</span></span>|
|<span data-ttu-id="55b33-159">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="55b33-159">tpmSpecificationVersion</span></span>|<span data-ttu-id="55b33-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="55b33-160">String</span></span>|<span data-ttu-id="55b33-161">Zeichenfolge, die die Spezifikationsversion angibt.</span><span class="sxs-lookup"><span data-stu-id="55b33-161">String that specifies the specification version.</span></span>|
|<span data-ttu-id="55b33-162">operatingSystemEdition</span><span class="sxs-lookup"><span data-stu-id="55b33-162">operatingSystemEdition</span></span>|<span data-ttu-id="55b33-163">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="55b33-163">String</span></span>|<span data-ttu-id="55b33-164">Zeichenfolge, die die OS-Edition angibt.</span><span class="sxs-lookup"><span data-stu-id="55b33-164">String that specifies the OS edition.</span></span>|
|<span data-ttu-id="55b33-165">deviceFullQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="55b33-165">deviceFullQualifiedDomainName</span></span>|<span data-ttu-id="55b33-166">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="55b33-166">String</span></span>|<span data-ttu-id="55b33-167">Gibt den vollqualifizierten Domänennamen des Geräts zurück (sofern vorhanden).</span><span class="sxs-lookup"><span data-stu-id="55b33-167">Returns the fully qualified domain name of the device (if any).</span></span> <span data-ttu-id="55b33-168">Wenn das Gerät nicht mit einer Domäne verbunden ist, wird eine leere Zeichenfolge zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="55b33-168">If the device is not domain-joined, it returns an empty string.</span></span> |
|<span data-ttu-id="55b33-169">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="55b33-169">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>|[<span data-ttu-id="55b33-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="55b33-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|<span data-ttu-id="55b33-171">Virtualisierungs-basierter Sicherheitshardware-Anforderungsstatus.</span><span class="sxs-lookup"><span data-stu-id="55b33-171">Virtualization-based security hardware requirement status.</span></span> <span data-ttu-id="55b33-172">Mögliche Werte: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span><span class="sxs-lookup"><span data-stu-id="55b33-172">Possible values are: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span></span>|
|<span data-ttu-id="55b33-173">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="55b33-173">deviceGuardVirtualizationBasedSecurityState</span></span>|[<span data-ttu-id="55b33-174">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="55b33-174">deviceGuardVirtualizationBasedSecurityState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|<span data-ttu-id="55b33-175">Virtualisierungs-basierter Sicherheitsstatus.</span><span class="sxs-lookup"><span data-stu-id="55b33-175">Virtualization-based security status.</span></span> <span data-ttu-id="55b33-176">.</span><span class="sxs-lookup"><span data-stu-id="55b33-176"></span></span> <span data-ttu-id="55b33-177">Mögliche Werte sind: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements` und `other`.</span><span class="sxs-lookup"><span data-stu-id="55b33-177">Possible values are: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span></span>|
|<span data-ttu-id="55b33-178">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="55b33-178">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>|[<span data-ttu-id="55b33-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="55b33-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|<span data-ttu-id="55b33-180">Status der LSA-Anmeldeinformationen (Local System Authority).</span><span class="sxs-lookup"><span data-stu-id="55b33-180">Local System Authority (LSA) credential guard status.</span></span> <span data-ttu-id="55b33-181">.</span><span class="sxs-lookup"><span data-stu-id="55b33-181"></span></span> <span data-ttu-id="55b33-182">Mögliche Werte: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span><span class="sxs-lookup"><span data-stu-id="55b33-182">Possible values are: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="55b33-183">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="55b33-183">Relationships</span></span>
<span data-ttu-id="55b33-184">Keine</span><span class="sxs-lookup"><span data-stu-id="55b33-184">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="55b33-185">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="55b33-185">JSON Representation</span></span>
<span data-ttu-id="55b33-186">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="55b33-186">Here is a JSON representation of the resource.</span></span>
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




