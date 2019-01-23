---
title: Aktualisieren von „editionUpgradeConfiguration“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs editionUpgradeConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 870237a8b154e9adcc1ab4a60285230ffb94c01f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397925"
---
# <a name="update-editionupgradeconfiguration"></a><span data-ttu-id="bae91-103">Aktualisieren von „editionUpgradeConfiguration“</span><span class="sxs-lookup"><span data-stu-id="bae91-103">Update editionUpgradeConfiguration</span></span>

> <span data-ttu-id="bae91-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="bae91-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bae91-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bae91-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bae91-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bae91-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bae91-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bae91-107">Update the properties of a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bae91-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="bae91-108">Prerequisites</span></span>
<span data-ttu-id="bae91-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="bae91-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bae91-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bae91-111">Permission type</span></span>|<span data-ttu-id="bae91-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bae91-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bae91-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bae91-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bae91-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bae91-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bae91-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bae91-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bae91-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bae91-116">Not supported.</span></span>|
|<span data-ttu-id="bae91-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bae91-117">Application</span></span>|<span data-ttu-id="bae91-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bae91-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bae91-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bae91-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="bae91-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bae91-120">Request headers</span></span>
|<span data-ttu-id="bae91-121">Header</span><span class="sxs-lookup"><span data-stu-id="bae91-121">Header</span></span>|<span data-ttu-id="bae91-122">Wert</span><span class="sxs-lookup"><span data-stu-id="bae91-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bae91-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="bae91-123">Authorization</span></span>|<span data-ttu-id="bae91-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="bae91-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bae91-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="bae91-125">Accept</span></span>|<span data-ttu-id="bae91-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bae91-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bae91-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bae91-127">Request body</span></span>
<span data-ttu-id="bae91-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="bae91-128">In the request body, supply a JSON representation for the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

<span data-ttu-id="bae91-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="bae91-129">The following table shows the properties that are required when you create the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span></span>

|<span data-ttu-id="bae91-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bae91-130">Property</span></span>|<span data-ttu-id="bae91-131">Typ</span><span class="sxs-lookup"><span data-stu-id="bae91-131">Type</span></span>|<span data-ttu-id="bae91-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bae91-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bae91-133">id</span><span class="sxs-lookup"><span data-stu-id="bae91-133">id</span></span>|<span data-ttu-id="bae91-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bae91-134">String</span></span>|<span data-ttu-id="bae91-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="bae91-135">Key of the entity.</span></span> <span data-ttu-id="bae91-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bae91-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bae91-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bae91-137">lastModifiedDateTime</span></span>|<span data-ttu-id="bae91-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bae91-138">DateTimeOffset</span></span>|<span data-ttu-id="bae91-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="bae91-139">DateTime the object was last modified.</span></span> <span data-ttu-id="bae91-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bae91-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bae91-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bae91-141">roleScopeTagIds</span></span>|<span data-ttu-id="bae91-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="bae91-142">String collection</span></span>|<span data-ttu-id="bae91-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="bae91-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bae91-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bae91-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bae91-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="bae91-145">supportsScopeTags</span></span>|<span data-ttu-id="bae91-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="bae91-146">Boolean</span></span>|<span data-ttu-id="bae91-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bae91-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="bae91-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="bae91-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="bae91-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="bae91-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="bae91-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bae91-150">This property is read-only.</span></span> <span data-ttu-id="bae91-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bae91-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bae91-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bae91-152">createdDateTime</span></span>|<span data-ttu-id="bae91-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bae91-153">DateTimeOffset</span></span>|<span data-ttu-id="bae91-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="bae91-154">DateTime the object was created.</span></span> <span data-ttu-id="bae91-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bae91-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bae91-156">description</span><span class="sxs-lookup"><span data-stu-id="bae91-156">description</span></span>|<span data-ttu-id="bae91-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bae91-157">String</span></span>|<span data-ttu-id="bae91-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="bae91-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bae91-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bae91-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bae91-160">displayName</span><span class="sxs-lookup"><span data-stu-id="bae91-160">displayName</span></span>|<span data-ttu-id="bae91-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bae91-161">String</span></span>|<span data-ttu-id="bae91-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="bae91-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bae91-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bae91-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bae91-164">Version</span><span class="sxs-lookup"><span data-stu-id="bae91-164">version</span></span>|<span data-ttu-id="bae91-165">Int32</span><span class="sxs-lookup"><span data-stu-id="bae91-165">Int32</span></span>|<span data-ttu-id="bae91-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="bae91-166">Version of the device configuration.</span></span> <span data-ttu-id="bae91-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bae91-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bae91-168">licenseType</span><span class="sxs-lookup"><span data-stu-id="bae91-168">licenseType</span></span>|[<span data-ttu-id="bae91-169">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="bae91-169">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="bae91-170">Typ der Edition Upgrade-Lizenz.</span><span class="sxs-lookup"><span data-stu-id="bae91-170">Edition Upgrade License Type.</span></span> <span data-ttu-id="bae91-171">Mögliche Werte sind: `productKey`, `licenseFile` und `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="bae91-171">Possible values are: `productKey`, `licenseFile`, `notConfigured`.</span></span>|
|<span data-ttu-id="bae91-172">targetEdition</span><span class="sxs-lookup"><span data-stu-id="bae91-172">targetEdition</span></span>|[<span data-ttu-id="bae91-173">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="bae91-173">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="bae91-174">Zieledition von Edition Upgrade.</span><span class="sxs-lookup"><span data-stu-id="bae91-174">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="bae91-175">Mögliche Werte sind: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="bae91-175">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`.</span></span>|
|<span data-ttu-id="bae91-176">license</span><span class="sxs-lookup"><span data-stu-id="bae91-176">license</span></span>|<span data-ttu-id="bae91-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bae91-177">String</span></span>|<span data-ttu-id="bae91-178">Inhalt der Edition Upgrade-Lizenzdatei</span><span class="sxs-lookup"><span data-stu-id="bae91-178">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="bae91-179">productKey</span><span class="sxs-lookup"><span data-stu-id="bae91-179">productKey</span></span>|<span data-ttu-id="bae91-180">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bae91-180">String</span></span>|<span data-ttu-id="bae91-181">Product Key von Edition Upgrade</span><span class="sxs-lookup"><span data-stu-id="bae91-181">Edition Upgrade Product Key.</span></span>|
|<span data-ttu-id="bae91-182">windowsSMode</span><span class="sxs-lookup"><span data-stu-id="bae91-182">windowsSMode</span></span>|[<span data-ttu-id="bae91-183">windowsSModeConfiguration</span><span class="sxs-lookup"><span data-stu-id="bae91-183">windowsSModeConfiguration</span></span>](../resources/intune-deviceconfig-windowssmodeconfiguration.md)|<span data-ttu-id="bae91-184">S Modus Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="bae91-184">S mode configuration.</span></span> <span data-ttu-id="bae91-185">Mögliche Werte sind: `noRestriction`, `block` und `unlock`.</span><span class="sxs-lookup"><span data-stu-id="bae91-185">Possible values are: `noRestriction`, `block`, `unlock`.</span></span>|



## <a name="response"></a><span data-ttu-id="bae91-186">Antwort</span><span class="sxs-lookup"><span data-stu-id="bae91-186">Response</span></span>
<span data-ttu-id="bae91-187">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="bae91-187">If successful, this method returns a `200 OK` response code and an updated [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bae91-188">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bae91-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="bae91-189">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bae91-189">Request</span></span>
<span data-ttu-id="bae91-190">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bae91-190">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="bae91-191">Antwort</span><span class="sxs-lookup"><span data-stu-id="bae91-191">Response</span></span>
<span data-ttu-id="bae91-p114">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bae91-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




