---
title: ManagedDeviceEncryptionState aktualisieren
description: Aktualisieren der Eigenschaften eines managedDeviceEncryptionState-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9898d9eeb5e26dfa13707f5e93faa9907bcf1dee
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30978213"
---
# <a name="update-manageddeviceencryptionstate"></a><span data-ttu-id="79767-103">ManagedDeviceEncryptionState aktualisieren</span><span class="sxs-lookup"><span data-stu-id="79767-103">Update managedDeviceEncryptionState</span></span>

> <span data-ttu-id="79767-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="79767-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79767-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="79767-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79767-106">Aktualisieren der Eigenschaften eines [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="79767-106">Update the properties of a [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79767-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="79767-107">Prerequisites</span></span>
<span data-ttu-id="79767-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79767-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79767-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="79767-110">Permission type</span></span>|<span data-ttu-id="79767-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="79767-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79767-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="79767-112">Delegated (work or school account)</span></span>|<span data-ttu-id="79767-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79767-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="79767-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="79767-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79767-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="79767-115">Not supported.</span></span>|
|<span data-ttu-id="79767-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="79767-116">Application</span></span>|<span data-ttu-id="79767-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="79767-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="79767-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="79767-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceEncryptionStates/{managedDeviceEncryptionStateId}
```

## <a name="request-headers"></a><span data-ttu-id="79767-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="79767-119">Request headers</span></span>
|<span data-ttu-id="79767-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="79767-120">Header</span></span>|<span data-ttu-id="79767-121">Wert</span><span class="sxs-lookup"><span data-stu-id="79767-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79767-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="79767-122">Authorization</span></span>|<span data-ttu-id="79767-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="79767-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79767-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="79767-124">Accept</span></span>|<span data-ttu-id="79767-125">application/json</span><span class="sxs-lookup"><span data-stu-id="79767-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79767-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="79767-126">Request body</span></span>
<span data-ttu-id="79767-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="79767-127">In the request body, supply a JSON representation for the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>

<span data-ttu-id="79767-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="79767-128">The following table shows the properties that are required when you create the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md).</span></span>

|<span data-ttu-id="79767-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="79767-129">Property</span></span>|<span data-ttu-id="79767-130">Typ</span><span class="sxs-lookup"><span data-stu-id="79767-130">Type</span></span>|<span data-ttu-id="79767-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="79767-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79767-132">id</span><span class="sxs-lookup"><span data-stu-id="79767-132">id</span></span>|<span data-ttu-id="79767-133">String</span><span class="sxs-lookup"><span data-stu-id="79767-133">String</span></span>|<span data-ttu-id="79767-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="79767-134">Key of the entity.</span></span>|
|<span data-ttu-id="79767-135">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="79767-135">userPrincipalName</span></span>|<span data-ttu-id="79767-136">String</span><span class="sxs-lookup"><span data-stu-id="79767-136">String</span></span>|<span data-ttu-id="79767-137">Benutzername</span><span class="sxs-lookup"><span data-stu-id="79767-137">User name</span></span>|
|<span data-ttu-id="79767-138">deviceType</span><span class="sxs-lookup"><span data-stu-id="79767-138">deviceType</span></span>|[<span data-ttu-id="79767-139">deviceTypes</span><span class="sxs-lookup"><span data-stu-id="79767-139">deviceTypes</span></span>](../resources/intune-deviceconfig-devicetypes.md)|<span data-ttu-id="79767-140">Plattform des Geräts.</span><span class="sxs-lookup"><span data-stu-id="79767-140">Platform of the device.</span></span> <span data-ttu-id="79767-141">Mögliche Werte sind: `desktop`, `windowsRT`, `winMO6` `nokia` `windowsPhone` `mac` `winCE` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM`,,,,,,,, `holoLens`,, `androidEnterprise` ,,,,,, `surfaceHub` `androidForWork` `winEmbedded` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="79767-141">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="79767-142">osVersion</span><span class="sxs-lookup"><span data-stu-id="79767-142">osVersion</span></span>|<span data-ttu-id="79767-143">String</span><span class="sxs-lookup"><span data-stu-id="79767-143">String</span></span>|<span data-ttu-id="79767-144">Betriebssystemversion des Geräts</span><span class="sxs-lookup"><span data-stu-id="79767-144">Operating system version of the device</span></span>|
|<span data-ttu-id="79767-145">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="79767-145">tpmSpecificationVersion</span></span>|<span data-ttu-id="79767-146">String</span><span class="sxs-lookup"><span data-stu-id="79767-146">String</span></span>|<span data-ttu-id="79767-147">Geräte-TPM-Version</span><span class="sxs-lookup"><span data-stu-id="79767-147">Device TPM Version</span></span>|
|<span data-ttu-id="79767-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="79767-148">deviceName</span></span>|<span data-ttu-id="79767-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="79767-149">String</span></span>|<span data-ttu-id="79767-150">Gerätename</span><span class="sxs-lookup"><span data-stu-id="79767-150">Device name</span></span>|
|<span data-ttu-id="79767-151">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="79767-151">encryptionReadinessState</span></span>|[<span data-ttu-id="79767-152">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="79767-152">encryptionReadinessState</span></span>](../resources/intune-deviceconfig-encryptionreadinessstate.md)|<span data-ttu-id="79767-153">Verschlüsselungs Bereitschaftsstatus.</span><span class="sxs-lookup"><span data-stu-id="79767-153">Encryption readiness state.</span></span> <span data-ttu-id="79767-154">Mögliche Werte sind: `notReady` und `ready`.</span><span class="sxs-lookup"><span data-stu-id="79767-154">Possible values are: `notReady`, `ready`.</span></span>|
|<span data-ttu-id="79767-155">encryptionState</span><span class="sxs-lookup"><span data-stu-id="79767-155">encryptionState</span></span>|[<span data-ttu-id="79767-156">encryptionState</span><span class="sxs-lookup"><span data-stu-id="79767-156">encryptionState</span></span>](../resources/intune-deviceconfig-encryptionstate.md)|<span data-ttu-id="79767-157">Geräte Verschlüsselungsstatus.</span><span class="sxs-lookup"><span data-stu-id="79767-157">Device encryption state.</span></span> <span data-ttu-id="79767-158">Mögliche Werte sind: `notEncrypted` und `encrypted`.</span><span class="sxs-lookup"><span data-stu-id="79767-158">Possible values are: `notEncrypted`, `encrypted`.</span></span>|
|<span data-ttu-id="79767-159">encryptionPolicySettingState</span><span class="sxs-lookup"><span data-stu-id="79767-159">encryptionPolicySettingState</span></span>|[<span data-ttu-id="79767-160">Wurde</span><span class="sxs-lookup"><span data-stu-id="79767-160">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="79767-161">Status der Verschlüsselungsrichtlinien Einstellung.</span><span class="sxs-lookup"><span data-stu-id="79767-161">Encryption policy setting state.</span></span> <span data-ttu-id="79767-162">Mögliche Werte: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="79767-162">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="79767-163">advancedBitLockerStates</span><span class="sxs-lookup"><span data-stu-id="79767-163">advancedBitLockerStates</span></span>|[<span data-ttu-id="79767-164">advancedBitLockerState</span><span class="sxs-lookup"><span data-stu-id="79767-164">advancedBitLockerState</span></span>](../resources/intune-deviceconfig-advancedbitlockerstate.md)|<span data-ttu-id="79767-165">Erweiterter BitLocker-Status.</span><span class="sxs-lookup"><span data-stu-id="79767-165">Advanced BitLocker State.</span></span> <span data-ttu-id="79767-166">Mögliche Werte sind: `success`, `noUserConsent`, `osVolumeEncryptionMethodMismatch` `osVolumeTpmRequired` `osVolumeTpmOnlyRequired` `osVolumeTpmPinRequired` `osVolumeTpmStartupKeyRequired` `recoveryKeyBackupFailed` `fixedDriveNotEncrypted` `fixedDriveEncryptionMethodMismatch` `loggedOnUserNonAdmin` `windowsRecoveryEnvironmentNotConfigured` `tpmNotAvailable`,,,, `tpmNotReady`,,,,,,,,,, `networkError` `osVolumeTpmPinStartupKeyRequired` `osVolumeUnprotected`</span><span class="sxs-lookup"><span data-stu-id="79767-166">Possible values are: `success`, `noUserConsent`, `osVolumeEncryptionMethodMismatch`, `osVolumeTpmRequired`, `osVolumeTpmOnlyRequired`, `osVolumeTpmPinRequired`, `osVolumeTpmStartupKeyRequired`, `osVolumeTpmPinStartupKeyRequired`, `osVolumeUnprotected`, `recoveryKeyBackupFailed`, `fixedDriveNotEncrypted`, `fixedDriveEncryptionMethodMismatch`, `loggedOnUserNonAdmin`, `windowsRecoveryEnvironmentNotConfigured`, `tpmNotAvailable`, `tpmNotReady`, `networkError`.</span></span>|
|<span data-ttu-id="79767-167">policyDetails</span><span class="sxs-lookup"><span data-stu-id="79767-167">policyDetails</span></span>|<span data-ttu-id="79767-168">[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="79767-168">[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md) collection</span></span>|<span data-ttu-id="79767-169">Richtlinien Details</span><span class="sxs-lookup"><span data-stu-id="79767-169">Policy Details</span></span>|



## <a name="response"></a><span data-ttu-id="79767-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="79767-170">Response</span></span>
<span data-ttu-id="79767-171">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="79767-171">If successful, this method returns a `200 OK` response code and an updated [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79767-172">Beispiel</span><span class="sxs-lookup"><span data-stu-id="79767-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="79767-173">Anforderung</span><span class="sxs-lookup"><span data-stu-id="79767-173">Request</span></span>
<span data-ttu-id="79767-174">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="79767-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDeviceEncryptionStates/{managedDeviceEncryptionStateId}
Content-type: application/json
Content-length: 658

{
  "@odata.type": "#microsoft.graph.managedDeviceEncryptionState",
  "userPrincipalName": "User Principal Name value",
  "deviceType": "windowsRT",
  "osVersion": "Os Version value",
  "tpmSpecificationVersion": "Tpm Specification Version value",
  "deviceName": "Device Name value",
  "encryptionReadinessState": "ready",
  "encryptionState": "encrypted",
  "encryptionPolicySettingState": "notApplicable",
  "advancedBitLockerStates": "noUserConsent",
  "policyDetails": [
    {
      "@odata.type": "microsoft.graph.encryptionReportPolicyDetails",
      "policyId": "Policy Id value",
      "policyName": "Policy Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="79767-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="79767-175">Response</span></span>
<span data-ttu-id="79767-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="79767-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 707

{
  "@odata.type": "#microsoft.graph.managedDeviceEncryptionState",
  "id": "f09b4ab6-4ab6-f09b-b64a-9bf0b64a9bf0",
  "userPrincipalName": "User Principal Name value",
  "deviceType": "windowsRT",
  "osVersion": "Os Version value",
  "tpmSpecificationVersion": "Tpm Specification Version value",
  "deviceName": "Device Name value",
  "encryptionReadinessState": "ready",
  "encryptionState": "encrypted",
  "encryptionPolicySettingState": "notApplicable",
  "advancedBitLockerStates": "noUserConsent",
  "policyDetails": [
    {
      "@odata.type": "microsoft.graph.encryptionReportPolicyDetails",
      "policyId": "Policy Id value",
      "policyName": "Policy Name value"
    }
  ]
}
```




