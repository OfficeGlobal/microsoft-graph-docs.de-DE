---
title: ManagedDeviceEncryptionState erstellen
description: Erstellen eines neuen managedDeviceEncryptionState-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 859f8fff57b90e86421b7720cc48c6cc979fce40
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30177903"
---
# <a name="create-manageddeviceencryptionstate"></a><span data-ttu-id="842dd-103">ManagedDeviceEncryptionState erstellen</span><span class="sxs-lookup"><span data-stu-id="842dd-103">Create managedDeviceEncryptionState</span></span>

> <span data-ttu-id="842dd-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="842dd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="842dd-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="842dd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="842dd-106">Erstellen eines neuen [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="842dd-106">Create a new [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="842dd-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="842dd-107">Prerequisites</span></span>
<span data-ttu-id="842dd-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="842dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="842dd-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="842dd-110">Permission type</span></span>|<span data-ttu-id="842dd-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="842dd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="842dd-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="842dd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="842dd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="842dd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="842dd-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="842dd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="842dd-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="842dd-115">Not supported.</span></span>|
|<span data-ttu-id="842dd-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="842dd-116">Application</span></span>|<span data-ttu-id="842dd-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="842dd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="842dd-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="842dd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDeviceEncryptionStates
```

## <a name="request-headers"></a><span data-ttu-id="842dd-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="842dd-119">Request headers</span></span>
|<span data-ttu-id="842dd-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="842dd-120">Header</span></span>|<span data-ttu-id="842dd-121">Wert</span><span class="sxs-lookup"><span data-stu-id="842dd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="842dd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="842dd-122">Authorization</span></span>|<span data-ttu-id="842dd-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="842dd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="842dd-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="842dd-124">Accept</span></span>|<span data-ttu-id="842dd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="842dd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="842dd-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="842dd-126">Request body</span></span>
<span data-ttu-id="842dd-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das managedDeviceEncryptionState-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="842dd-127">In the request body, supply a JSON representation for the managedDeviceEncryptionState object.</span></span>

<span data-ttu-id="842dd-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der managedDeviceEncryptionState erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="842dd-128">The following table shows the properties that are required when you create the managedDeviceEncryptionState.</span></span>

|<span data-ttu-id="842dd-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="842dd-129">Property</span></span>|<span data-ttu-id="842dd-130">Typ</span><span class="sxs-lookup"><span data-stu-id="842dd-130">Type</span></span>|<span data-ttu-id="842dd-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="842dd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="842dd-132">id</span><span class="sxs-lookup"><span data-stu-id="842dd-132">id</span></span>|<span data-ttu-id="842dd-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="842dd-133">String</span></span>|<span data-ttu-id="842dd-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="842dd-134">Key of the entity.</span></span>|
|<span data-ttu-id="842dd-135">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="842dd-135">userPrincipalName</span></span>|<span data-ttu-id="842dd-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="842dd-136">String</span></span>|<span data-ttu-id="842dd-137">Benutzername</span><span class="sxs-lookup"><span data-stu-id="842dd-137">User name</span></span>|
|<span data-ttu-id="842dd-138">deviceType</span><span class="sxs-lookup"><span data-stu-id="842dd-138">deviceType</span></span>|[<span data-ttu-id="842dd-139">deviceTypes</span><span class="sxs-lookup"><span data-stu-id="842dd-139">deviceTypes</span></span>](../resources/intune-deviceconfig-devicetypes.md)|<span data-ttu-id="842dd-140">Plattform des Geräts.</span><span class="sxs-lookup"><span data-stu-id="842dd-140">Platform of the device.</span></span> <span data-ttu-id="842dd-141">Mögliche Werte sind: `desktop`, `windowsRT`, `winMO6` `nokia` `windowsPhone` `mac` `winCE` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM`,,,,,,,, `holoLens`,, `androidEnterprise` ,,,,,, `surfaceHub` `androidForWork` `winEmbedded` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="842dd-141">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="842dd-142">osVersion</span><span class="sxs-lookup"><span data-stu-id="842dd-142">osVersion</span></span>|<span data-ttu-id="842dd-143">String</span><span class="sxs-lookup"><span data-stu-id="842dd-143">String</span></span>|<span data-ttu-id="842dd-144">Betriebssystemversion des Geräts</span><span class="sxs-lookup"><span data-stu-id="842dd-144">Operating system version of the device</span></span>|
|<span data-ttu-id="842dd-145">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="842dd-145">tpmSpecificationVersion</span></span>|<span data-ttu-id="842dd-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="842dd-146">String</span></span>|<span data-ttu-id="842dd-147">Geräte-TPM-Version</span><span class="sxs-lookup"><span data-stu-id="842dd-147">Device TPM Version</span></span>|
|<span data-ttu-id="842dd-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="842dd-148">deviceName</span></span>|<span data-ttu-id="842dd-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="842dd-149">String</span></span>|<span data-ttu-id="842dd-150">Gerätename</span><span class="sxs-lookup"><span data-stu-id="842dd-150">Device name</span></span>|
|<span data-ttu-id="842dd-151">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="842dd-151">encryptionReadinessState</span></span>|[<span data-ttu-id="842dd-152">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="842dd-152">encryptionReadinessState</span></span>](../resources/intune-deviceconfig-encryptionreadinessstate.md)|<span data-ttu-id="842dd-153">Verschlüsselungs Bereitschaftsstatus.</span><span class="sxs-lookup"><span data-stu-id="842dd-153">Encryption readiness state.</span></span> <span data-ttu-id="842dd-154">Mögliche Werte sind: `notReady` und `ready`.</span><span class="sxs-lookup"><span data-stu-id="842dd-154">Possible values are: `notReady`, `ready`.</span></span>|
|<span data-ttu-id="842dd-155">encryptionState</span><span class="sxs-lookup"><span data-stu-id="842dd-155">encryptionState</span></span>|[<span data-ttu-id="842dd-156">encryptionState</span><span class="sxs-lookup"><span data-stu-id="842dd-156">encryptionState</span></span>](../resources/intune-deviceconfig-encryptionstate.md)|<span data-ttu-id="842dd-157">Geräte Verschlüsselungsstatus.</span><span class="sxs-lookup"><span data-stu-id="842dd-157">Device encryption state.</span></span> <span data-ttu-id="842dd-158">Mögliche Werte sind: `notEncrypted` und `encrypted`.</span><span class="sxs-lookup"><span data-stu-id="842dd-158">Possible values are: `notEncrypted`, `encrypted`.</span></span>|
|<span data-ttu-id="842dd-159">encryptionPolicySettingState</span><span class="sxs-lookup"><span data-stu-id="842dd-159">encryptionPolicySettingState</span></span>|[<span data-ttu-id="842dd-160">Wurde</span><span class="sxs-lookup"><span data-stu-id="842dd-160">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="842dd-161">Status der Verschlüsselungsrichtlinien Einstellung.</span><span class="sxs-lookup"><span data-stu-id="842dd-161">Encryption policy setting state.</span></span> <span data-ttu-id="842dd-162">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="842dd-162">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="842dd-163">advancedBitLockerStates</span><span class="sxs-lookup"><span data-stu-id="842dd-163">advancedBitLockerStates</span></span>|[<span data-ttu-id="842dd-164">advancedBitLockerState</span><span class="sxs-lookup"><span data-stu-id="842dd-164">advancedBitLockerState</span></span>](../resources/intune-deviceconfig-advancedbitlockerstate.md)|<span data-ttu-id="842dd-165">Erweiterter BitLocker-Status.</span><span class="sxs-lookup"><span data-stu-id="842dd-165">Advanced BitLocker State.</span></span> <span data-ttu-id="842dd-166">Mögliche Werte sind: `success`, `noUserConsent`, `osVolumeEncryptionMethodMismatch` `osVolumeTpmRequired` `osVolumeTpmOnlyRequired` `osVolumeTpmPinRequired` `osVolumeTpmStartupKeyRequired` `recoveryKeyBackupFailed` `fixedDriveNotEncrypted` `fixedDriveEncryptionMethodMismatch` `loggedOnUserNonAdmin` `windowsRecoveryEnvironmentNotConfigured` `tpmNotAvailable`,,,, `tpmNotReady`,,,,,,,,,, `networkError` `osVolumeTpmPinStartupKeyRequired` `osVolumeUnprotected`</span><span class="sxs-lookup"><span data-stu-id="842dd-166">Possible values are: `success`, `noUserConsent`, `osVolumeEncryptionMethodMismatch`, `osVolumeTpmRequired`, `osVolumeTpmOnlyRequired`, `osVolumeTpmPinRequired`, `osVolumeTpmStartupKeyRequired`, `osVolumeTpmPinStartupKeyRequired`, `osVolumeUnprotected`, `recoveryKeyBackupFailed`, `fixedDriveNotEncrypted`, `fixedDriveEncryptionMethodMismatch`, `loggedOnUserNonAdmin`, `windowsRecoveryEnvironmentNotConfigured`, `tpmNotAvailable`, `tpmNotReady`, `networkError`.</span></span>|
|<span data-ttu-id="842dd-167">policyDetails</span><span class="sxs-lookup"><span data-stu-id="842dd-167">policyDetails</span></span>|<span data-ttu-id="842dd-168">[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="842dd-168">[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md) collection</span></span>|<span data-ttu-id="842dd-169">Richtlinien Details</span><span class="sxs-lookup"><span data-stu-id="842dd-169">Policy Details</span></span>|



## <a name="response"></a><span data-ttu-id="842dd-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="842dd-170">Response</span></span>
<span data-ttu-id="842dd-171">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="842dd-171">If successful, this method returns a `201 Created` response code and a [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="842dd-172">Beispiel</span><span class="sxs-lookup"><span data-stu-id="842dd-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="842dd-173">Anforderung</span><span class="sxs-lookup"><span data-stu-id="842dd-173">Request</span></span>
<span data-ttu-id="842dd-174">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="842dd-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDeviceEncryptionStates
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

### <a name="response"></a><span data-ttu-id="842dd-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="842dd-175">Response</span></span>
<span data-ttu-id="842dd-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="842dd-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



