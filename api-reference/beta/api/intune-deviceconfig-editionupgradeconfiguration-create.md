---
title: Erstellen von „editionUpgradeConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs editionUpgradeConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 60694b4aa97b5b57c1dcb5ee15da7ba92350d2a6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939455"
---
# <a name="create-editionupgradeconfiguration"></a><span data-ttu-id="50177-103">Erstellen von „editionUpgradeConfiguration“</span><span class="sxs-lookup"><span data-stu-id="50177-103">Create editionUpgradeConfiguration</span></span>

> <span data-ttu-id="50177-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="50177-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="50177-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="50177-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="50177-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="50177-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="50177-107">Diese Methode erstellt ein neues Objekt des Typs [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50177-107">Create a new [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="50177-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="50177-108">Prerequisites</span></span>
<span data-ttu-id="50177-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50177-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50177-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="50177-111">Permission type</span></span>|<span data-ttu-id="50177-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="50177-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50177-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="50177-113">Delegated (work or school account)</span></span>|<span data-ttu-id="50177-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50177-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="50177-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="50177-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50177-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="50177-116">Not supported.</span></span>|
|<span data-ttu-id="50177-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="50177-117">Application</span></span>|<span data-ttu-id="50177-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="50177-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50177-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="50177-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="50177-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="50177-120">Request headers</span></span>
|<span data-ttu-id="50177-121">Header</span><span class="sxs-lookup"><span data-stu-id="50177-121">Header</span></span>|<span data-ttu-id="50177-122">Wert</span><span class="sxs-lookup"><span data-stu-id="50177-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50177-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="50177-123">Authorization</span></span>|<span data-ttu-id="50177-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="50177-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50177-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="50177-125">Accept</span></span>|<span data-ttu-id="50177-126">application/json</span><span class="sxs-lookup"><span data-stu-id="50177-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50177-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="50177-127">Request body</span></span>
<span data-ttu-id="50177-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „editionUpgradeConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="50177-128">In the request body, supply a JSON representation for the editionUpgradeConfiguration object.</span></span>

<span data-ttu-id="50177-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „editionUpgradeConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="50177-129">The following table shows the properties that are required when you create the editionUpgradeConfiguration.</span></span>

|<span data-ttu-id="50177-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="50177-130">Property</span></span>|<span data-ttu-id="50177-131">Typ</span><span class="sxs-lookup"><span data-stu-id="50177-131">Type</span></span>|<span data-ttu-id="50177-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="50177-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50177-133">id</span><span class="sxs-lookup"><span data-stu-id="50177-133">id</span></span>|<span data-ttu-id="50177-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="50177-134">String</span></span>|<span data-ttu-id="50177-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="50177-135">Key of the entity.</span></span> <span data-ttu-id="50177-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50177-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50177-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="50177-137">lastModifiedDateTime</span></span>|<span data-ttu-id="50177-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50177-138">DateTimeOffset</span></span>|<span data-ttu-id="50177-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="50177-139">DateTime the object was last modified.</span></span> <span data-ttu-id="50177-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50177-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50177-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="50177-141">roleScopeTagIds</span></span>|<span data-ttu-id="50177-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="50177-142">String collection</span></span>|<span data-ttu-id="50177-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="50177-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="50177-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50177-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50177-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="50177-145">supportsScopeTags</span></span>|<span data-ttu-id="50177-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="50177-146">Boolean</span></span>|<span data-ttu-id="50177-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="50177-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="50177-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="50177-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="50177-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="50177-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="50177-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="50177-150">This property is read-only.</span></span> <span data-ttu-id="50177-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50177-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50177-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="50177-152">createdDateTime</span></span>|<span data-ttu-id="50177-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50177-153">DateTimeOffset</span></span>|<span data-ttu-id="50177-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="50177-154">DateTime the object was created.</span></span> <span data-ttu-id="50177-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50177-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50177-156">description</span><span class="sxs-lookup"><span data-stu-id="50177-156">description</span></span>|<span data-ttu-id="50177-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="50177-157">String</span></span>|<span data-ttu-id="50177-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="50177-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="50177-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50177-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50177-160">displayName</span><span class="sxs-lookup"><span data-stu-id="50177-160">displayName</span></span>|<span data-ttu-id="50177-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="50177-161">String</span></span>|<span data-ttu-id="50177-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="50177-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="50177-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50177-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50177-164">Version</span><span class="sxs-lookup"><span data-stu-id="50177-164">version</span></span>|<span data-ttu-id="50177-165">Int32</span><span class="sxs-lookup"><span data-stu-id="50177-165">Int32</span></span>|<span data-ttu-id="50177-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="50177-166">Version of the device configuration.</span></span> <span data-ttu-id="50177-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50177-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50177-168">licenseType</span><span class="sxs-lookup"><span data-stu-id="50177-168">licenseType</span></span>|[<span data-ttu-id="50177-169">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="50177-169">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="50177-170">Typ der Edition Upgrade-Lizenz.</span><span class="sxs-lookup"><span data-stu-id="50177-170">Edition Upgrade License Type.</span></span> <span data-ttu-id="50177-171">Mögliche Werte sind: `productKey`, `licenseFile` und `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="50177-171">Possible values are: `productKey`, `licenseFile`, `notConfigured`.</span></span>|
|<span data-ttu-id="50177-172">targetEdition</span><span class="sxs-lookup"><span data-stu-id="50177-172">targetEdition</span></span>|[<span data-ttu-id="50177-173">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="50177-173">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="50177-174">Zieledition von Edition Upgrade.</span><span class="sxs-lookup"><span data-stu-id="50177-174">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="50177-175">Mögliche Werte sind: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="50177-175">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`.</span></span>|
|<span data-ttu-id="50177-176">license</span><span class="sxs-lookup"><span data-stu-id="50177-176">license</span></span>|<span data-ttu-id="50177-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="50177-177">String</span></span>|<span data-ttu-id="50177-178">Inhalt der Edition Upgrade-Lizenzdatei</span><span class="sxs-lookup"><span data-stu-id="50177-178">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="50177-179">productKey</span><span class="sxs-lookup"><span data-stu-id="50177-179">productKey</span></span>|<span data-ttu-id="50177-180">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="50177-180">String</span></span>|<span data-ttu-id="50177-181">Product Key von Edition Upgrade</span><span class="sxs-lookup"><span data-stu-id="50177-181">Edition Upgrade Product Key.</span></span>|
|<span data-ttu-id="50177-182">windowsSMode</span><span class="sxs-lookup"><span data-stu-id="50177-182">windowsSMode</span></span>|[<span data-ttu-id="50177-183">windowsSModeConfiguration</span><span class="sxs-lookup"><span data-stu-id="50177-183">windowsSModeConfiguration</span></span>](../resources/intune-deviceconfig-windowssmodeconfiguration.md)|<span data-ttu-id="50177-184">S Modus Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="50177-184">S mode configuration.</span></span> <span data-ttu-id="50177-185">Mögliche Werte sind: `noRestriction`, `block` und `unlock`.</span><span class="sxs-lookup"><span data-stu-id="50177-185">Possible values are: `noRestriction`, `block`, `unlock`.</span></span>|



## <a name="response"></a><span data-ttu-id="50177-186">Antwort</span><span class="sxs-lookup"><span data-stu-id="50177-186">Response</span></span>
<span data-ttu-id="50177-187">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="50177-187">If successful, this method returns a `201 Created` response code and a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50177-188">Beispiel</span><span class="sxs-lookup"><span data-stu-id="50177-188">Example</span></span>
### <a name="request"></a><span data-ttu-id="50177-189">Anforderung</span><span class="sxs-lookup"><span data-stu-id="50177-189">Request</span></span>
<span data-ttu-id="50177-190">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="50177-190">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 495

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="50177-191">Antwort</span><span class="sxs-lookup"><span data-stu-id="50177-191">Response</span></span>
<span data-ttu-id="50177-p114">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="50177-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





