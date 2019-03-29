---
title: Aktualisieren von „windows10EnterpriseModernAppManagementConfiguration“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs windows10EnterpriseModernAppManagementConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 553b072a5fb42b1df8c2673f52225212ef6cc91e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30966313"
---
# <a name="update-windows10enterprisemodernappmanagementconfiguration"></a><span data-ttu-id="48107-103">Aktualisieren von „windows10EnterpriseModernAppManagementConfiguration“</span><span class="sxs-lookup"><span data-stu-id="48107-103">Update windows10EnterpriseModernAppManagementConfiguration</span></span>

> <span data-ttu-id="48107-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="48107-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="48107-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="48107-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48107-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="48107-106">Update the properties of a [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="48107-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="48107-107">Prerequisites</span></span>
<span data-ttu-id="48107-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48107-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48107-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="48107-110">Permission type</span></span>|<span data-ttu-id="48107-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="48107-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48107-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="48107-112">Delegated (work or school account)</span></span>|<span data-ttu-id="48107-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48107-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="48107-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="48107-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48107-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="48107-115">Not supported.</span></span>|
|<span data-ttu-id="48107-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="48107-116">Application</span></span>|<span data-ttu-id="48107-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="48107-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="48107-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="48107-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="48107-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="48107-119">Request headers</span></span>
|<span data-ttu-id="48107-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="48107-120">Header</span></span>|<span data-ttu-id="48107-121">Wert</span><span class="sxs-lookup"><span data-stu-id="48107-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48107-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="48107-122">Authorization</span></span>|<span data-ttu-id="48107-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="48107-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48107-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="48107-124">Accept</span></span>|<span data-ttu-id="48107-125">application/json</span><span class="sxs-lookup"><span data-stu-id="48107-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48107-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="48107-126">Request body</span></span>
<span data-ttu-id="48107-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="48107-127">In the request body, supply a JSON representation for the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>

<span data-ttu-id="48107-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="48107-128">The following table shows the properties that are required when you create the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span></span>

|<span data-ttu-id="48107-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="48107-129">Property</span></span>|<span data-ttu-id="48107-130">Typ</span><span class="sxs-lookup"><span data-stu-id="48107-130">Type</span></span>|<span data-ttu-id="48107-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="48107-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48107-132">id</span><span class="sxs-lookup"><span data-stu-id="48107-132">id</span></span>|<span data-ttu-id="48107-133">String</span><span class="sxs-lookup"><span data-stu-id="48107-133">String</span></span>|<span data-ttu-id="48107-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="48107-134">Key of the entity.</span></span> <span data-ttu-id="48107-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="48107-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48107-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="48107-136">lastModifiedDateTime</span></span>|<span data-ttu-id="48107-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48107-137">DateTimeOffset</span></span>|<span data-ttu-id="48107-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="48107-138">DateTime the object was last modified.</span></span> <span data-ttu-id="48107-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="48107-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48107-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="48107-140">roleScopeTagIds</span></span>|<span data-ttu-id="48107-141">String collection</span><span class="sxs-lookup"><span data-stu-id="48107-141">String collection</span></span>|<span data-ttu-id="48107-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="48107-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="48107-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="48107-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48107-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="48107-144">supportsScopeTags</span></span>|<span data-ttu-id="48107-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="48107-145">Boolean</span></span>|<span data-ttu-id="48107-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="48107-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="48107-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="48107-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="48107-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="48107-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="48107-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="48107-149">This property is read-only.</span></span> <span data-ttu-id="48107-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="48107-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48107-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="48107-151">createdDateTime</span></span>|<span data-ttu-id="48107-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48107-152">DateTimeOffset</span></span>|<span data-ttu-id="48107-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="48107-153">DateTime the object was created.</span></span> <span data-ttu-id="48107-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="48107-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48107-155">description</span><span class="sxs-lookup"><span data-stu-id="48107-155">description</span></span>|<span data-ttu-id="48107-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="48107-156">String</span></span>|<span data-ttu-id="48107-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="48107-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="48107-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="48107-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48107-159">displayName</span><span class="sxs-lookup"><span data-stu-id="48107-159">displayName</span></span>|<span data-ttu-id="48107-160">String</span><span class="sxs-lookup"><span data-stu-id="48107-160">String</span></span>|<span data-ttu-id="48107-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="48107-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="48107-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="48107-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48107-163">Version</span><span class="sxs-lookup"><span data-stu-id="48107-163">version</span></span>|<span data-ttu-id="48107-164">Int32</span><span class="sxs-lookup"><span data-stu-id="48107-164">Int32</span></span>|<span data-ttu-id="48107-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="48107-165">Version of the device configuration.</span></span> <span data-ttu-id="48107-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="48107-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48107-167">uninstallBuiltInApps</span><span class="sxs-lookup"><span data-stu-id="48107-167">uninstallBuiltInApps</span></span>|<span data-ttu-id="48107-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="48107-168">Boolean</span></span>|<span data-ttu-id="48107-169">Gibt an, ob eine festgelegte Liste integrierter Windows-Apps deinstalliert werden soll.</span><span class="sxs-lookup"><span data-stu-id="48107-169">Indicates whether or not to uninstall a fixed list of built-in Windows apps.</span></span>|



## <a name="response"></a><span data-ttu-id="48107-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="48107-170">Response</span></span>
<span data-ttu-id="48107-171">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="48107-171">If successful, this method returns a `200 OK` response code and an updated [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48107-172">Beispiel</span><span class="sxs-lookup"><span data-stu-id="48107-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="48107-173">Anforderung</span><span class="sxs-lookup"><span data-stu-id="48107-173">Request</span></span>
<span data-ttu-id="48107-174">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="48107-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 314

{
  "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
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

### <a name="response"></a><span data-ttu-id="48107-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="48107-175">Response</span></span>
<span data-ttu-id="48107-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="48107-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




