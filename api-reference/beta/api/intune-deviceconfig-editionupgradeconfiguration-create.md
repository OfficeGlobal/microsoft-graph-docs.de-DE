---
title: Erstellen von „editionUpgradeConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs editionUpgradeConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e18b8d9438da649cec250063913afffb47db1bf2
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30974426"
---
# <a name="create-editionupgradeconfiguration"></a><span data-ttu-id="70cf5-103">Erstellen von „editionUpgradeConfiguration“</span><span class="sxs-lookup"><span data-stu-id="70cf5-103">Create editionUpgradeConfiguration</span></span>

> <span data-ttu-id="70cf5-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="70cf5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="70cf5-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="70cf5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70cf5-106">Diese Methode erstellt ein neues Objekt des Typs [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70cf5-106">Create a new [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="70cf5-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="70cf5-107">Prerequisites</span></span>
<span data-ttu-id="70cf5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70cf5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70cf5-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="70cf5-110">Permission type</span></span>|<span data-ttu-id="70cf5-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="70cf5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70cf5-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="70cf5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="70cf5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70cf5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="70cf5-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="70cf5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70cf5-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="70cf5-115">Not supported.</span></span>|
|<span data-ttu-id="70cf5-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="70cf5-116">Application</span></span>|<span data-ttu-id="70cf5-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="70cf5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="70cf5-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="70cf5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="70cf5-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="70cf5-119">Request headers</span></span>
|<span data-ttu-id="70cf5-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="70cf5-120">Header</span></span>|<span data-ttu-id="70cf5-121">Wert</span><span class="sxs-lookup"><span data-stu-id="70cf5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70cf5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="70cf5-122">Authorization</span></span>|<span data-ttu-id="70cf5-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="70cf5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70cf5-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="70cf5-124">Accept</span></span>|<span data-ttu-id="70cf5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="70cf5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70cf5-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="70cf5-126">Request body</span></span>
<span data-ttu-id="70cf5-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „editionUpgradeConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="70cf5-127">In the request body, supply a JSON representation for the editionUpgradeConfiguration object.</span></span>

<span data-ttu-id="70cf5-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „editionUpgradeConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="70cf5-128">The following table shows the properties that are required when you create the editionUpgradeConfiguration.</span></span>

|<span data-ttu-id="70cf5-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="70cf5-129">Property</span></span>|<span data-ttu-id="70cf5-130">Typ</span><span class="sxs-lookup"><span data-stu-id="70cf5-130">Type</span></span>|<span data-ttu-id="70cf5-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="70cf5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70cf5-132">id</span><span class="sxs-lookup"><span data-stu-id="70cf5-132">id</span></span>|<span data-ttu-id="70cf5-133">String</span><span class="sxs-lookup"><span data-stu-id="70cf5-133">String</span></span>|<span data-ttu-id="70cf5-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="70cf5-134">Key of the entity.</span></span> <span data-ttu-id="70cf5-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70cf5-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70cf5-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="70cf5-136">lastModifiedDateTime</span></span>|<span data-ttu-id="70cf5-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70cf5-137">DateTimeOffset</span></span>|<span data-ttu-id="70cf5-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="70cf5-138">DateTime the object was last modified.</span></span> <span data-ttu-id="70cf5-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70cf5-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70cf5-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="70cf5-140">roleScopeTagIds</span></span>|<span data-ttu-id="70cf5-141">String collection</span><span class="sxs-lookup"><span data-stu-id="70cf5-141">String collection</span></span>|<span data-ttu-id="70cf5-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="70cf5-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="70cf5-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70cf5-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70cf5-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="70cf5-144">supportsScopeTags</span></span>|<span data-ttu-id="70cf5-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="70cf5-145">Boolean</span></span>|<span data-ttu-id="70cf5-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="70cf5-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="70cf5-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="70cf5-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="70cf5-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="70cf5-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="70cf5-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="70cf5-149">This property is read-only.</span></span> <span data-ttu-id="70cf5-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70cf5-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70cf5-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="70cf5-151">createdDateTime</span></span>|<span data-ttu-id="70cf5-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70cf5-152">DateTimeOffset</span></span>|<span data-ttu-id="70cf5-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="70cf5-153">DateTime the object was created.</span></span> <span data-ttu-id="70cf5-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70cf5-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70cf5-155">description</span><span class="sxs-lookup"><span data-stu-id="70cf5-155">description</span></span>|<span data-ttu-id="70cf5-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="70cf5-156">String</span></span>|<span data-ttu-id="70cf5-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="70cf5-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="70cf5-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70cf5-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70cf5-159">displayName</span><span class="sxs-lookup"><span data-stu-id="70cf5-159">displayName</span></span>|<span data-ttu-id="70cf5-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="70cf5-160">String</span></span>|<span data-ttu-id="70cf5-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="70cf5-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="70cf5-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="70cf5-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70cf5-163">Version</span><span class="sxs-lookup"><span data-stu-id="70cf5-163">version</span></span>|<span data-ttu-id="70cf5-164">Int32</span><span class="sxs-lookup"><span data-stu-id="70cf5-164">Int32</span></span>|<span data-ttu-id="70cf5-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="70cf5-165">Version of the device configuration.</span></span> <span data-ttu-id="70cf5-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70cf5-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70cf5-167">licenseType</span><span class="sxs-lookup"><span data-stu-id="70cf5-167">licenseType</span></span>|[<span data-ttu-id="70cf5-168">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="70cf5-168">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="70cf5-169">Typ der Edition Upgrade-Lizenz.</span><span class="sxs-lookup"><span data-stu-id="70cf5-169">Edition Upgrade License Type.</span></span> <span data-ttu-id="70cf5-170">Mögliche Werte sind: `productKey`, `licenseFile` und `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="70cf5-170">Possible values are: `productKey`, `licenseFile`, `notConfigured`.</span></span>|
|<span data-ttu-id="70cf5-171">targetEdition</span><span class="sxs-lookup"><span data-stu-id="70cf5-171">targetEdition</span></span>|[<span data-ttu-id="70cf5-172">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="70cf5-172">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="70cf5-173">Zieledition von Edition Upgrade.</span><span class="sxs-lookup"><span data-stu-id="70cf5-173">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="70cf5-174">Mögliche Werte: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="70cf5-174">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`.</span></span>|
|<span data-ttu-id="70cf5-175">license</span><span class="sxs-lookup"><span data-stu-id="70cf5-175">license</span></span>|<span data-ttu-id="70cf5-176">String</span><span class="sxs-lookup"><span data-stu-id="70cf5-176">String</span></span>|<span data-ttu-id="70cf5-177">Inhalt der Edition Upgrade-Lizenzdatei</span><span class="sxs-lookup"><span data-stu-id="70cf5-177">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="70cf5-178">productKey</span><span class="sxs-lookup"><span data-stu-id="70cf5-178">productKey</span></span>|<span data-ttu-id="70cf5-179">String</span><span class="sxs-lookup"><span data-stu-id="70cf5-179">String</span></span>|<span data-ttu-id="70cf5-180">Product Key von Edition Upgrade</span><span class="sxs-lookup"><span data-stu-id="70cf5-180">Edition Upgrade Product Key.</span></span>|
|<span data-ttu-id="70cf5-181">windowsSMode</span><span class="sxs-lookup"><span data-stu-id="70cf5-181">windowsSMode</span></span>|[<span data-ttu-id="70cf5-182">windowsSModeConfiguration</span><span class="sxs-lookup"><span data-stu-id="70cf5-182">windowsSModeConfiguration</span></span>](../resources/intune-deviceconfig-windowssmodeconfiguration.md)|<span data-ttu-id="70cf5-183">Konfiguration des S-Modus.</span><span class="sxs-lookup"><span data-stu-id="70cf5-183">S mode configuration.</span></span> <span data-ttu-id="70cf5-184">Mögliche Werte sind: `noRestriction`, `block` und `unlock`.</span><span class="sxs-lookup"><span data-stu-id="70cf5-184">Possible values are: `noRestriction`, `block`, `unlock`.</span></span>|



## <a name="response"></a><span data-ttu-id="70cf5-185">Antwort</span><span class="sxs-lookup"><span data-stu-id="70cf5-185">Response</span></span>
<span data-ttu-id="70cf5-186">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="70cf5-186">If successful, this method returns a `201 Created` response code and a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70cf5-187">Beispiel</span><span class="sxs-lookup"><span data-stu-id="70cf5-187">Example</span></span>

### <a name="request"></a><span data-ttu-id="70cf5-188">Anforderung</span><span class="sxs-lookup"><span data-stu-id="70cf5-188">Request</span></span>
<span data-ttu-id="70cf5-189">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="70cf5-189">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 431

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "licenseType": "licenseFile",
  "targetEdition": "windows10EnterpriseN",
  "license": "License value",
  "productKey": "Product Key value",
  "windowsSMode": "block"
}
```

### <a name="response"></a><span data-ttu-id="70cf5-190">Antwort</span><span class="sxs-lookup"><span data-stu-id="70cf5-190">Response</span></span>
<span data-ttu-id="70cf5-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="70cf5-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 603

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "id": "f39fc471-c471-f39f-71c4-9ff371c49ff3",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "licenseType": "licenseFile",
  "targetEdition": "windows10EnterpriseN",
  "license": "License value",
  "productKey": "Product Key value",
  "windowsSMode": "block"
}
```




