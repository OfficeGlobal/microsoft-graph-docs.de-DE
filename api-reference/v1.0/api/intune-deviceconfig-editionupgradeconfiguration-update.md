---
title: Aktualisieren von „editionUpgradeConfiguration“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs editionUpgradeConfiguration.
author: tfitzmac
ms.openlocfilehash: 011a9869ae7c15853e246292ac0acb80e7ad650f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329113"
---
# <a name="update-editionupgradeconfiguration"></a><span data-ttu-id="8e755-103">Aktualisieren von „editionUpgradeConfiguration“</span><span class="sxs-lookup"><span data-stu-id="8e755-103">Update editionUpgradeConfiguration</span></span>

> <span data-ttu-id="8e755-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8e755-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8e755-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8e755-105">Update the properties of a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8e755-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8e755-106">Prerequisites</span></span>
<span data-ttu-id="8e755-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e755-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e755-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8e755-109">Permission type</span></span>|<span data-ttu-id="8e755-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8e755-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e755-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8e755-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8e755-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e755-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8e755-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8e755-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e755-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8e755-114">Not supported.</span></span>|
|<span data-ttu-id="8e755-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8e755-115">Application</span></span>|<span data-ttu-id="8e755-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8e755-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e755-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8e755-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="8e755-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8e755-118">Request headers</span></span>
|<span data-ttu-id="8e755-119">Header</span><span class="sxs-lookup"><span data-stu-id="8e755-119">Header</span></span>|<span data-ttu-id="8e755-120">Wert</span><span class="sxs-lookup"><span data-stu-id="8e755-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e755-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="8e755-121">Authorization</span></span>|<span data-ttu-id="8e755-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8e755-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e755-123">Accept</span><span class="sxs-lookup"><span data-stu-id="8e755-123">Accept</span></span>|<span data-ttu-id="8e755-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8e755-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e755-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8e755-125">Request body</span></span>
<span data-ttu-id="8e755-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="8e755-126">In the request body, supply a JSON representation for the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

<span data-ttu-id="8e755-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="8e755-127">The following table shows the properties that are required when you create the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span></span>

|<span data-ttu-id="8e755-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8e755-128">Property</span></span>|<span data-ttu-id="8e755-129">Typ</span><span class="sxs-lookup"><span data-stu-id="8e755-129">Type</span></span>|<span data-ttu-id="8e755-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8e755-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e755-131">id</span><span class="sxs-lookup"><span data-stu-id="8e755-131">id</span></span>|<span data-ttu-id="8e755-132">String</span><span class="sxs-lookup"><span data-stu-id="8e755-132">String</span></span>|<span data-ttu-id="8e755-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="8e755-133">Key of the entity.</span></span> <span data-ttu-id="8e755-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8e755-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8e755-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8e755-135">lastModifiedDateTime</span></span>|<span data-ttu-id="8e755-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e755-136">DateTimeOffset</span></span>|<span data-ttu-id="8e755-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="8e755-137">DateTime the object was last modified.</span></span> <span data-ttu-id="8e755-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8e755-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8e755-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8e755-139">createdDateTime</span></span>|<span data-ttu-id="8e755-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e755-140">DateTimeOffset</span></span>|<span data-ttu-id="8e755-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="8e755-141">DateTime the object was created.</span></span> <span data-ttu-id="8e755-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8e755-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8e755-143">description</span><span class="sxs-lookup"><span data-stu-id="8e755-143">description</span></span>|<span data-ttu-id="8e755-144">String</span><span class="sxs-lookup"><span data-stu-id="8e755-144">String</span></span>|<span data-ttu-id="8e755-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="8e755-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8e755-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8e755-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8e755-147">displayName</span><span class="sxs-lookup"><span data-stu-id="8e755-147">displayName</span></span>|<span data-ttu-id="8e755-148">String</span><span class="sxs-lookup"><span data-stu-id="8e755-148">String</span></span>|<span data-ttu-id="8e755-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="8e755-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8e755-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8e755-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8e755-151">Version</span><span class="sxs-lookup"><span data-stu-id="8e755-151">version</span></span>|<span data-ttu-id="8e755-152">Int32</span><span class="sxs-lookup"><span data-stu-id="8e755-152">Int32</span></span>|<span data-ttu-id="8e755-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="8e755-153">Version of the device configuration.</span></span> <span data-ttu-id="8e755-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8e755-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8e755-155">licenseType</span><span class="sxs-lookup"><span data-stu-id="8e755-155">licenseType</span></span>|[<span data-ttu-id="8e755-156">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="8e755-156">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="8e755-157">Typ der Edition Upgrade-Lizenz.</span><span class="sxs-lookup"><span data-stu-id="8e755-157">Edition Upgrade License Type.</span></span> <span data-ttu-id="8e755-158">Mögliche Werte sind: `productKey` und `licenseFile`.</span><span class="sxs-lookup"><span data-stu-id="8e755-158">Possible values are: `productKey`, `licenseFile`.</span></span>|
|<span data-ttu-id="8e755-159">targetEdition</span><span class="sxs-lookup"><span data-stu-id="8e755-159">targetEdition</span></span>|[<span data-ttu-id="8e755-160">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="8e755-160">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="8e755-161">Zieledition von Edition Upgrade.</span><span class="sxs-lookup"><span data-stu-id="8e755-161">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="8e755-162">Mögliche Werte sind: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation` und `windows10ProfessionalWorkstationN`.</span><span class="sxs-lookup"><span data-stu-id="8e755-162">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.</span></span>|
|<span data-ttu-id="8e755-163">license</span><span class="sxs-lookup"><span data-stu-id="8e755-163">license</span></span>|<span data-ttu-id="8e755-164">String</span><span class="sxs-lookup"><span data-stu-id="8e755-164">String</span></span>|<span data-ttu-id="8e755-165">Inhalt der Edition Upgrade-Lizenzdatei</span><span class="sxs-lookup"><span data-stu-id="8e755-165">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="8e755-166">productKey</span><span class="sxs-lookup"><span data-stu-id="8e755-166">productKey</span></span>|<span data-ttu-id="8e755-167">String</span><span class="sxs-lookup"><span data-stu-id="8e755-167">String</span></span>|<span data-ttu-id="8e755-168">Product Key von Edition Upgrade</span><span class="sxs-lookup"><span data-stu-id="8e755-168">Edition Upgrade Product Key.</span></span>|



## <a name="response"></a><span data-ttu-id="8e755-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="8e755-169">Response</span></span>
<span data-ttu-id="8e755-170">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="8e755-170">If successful, this method returns a `200 OK` response code and an updated [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e755-171">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8e755-171">Example</span></span>
### <a name="request"></a><span data-ttu-id="8e755-172">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8e755-172">Request</span></span>
<span data-ttu-id="8e755-173">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8e755-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 311

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "licenseType": "licenseFile",
  "targetEdition": "windows10EnterpriseN",
  "license": "License value",
  "productKey": "Product Key value"
}
```

### <a name="response"></a><span data-ttu-id="8e755-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="8e755-174">Response</span></span>
<span data-ttu-id="8e755-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8e755-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 483

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "id": "f39fc471-c471-f39f-71c4-9ff371c49ff3",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "licenseType": "licenseFile",
  "targetEdition": "windows10EnterpriseN",
  "license": "License value",
  "productKey": "Product Key value"
}
```



