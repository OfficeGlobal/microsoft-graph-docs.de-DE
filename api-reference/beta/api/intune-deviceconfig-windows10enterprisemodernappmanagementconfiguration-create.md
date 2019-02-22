---
title: Erstellen von „windows10EnterpriseModernAppManagementConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs windows10EnterpriseModernAppManagementConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bfa2ab6981c09e5fb9603185f9f1dfa77cbf7126
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161838"
---
# <a name="create-windows10enterprisemodernappmanagementconfiguration"></a><span data-ttu-id="eef3e-103">Erstellen von „windows10EnterpriseModernAppManagementConfiguration“</span><span class="sxs-lookup"><span data-stu-id="eef3e-103">Create windows10EnterpriseModernAppManagementConfiguration</span></span>

> <span data-ttu-id="eef3e-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="eef3e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eef3e-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="eef3e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eef3e-106">Diese Methode erstellt ein neues Objekt des Typs [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eef3e-106">Create a new [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eef3e-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="eef3e-107">Prerequisites</span></span>
<span data-ttu-id="eef3e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="eef3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="eef3e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="eef3e-110">Permission type</span></span>|<span data-ttu-id="eef3e-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="eef3e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eef3e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="eef3e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eef3e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eef3e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="eef3e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="eef3e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eef3e-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eef3e-115">Not supported.</span></span>|
|<span data-ttu-id="eef3e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="eef3e-116">Application</span></span>|<span data-ttu-id="eef3e-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eef3e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eef3e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="eef3e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="eef3e-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="eef3e-119">Request headers</span></span>
|<span data-ttu-id="eef3e-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="eef3e-120">Header</span></span>|<span data-ttu-id="eef3e-121">Wert</span><span class="sxs-lookup"><span data-stu-id="eef3e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eef3e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="eef3e-122">Authorization</span></span>|<span data-ttu-id="eef3e-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="eef3e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eef3e-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="eef3e-124">Accept</span></span>|<span data-ttu-id="eef3e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eef3e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eef3e-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="eef3e-126">Request body</span></span>
<span data-ttu-id="eef3e-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „windows10EnterpriseModernAppManagementConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="eef3e-127">In the request body, supply a JSON representation for the windows10EnterpriseModernAppManagementConfiguration object.</span></span>

<span data-ttu-id="eef3e-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „windows10EnterpriseModernAppManagementConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="eef3e-128">The following table shows the properties that are required when you create the windows10EnterpriseModernAppManagementConfiguration.</span></span>

|<span data-ttu-id="eef3e-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="eef3e-129">Property</span></span>|<span data-ttu-id="eef3e-130">Typ</span><span class="sxs-lookup"><span data-stu-id="eef3e-130">Type</span></span>|<span data-ttu-id="eef3e-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eef3e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eef3e-132">id</span><span class="sxs-lookup"><span data-stu-id="eef3e-132">id</span></span>|<span data-ttu-id="eef3e-133">string</span><span class="sxs-lookup"><span data-stu-id="eef3e-133">String</span></span>|<span data-ttu-id="eef3e-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="eef3e-134">Key of the entity.</span></span> <span data-ttu-id="eef3e-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eef3e-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eef3e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eef3e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="eef3e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eef3e-137">DateTimeOffset</span></span>|<span data-ttu-id="eef3e-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="eef3e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="eef3e-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eef3e-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eef3e-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="eef3e-140">roleScopeTagIds</span></span>|<span data-ttu-id="eef3e-141">String collection</span><span class="sxs-lookup"><span data-stu-id="eef3e-141">String collection</span></span>|<span data-ttu-id="eef3e-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="eef3e-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="eef3e-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eef3e-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eef3e-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="eef3e-144">supportsScopeTags</span></span>|<span data-ttu-id="eef3e-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="eef3e-145">Boolean</span></span>|<span data-ttu-id="eef3e-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="eef3e-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="eef3e-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="eef3e-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="eef3e-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="eef3e-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="eef3e-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="eef3e-149">This property is read-only.</span></span> <span data-ttu-id="eef3e-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eef3e-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eef3e-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eef3e-151">createdDateTime</span></span>|<span data-ttu-id="eef3e-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eef3e-152">DateTimeOffset</span></span>|<span data-ttu-id="eef3e-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="eef3e-153">DateTime the object was created.</span></span> <span data-ttu-id="eef3e-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eef3e-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eef3e-155">description</span><span class="sxs-lookup"><span data-stu-id="eef3e-155">description</span></span>|<span data-ttu-id="eef3e-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eef3e-156">String</span></span>|<span data-ttu-id="eef3e-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="eef3e-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="eef3e-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eef3e-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eef3e-159">displayName</span><span class="sxs-lookup"><span data-stu-id="eef3e-159">displayName</span></span>|<span data-ttu-id="eef3e-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eef3e-160">String</span></span>|<span data-ttu-id="eef3e-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="eef3e-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="eef3e-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eef3e-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eef3e-163">Version</span><span class="sxs-lookup"><span data-stu-id="eef3e-163">version</span></span>|<span data-ttu-id="eef3e-164">Int32</span><span class="sxs-lookup"><span data-stu-id="eef3e-164">Int32</span></span>|<span data-ttu-id="eef3e-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="eef3e-165">Version of the device configuration.</span></span> <span data-ttu-id="eef3e-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eef3e-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eef3e-167">uninstallBuiltInApps</span><span class="sxs-lookup"><span data-stu-id="eef3e-167">uninstallBuiltInApps</span></span>|<span data-ttu-id="eef3e-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="eef3e-168">Boolean</span></span>|<span data-ttu-id="eef3e-169">Gibt an, ob eine festgelegte Liste integrierter Windows-Apps deinstalliert werden soll.</span><span class="sxs-lookup"><span data-stu-id="eef3e-169">Indicates whether or not to uninstall a fixed list of built-in Windows apps.</span></span>|



## <a name="response"></a><span data-ttu-id="eef3e-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="eef3e-170">Response</span></span>
<span data-ttu-id="eef3e-171">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="eef3e-171">If successful, this method returns a `201 Created` response code and a [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eef3e-172">Beispiel</span><span class="sxs-lookup"><span data-stu-id="eef3e-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="eef3e-173">Anforderung</span><span class="sxs-lookup"><span data-stu-id="eef3e-173">Request</span></span>
<span data-ttu-id="eef3e-174">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="eef3e-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="eef3e-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="eef3e-175">Response</span></span>
<span data-ttu-id="eef3e-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eef3e-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




