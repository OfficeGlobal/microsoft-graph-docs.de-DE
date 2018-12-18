---
title: Erstellen von „editionUpgradeConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs editionUpgradeConfiguration.
author: tfitzmac
ms.openlocfilehash: 9ea7bb6206b882f81cad3cfd62419dc887f04898
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332739"
---
# <a name="create-editionupgradeconfiguration"></a><span data-ttu-id="cbc97-103">Erstellen von „editionUpgradeConfiguration“</span><span class="sxs-lookup"><span data-stu-id="cbc97-103">Create editionUpgradeConfiguration</span></span>

> <span data-ttu-id="cbc97-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="cbc97-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cbc97-105">Diese Methode erstellt ein neues Objekt des Typs [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cbc97-105">Create a new [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cbc97-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="cbc97-106">Prerequisites</span></span>
<span data-ttu-id="cbc97-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cbc97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbc97-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cbc97-109">Permission type</span></span>|<span data-ttu-id="cbc97-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cbc97-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cbc97-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cbc97-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cbc97-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbc97-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cbc97-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cbc97-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cbc97-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cbc97-114">Not supported.</span></span>|
|<span data-ttu-id="cbc97-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cbc97-115">Application</span></span>|<span data-ttu-id="cbc97-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cbc97-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cbc97-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cbc97-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="cbc97-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cbc97-118">Request headers</span></span>
|<span data-ttu-id="cbc97-119">Header</span><span class="sxs-lookup"><span data-stu-id="cbc97-119">Header</span></span>|<span data-ttu-id="cbc97-120">Wert</span><span class="sxs-lookup"><span data-stu-id="cbc97-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cbc97-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="cbc97-121">Authorization</span></span>|<span data-ttu-id="cbc97-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="cbc97-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cbc97-123">Accept</span><span class="sxs-lookup"><span data-stu-id="cbc97-123">Accept</span></span>|<span data-ttu-id="cbc97-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cbc97-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbc97-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cbc97-125">Request body</span></span>
<span data-ttu-id="cbc97-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „editionUpgradeConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="cbc97-126">In the request body, supply a JSON representation for the editionUpgradeConfiguration object.</span></span>

<span data-ttu-id="cbc97-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „editionUpgradeConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="cbc97-127">The following table shows the properties that are required when you create the editionUpgradeConfiguration.</span></span>

|<span data-ttu-id="cbc97-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cbc97-128">Property</span></span>|<span data-ttu-id="cbc97-129">Typ</span><span class="sxs-lookup"><span data-stu-id="cbc97-129">Type</span></span>|<span data-ttu-id="cbc97-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cbc97-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cbc97-131">id</span><span class="sxs-lookup"><span data-stu-id="cbc97-131">id</span></span>|<span data-ttu-id="cbc97-132">String</span><span class="sxs-lookup"><span data-stu-id="cbc97-132">String</span></span>|<span data-ttu-id="cbc97-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="cbc97-133">Key of the entity.</span></span> <span data-ttu-id="cbc97-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cbc97-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cbc97-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cbc97-135">lastModifiedDateTime</span></span>|<span data-ttu-id="cbc97-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cbc97-136">DateTimeOffset</span></span>|<span data-ttu-id="cbc97-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="cbc97-137">DateTime the object was last modified.</span></span> <span data-ttu-id="cbc97-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cbc97-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cbc97-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cbc97-139">createdDateTime</span></span>|<span data-ttu-id="cbc97-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cbc97-140">DateTimeOffset</span></span>|<span data-ttu-id="cbc97-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="cbc97-141">DateTime the object was created.</span></span> <span data-ttu-id="cbc97-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cbc97-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cbc97-143">description</span><span class="sxs-lookup"><span data-stu-id="cbc97-143">description</span></span>|<span data-ttu-id="cbc97-144">String</span><span class="sxs-lookup"><span data-stu-id="cbc97-144">String</span></span>|<span data-ttu-id="cbc97-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="cbc97-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cbc97-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cbc97-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cbc97-147">displayName</span><span class="sxs-lookup"><span data-stu-id="cbc97-147">displayName</span></span>|<span data-ttu-id="cbc97-148">String</span><span class="sxs-lookup"><span data-stu-id="cbc97-148">String</span></span>|<span data-ttu-id="cbc97-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="cbc97-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cbc97-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cbc97-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cbc97-151">Version</span><span class="sxs-lookup"><span data-stu-id="cbc97-151">version</span></span>|<span data-ttu-id="cbc97-152">Int32</span><span class="sxs-lookup"><span data-stu-id="cbc97-152">Int32</span></span>|<span data-ttu-id="cbc97-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="cbc97-153">Version of the device configuration.</span></span> <span data-ttu-id="cbc97-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cbc97-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cbc97-155">licenseType</span><span class="sxs-lookup"><span data-stu-id="cbc97-155">licenseType</span></span>|[<span data-ttu-id="cbc97-156">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="cbc97-156">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="cbc97-157">Typ der Edition Upgrade-Lizenz.</span><span class="sxs-lookup"><span data-stu-id="cbc97-157">Edition Upgrade License Type.</span></span> <span data-ttu-id="cbc97-158">Mögliche Werte sind: `productKey` und `licenseFile`.</span><span class="sxs-lookup"><span data-stu-id="cbc97-158">Possible values are: `productKey`, `licenseFile`.</span></span>|
|<span data-ttu-id="cbc97-159">targetEdition</span><span class="sxs-lookup"><span data-stu-id="cbc97-159">targetEdition</span></span>|[<span data-ttu-id="cbc97-160">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="cbc97-160">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="cbc97-161">Zieledition von Edition Upgrade.</span><span class="sxs-lookup"><span data-stu-id="cbc97-161">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="cbc97-162">Mögliche Werte sind: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation` und `windows10ProfessionalWorkstationN`.</span><span class="sxs-lookup"><span data-stu-id="cbc97-162">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.</span></span>|
|<span data-ttu-id="cbc97-163">license</span><span class="sxs-lookup"><span data-stu-id="cbc97-163">license</span></span>|<span data-ttu-id="cbc97-164">String</span><span class="sxs-lookup"><span data-stu-id="cbc97-164">String</span></span>|<span data-ttu-id="cbc97-165">Inhalt der Edition Upgrade-Lizenzdatei</span><span class="sxs-lookup"><span data-stu-id="cbc97-165">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="cbc97-166">productKey</span><span class="sxs-lookup"><span data-stu-id="cbc97-166">productKey</span></span>|<span data-ttu-id="cbc97-167">String</span><span class="sxs-lookup"><span data-stu-id="cbc97-167">String</span></span>|<span data-ttu-id="cbc97-168">Product Key von Edition Upgrade</span><span class="sxs-lookup"><span data-stu-id="cbc97-168">Edition Upgrade Product Key.</span></span>|



## <a name="response"></a><span data-ttu-id="cbc97-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="cbc97-169">Response</span></span>
<span data-ttu-id="cbc97-170">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="cbc97-170">If successful, this method returns a `201 Created` response code and a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbc97-171">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cbc97-171">Example</span></span>
### <a name="request"></a><span data-ttu-id="cbc97-172">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cbc97-172">Request</span></span>
<span data-ttu-id="cbc97-173">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cbc97-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="cbc97-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="cbc97-174">Response</span></span>
<span data-ttu-id="cbc97-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cbc97-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



