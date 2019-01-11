---
title: Aktualisieren von „windows10EnterpriseModernAppManagementConfiguration“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs windows10EnterpriseModernAppManagementConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5a6e545609c6b2e102b959d3d605d1d57dd3b609
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869027"
---
# <a name="update-windows10enterprisemodernappmanagementconfiguration"></a><span data-ttu-id="80a80-103">Aktualisieren von „windows10EnterpriseModernAppManagementConfiguration“</span><span class="sxs-lookup"><span data-stu-id="80a80-103">Update windows10EnterpriseModernAppManagementConfiguration</span></span>

> <span data-ttu-id="80a80-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="80a80-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="80a80-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="80a80-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="80a80-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="80a80-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="80a80-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80a80-107">Update the properties of a [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="80a80-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="80a80-108">Prerequisites</span></span>
<span data-ttu-id="80a80-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80a80-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80a80-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="80a80-111">Permission type</span></span>|<span data-ttu-id="80a80-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="80a80-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80a80-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="80a80-113">Delegated (work or school account)</span></span>|<span data-ttu-id="80a80-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80a80-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="80a80-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="80a80-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80a80-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="80a80-116">Not supported.</span></span>|
|<span data-ttu-id="80a80-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="80a80-117">Application</span></span>|<span data-ttu-id="80a80-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="80a80-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="80a80-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="80a80-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="80a80-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="80a80-120">Request headers</span></span>
|<span data-ttu-id="80a80-121">Header</span><span class="sxs-lookup"><span data-stu-id="80a80-121">Header</span></span>|<span data-ttu-id="80a80-122">Wert</span><span class="sxs-lookup"><span data-stu-id="80a80-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80a80-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="80a80-123">Authorization</span></span>|<span data-ttu-id="80a80-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="80a80-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80a80-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="80a80-125">Accept</span></span>|<span data-ttu-id="80a80-126">application/json</span><span class="sxs-lookup"><span data-stu-id="80a80-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80a80-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="80a80-127">Request body</span></span>
<span data-ttu-id="80a80-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="80a80-128">In the request body, supply a JSON representation for the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>

<span data-ttu-id="80a80-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="80a80-129">The following table shows the properties that are required when you create the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span></span>

|<span data-ttu-id="80a80-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="80a80-130">Property</span></span>|<span data-ttu-id="80a80-131">Typ</span><span class="sxs-lookup"><span data-stu-id="80a80-131">Type</span></span>|<span data-ttu-id="80a80-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="80a80-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80a80-133">id</span><span class="sxs-lookup"><span data-stu-id="80a80-133">id</span></span>|<span data-ttu-id="80a80-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80a80-134">String</span></span>|<span data-ttu-id="80a80-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="80a80-135">Key of the entity.</span></span> <span data-ttu-id="80a80-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80a80-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80a80-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="80a80-137">lastModifiedDateTime</span></span>|<span data-ttu-id="80a80-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80a80-138">DateTimeOffset</span></span>|<span data-ttu-id="80a80-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="80a80-139">DateTime the object was last modified.</span></span> <span data-ttu-id="80a80-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80a80-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80a80-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="80a80-141">roleScopeTagIds</span></span>|<span data-ttu-id="80a80-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="80a80-142">String collection</span></span>|<span data-ttu-id="80a80-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="80a80-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="80a80-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80a80-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80a80-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="80a80-145">supportsScopeTags</span></span>|<span data-ttu-id="80a80-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="80a80-146">Boolean</span></span>|<span data-ttu-id="80a80-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="80a80-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="80a80-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="80a80-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="80a80-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="80a80-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="80a80-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="80a80-150">This property is read-only.</span></span> <span data-ttu-id="80a80-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80a80-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80a80-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="80a80-152">createdDateTime</span></span>|<span data-ttu-id="80a80-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80a80-153">DateTimeOffset</span></span>|<span data-ttu-id="80a80-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="80a80-154">DateTime the object was created.</span></span> <span data-ttu-id="80a80-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80a80-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80a80-156">description</span><span class="sxs-lookup"><span data-stu-id="80a80-156">description</span></span>|<span data-ttu-id="80a80-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80a80-157">String</span></span>|<span data-ttu-id="80a80-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="80a80-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="80a80-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80a80-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80a80-160">displayName</span><span class="sxs-lookup"><span data-stu-id="80a80-160">displayName</span></span>|<span data-ttu-id="80a80-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80a80-161">String</span></span>|<span data-ttu-id="80a80-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="80a80-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="80a80-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80a80-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80a80-164">Version</span><span class="sxs-lookup"><span data-stu-id="80a80-164">version</span></span>|<span data-ttu-id="80a80-165">Int32</span><span class="sxs-lookup"><span data-stu-id="80a80-165">Int32</span></span>|<span data-ttu-id="80a80-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="80a80-166">Version of the device configuration.</span></span> <span data-ttu-id="80a80-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80a80-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80a80-168">uninstallBuiltInApps</span><span class="sxs-lookup"><span data-stu-id="80a80-168">uninstallBuiltInApps</span></span>|<span data-ttu-id="80a80-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="80a80-169">Boolean</span></span>|<span data-ttu-id="80a80-170">Gibt an, ob eine festgelegte Liste integrierter Windows-Apps deinstalliert werden soll.</span><span class="sxs-lookup"><span data-stu-id="80a80-170">Indicates whether or not to uninstall a fixed list of built-in Windows apps.</span></span>|



## <a name="response"></a><span data-ttu-id="80a80-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="80a80-171">Response</span></span>
<span data-ttu-id="80a80-172">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="80a80-172">If successful, this method returns a `200 OK` response code and an updated [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80a80-173">Beispiel</span><span class="sxs-lookup"><span data-stu-id="80a80-173">Example</span></span>
### <a name="request"></a><span data-ttu-id="80a80-174">Anforderung</span><span class="sxs-lookup"><span data-stu-id="80a80-174">Request</span></span>
<span data-ttu-id="80a80-175">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="80a80-175">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 288

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "uninstallBuiltInApps": true
}
```

### <a name="response"></a><span data-ttu-id="80a80-176">Antwort</span><span class="sxs-lookup"><span data-stu-id="80a80-176">Response</span></span>
<span data-ttu-id="80a80-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="80a80-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 486

{
  "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
  "id": "d6577687-7687-d657-8776-57d6877657d6",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "uninstallBuiltInApps": true
}
```





