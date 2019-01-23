---
title: Erstellen von „editionUpgradeConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs editionUpgradeConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 67a86f00fb8160d9226de0343b21230977523ef2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421242"
---
# <a name="create-editionupgradeconfiguration"></a><span data-ttu-id="2e58c-103">Erstellen von „editionUpgradeConfiguration“</span><span class="sxs-lookup"><span data-stu-id="2e58c-103">Create editionUpgradeConfiguration</span></span>

> <span data-ttu-id="2e58c-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="2e58c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2e58c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2e58c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2e58c-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2e58c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e58c-107">Diese Methode erstellt ein neues Objekt des Typs [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2e58c-107">Create a new [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2e58c-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2e58c-108">Prerequisites</span></span>
<span data-ttu-id="2e58c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2e58c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2e58c-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2e58c-111">Permission type</span></span>|<span data-ttu-id="2e58c-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2e58c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e58c-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2e58c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2e58c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e58c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2e58c-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2e58c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e58c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2e58c-116">Not supported.</span></span>|
|<span data-ttu-id="2e58c-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2e58c-117">Application</span></span>|<span data-ttu-id="2e58c-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2e58c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e58c-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2e58c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2e58c-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2e58c-120">Request headers</span></span>
|<span data-ttu-id="2e58c-121">Header</span><span class="sxs-lookup"><span data-stu-id="2e58c-121">Header</span></span>|<span data-ttu-id="2e58c-122">Wert</span><span class="sxs-lookup"><span data-stu-id="2e58c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e58c-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="2e58c-123">Authorization</span></span>|<span data-ttu-id="2e58c-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2e58c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e58c-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2e58c-125">Accept</span></span>|<span data-ttu-id="2e58c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2e58c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e58c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2e58c-127">Request body</span></span>
<span data-ttu-id="2e58c-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „editionUpgradeConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="2e58c-128">In the request body, supply a JSON representation for the editionUpgradeConfiguration object.</span></span>

<span data-ttu-id="2e58c-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „editionUpgradeConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="2e58c-129">The following table shows the properties that are required when you create the editionUpgradeConfiguration.</span></span>

|<span data-ttu-id="2e58c-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2e58c-130">Property</span></span>|<span data-ttu-id="2e58c-131">Typ</span><span class="sxs-lookup"><span data-stu-id="2e58c-131">Type</span></span>|<span data-ttu-id="2e58c-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2e58c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e58c-133">id</span><span class="sxs-lookup"><span data-stu-id="2e58c-133">id</span></span>|<span data-ttu-id="2e58c-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2e58c-134">String</span></span>|<span data-ttu-id="2e58c-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="2e58c-135">Key of the entity.</span></span> <span data-ttu-id="2e58c-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2e58c-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2e58c-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2e58c-137">lastModifiedDateTime</span></span>|<span data-ttu-id="2e58c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e58c-138">DateTimeOffset</span></span>|<span data-ttu-id="2e58c-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="2e58c-139">DateTime the object was last modified.</span></span> <span data-ttu-id="2e58c-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2e58c-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2e58c-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2e58c-141">roleScopeTagIds</span></span>|<span data-ttu-id="2e58c-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="2e58c-142">String collection</span></span>|<span data-ttu-id="2e58c-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="2e58c-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2e58c-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2e58c-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2e58c-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2e58c-145">supportsScopeTags</span></span>|<span data-ttu-id="2e58c-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="2e58c-146">Boolean</span></span>|<span data-ttu-id="2e58c-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2e58c-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2e58c-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="2e58c-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2e58c-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="2e58c-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2e58c-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2e58c-150">This property is read-only.</span></span> <span data-ttu-id="2e58c-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2e58c-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2e58c-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2e58c-152">createdDateTime</span></span>|<span data-ttu-id="2e58c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e58c-153">DateTimeOffset</span></span>|<span data-ttu-id="2e58c-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="2e58c-154">DateTime the object was created.</span></span> <span data-ttu-id="2e58c-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2e58c-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2e58c-156">description</span><span class="sxs-lookup"><span data-stu-id="2e58c-156">description</span></span>|<span data-ttu-id="2e58c-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2e58c-157">String</span></span>|<span data-ttu-id="2e58c-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="2e58c-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2e58c-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2e58c-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2e58c-160">displayName</span><span class="sxs-lookup"><span data-stu-id="2e58c-160">displayName</span></span>|<span data-ttu-id="2e58c-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2e58c-161">String</span></span>|<span data-ttu-id="2e58c-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="2e58c-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2e58c-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2e58c-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2e58c-164">Version</span><span class="sxs-lookup"><span data-stu-id="2e58c-164">version</span></span>|<span data-ttu-id="2e58c-165">Int32</span><span class="sxs-lookup"><span data-stu-id="2e58c-165">Int32</span></span>|<span data-ttu-id="2e58c-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="2e58c-166">Version of the device configuration.</span></span> <span data-ttu-id="2e58c-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2e58c-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2e58c-168">licenseType</span><span class="sxs-lookup"><span data-stu-id="2e58c-168">licenseType</span></span>|[<span data-ttu-id="2e58c-169">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="2e58c-169">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="2e58c-170">Typ der Edition Upgrade-Lizenz.</span><span class="sxs-lookup"><span data-stu-id="2e58c-170">Edition Upgrade License Type.</span></span> <span data-ttu-id="2e58c-171">Mögliche Werte sind: `productKey`, `licenseFile` und `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="2e58c-171">Possible values are: `productKey`, `licenseFile`, `notConfigured`.</span></span>|
|<span data-ttu-id="2e58c-172">targetEdition</span><span class="sxs-lookup"><span data-stu-id="2e58c-172">targetEdition</span></span>|[<span data-ttu-id="2e58c-173">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="2e58c-173">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="2e58c-174">Zieledition von Edition Upgrade.</span><span class="sxs-lookup"><span data-stu-id="2e58c-174">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="2e58c-175">Mögliche Werte sind: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="2e58c-175">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`.</span></span>|
|<span data-ttu-id="2e58c-176">license</span><span class="sxs-lookup"><span data-stu-id="2e58c-176">license</span></span>|<span data-ttu-id="2e58c-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2e58c-177">String</span></span>|<span data-ttu-id="2e58c-178">Inhalt der Edition Upgrade-Lizenzdatei</span><span class="sxs-lookup"><span data-stu-id="2e58c-178">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="2e58c-179">productKey</span><span class="sxs-lookup"><span data-stu-id="2e58c-179">productKey</span></span>|<span data-ttu-id="2e58c-180">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2e58c-180">String</span></span>|<span data-ttu-id="2e58c-181">Product Key von Edition Upgrade</span><span class="sxs-lookup"><span data-stu-id="2e58c-181">Edition Upgrade Product Key.</span></span>|
|<span data-ttu-id="2e58c-182">windowsSMode</span><span class="sxs-lookup"><span data-stu-id="2e58c-182">windowsSMode</span></span>|[<span data-ttu-id="2e58c-183">windowsSModeConfiguration</span><span class="sxs-lookup"><span data-stu-id="2e58c-183">windowsSModeConfiguration</span></span>](../resources/intune-deviceconfig-windowssmodeconfiguration.md)|<span data-ttu-id="2e58c-184">S Modus Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="2e58c-184">S mode configuration.</span></span> <span data-ttu-id="2e58c-185">Mögliche Werte sind: `noRestriction`, `block` und `unlock`.</span><span class="sxs-lookup"><span data-stu-id="2e58c-185">Possible values are: `noRestriction`, `block`, `unlock`.</span></span>|



## <a name="response"></a><span data-ttu-id="2e58c-186">Antwort</span><span class="sxs-lookup"><span data-stu-id="2e58c-186">Response</span></span>
<span data-ttu-id="2e58c-187">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2e58c-187">If successful, this method returns a `201 Created` response code and a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e58c-188">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2e58c-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="2e58c-189">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2e58c-189">Request</span></span>
<span data-ttu-id="2e58c-190">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2e58c-190">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2e58c-191">Antwort</span><span class="sxs-lookup"><span data-stu-id="2e58c-191">Response</span></span>
<span data-ttu-id="2e58c-p114">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2e58c-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




