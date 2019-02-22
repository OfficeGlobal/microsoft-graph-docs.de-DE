---
title: Aktualisieren von „windowsPhone81CustomConfiguration“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs windowsPhone81CustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 348e2a5cf4f4e4a9fadd7d1de6b2e6920828c31a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147411"
---
# <a name="update-windowsphone81customconfiguration"></a><span data-ttu-id="036e0-103">Aktualisieren von „windowsPhone81CustomConfiguration“</span><span class="sxs-lookup"><span data-stu-id="036e0-103">Update windowsPhone81CustomConfiguration</span></span>

> <span data-ttu-id="036e0-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="036e0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="036e0-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="036e0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="036e0-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="036e0-106">Update the properties of a [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="036e0-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="036e0-107">Prerequisites</span></span>
<span data-ttu-id="036e0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="036e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="036e0-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="036e0-110">Permission type</span></span>|<span data-ttu-id="036e0-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="036e0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="036e0-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="036e0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="036e0-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="036e0-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="036e0-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="036e0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="036e0-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="036e0-115">Not supported.</span></span>|
|<span data-ttu-id="036e0-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="036e0-116">Application</span></span>|<span data-ttu-id="036e0-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="036e0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="036e0-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="036e0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="036e0-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="036e0-119">Request headers</span></span>
|<span data-ttu-id="036e0-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="036e0-120">Header</span></span>|<span data-ttu-id="036e0-121">Wert</span><span class="sxs-lookup"><span data-stu-id="036e0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="036e0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="036e0-122">Authorization</span></span>|<span data-ttu-id="036e0-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="036e0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="036e0-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="036e0-124">Accept</span></span>|<span data-ttu-id="036e0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="036e0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="036e0-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="036e0-126">Request body</span></span>
<span data-ttu-id="036e0-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="036e0-127">In the request body, supply a JSON representation for the [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

<span data-ttu-id="036e0-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="036e0-128">The following table shows the properties that are required when you create the [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span></span>

|<span data-ttu-id="036e0-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="036e0-129">Property</span></span>|<span data-ttu-id="036e0-130">Typ</span><span class="sxs-lookup"><span data-stu-id="036e0-130">Type</span></span>|<span data-ttu-id="036e0-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="036e0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="036e0-132">id</span><span class="sxs-lookup"><span data-stu-id="036e0-132">id</span></span>|<span data-ttu-id="036e0-133">string</span><span class="sxs-lookup"><span data-stu-id="036e0-133">String</span></span>|<span data-ttu-id="036e0-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="036e0-134">Key of the entity.</span></span> <span data-ttu-id="036e0-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="036e0-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="036e0-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="036e0-136">lastModifiedDateTime</span></span>|<span data-ttu-id="036e0-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="036e0-137">DateTimeOffset</span></span>|<span data-ttu-id="036e0-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="036e0-138">DateTime the object was last modified.</span></span> <span data-ttu-id="036e0-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="036e0-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="036e0-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="036e0-140">roleScopeTagIds</span></span>|<span data-ttu-id="036e0-141">String collection</span><span class="sxs-lookup"><span data-stu-id="036e0-141">String collection</span></span>|<span data-ttu-id="036e0-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="036e0-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="036e0-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="036e0-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="036e0-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="036e0-144">supportsScopeTags</span></span>|<span data-ttu-id="036e0-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="036e0-145">Boolean</span></span>|<span data-ttu-id="036e0-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="036e0-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="036e0-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="036e0-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="036e0-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="036e0-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="036e0-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="036e0-149">This property is read-only.</span></span> <span data-ttu-id="036e0-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="036e0-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="036e0-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="036e0-151">createdDateTime</span></span>|<span data-ttu-id="036e0-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="036e0-152">DateTimeOffset</span></span>|<span data-ttu-id="036e0-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="036e0-153">DateTime the object was created.</span></span> <span data-ttu-id="036e0-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="036e0-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="036e0-155">description</span><span class="sxs-lookup"><span data-stu-id="036e0-155">description</span></span>|<span data-ttu-id="036e0-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="036e0-156">String</span></span>|<span data-ttu-id="036e0-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="036e0-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="036e0-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="036e0-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="036e0-159">displayName</span><span class="sxs-lookup"><span data-stu-id="036e0-159">displayName</span></span>|<span data-ttu-id="036e0-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="036e0-160">String</span></span>|<span data-ttu-id="036e0-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="036e0-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="036e0-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="036e0-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="036e0-163">Version</span><span class="sxs-lookup"><span data-stu-id="036e0-163">version</span></span>|<span data-ttu-id="036e0-164">Int32</span><span class="sxs-lookup"><span data-stu-id="036e0-164">Int32</span></span>|<span data-ttu-id="036e0-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="036e0-165">Version of the device configuration.</span></span> <span data-ttu-id="036e0-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="036e0-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="036e0-167">omaSettings</span><span class="sxs-lookup"><span data-stu-id="036e0-167">omaSettings</span></span>|<span data-ttu-id="036e0-168">Collection von Objekten des Typs [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="036e0-168">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="036e0-169">OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="036e0-169">OMA settings.</span></span> <span data-ttu-id="036e0-170">Diese Sammlung kann bis zu 1000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="036e0-170">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="036e0-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="036e0-171">Response</span></span>
<span data-ttu-id="036e0-172">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="036e0-172">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="036e0-173">Beispiel</span><span class="sxs-lookup"><span data-stu-id="036e0-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="036e0-174">Anforderung</span><span class="sxs-lookup"><span data-stu-id="036e0-174">Request</span></span>
<span data-ttu-id="036e0-175">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="036e0-175">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 501

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="036e0-176">Antwort</span><span class="sxs-lookup"><span data-stu-id="036e0-176">Response</span></span>
<span data-ttu-id="036e0-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="036e0-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 673

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
  "id": "0d98693c-693c-0d98-3c69-980d3c69980d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```




