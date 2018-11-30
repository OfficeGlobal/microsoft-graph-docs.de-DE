---
title: Aktualisieren von „windows10CustomConfiguration“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs windows10CustomConfiguration.
ms.openlocfilehash: a823f8341a6db84776714a28cb72bb94e8154d4e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065897"
---
# <a name="update-windows10customconfiguration"></a><span data-ttu-id="c53af-103">Aktualisieren von „windows10CustomConfiguration“</span><span class="sxs-lookup"><span data-stu-id="c53af-103">Update windows10CustomConfiguration</span></span>

> <span data-ttu-id="c53af-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c53af-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c53af-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c53af-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c53af-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c53af-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c53af-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c53af-107">Update the properties of a [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c53af-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c53af-108">Prerequisites</span></span>
<span data-ttu-id="c53af-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c53af-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c53af-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c53af-111">Permission type</span></span>|<span data-ttu-id="c53af-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c53af-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c53af-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c53af-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c53af-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c53af-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c53af-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c53af-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c53af-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c53af-116">Not supported.</span></span>|
|<span data-ttu-id="c53af-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c53af-117">Application</span></span>|<span data-ttu-id="c53af-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c53af-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c53af-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c53af-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c53af-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c53af-120">Request headers</span></span>
|<span data-ttu-id="c53af-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c53af-121">Header</span></span>|<span data-ttu-id="c53af-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c53af-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c53af-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c53af-123">Authorization</span></span>|<span data-ttu-id="c53af-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c53af-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c53af-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c53af-125">Accept</span></span>|<span data-ttu-id="c53af-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c53af-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c53af-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c53af-127">Request body</span></span>
<span data-ttu-id="c53af-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="c53af-128">In the request body, supply a JSON representation for the [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object.</span></span>

<span data-ttu-id="c53af-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="c53af-129">The following table shows the properties that are required when you create the [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span></span>

|<span data-ttu-id="c53af-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c53af-130">Property</span></span>|<span data-ttu-id="c53af-131">Typ</span><span class="sxs-lookup"><span data-stu-id="c53af-131">Type</span></span>|<span data-ttu-id="c53af-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c53af-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c53af-133">id</span><span class="sxs-lookup"><span data-stu-id="c53af-133">id</span></span>|<span data-ttu-id="c53af-134">String</span><span class="sxs-lookup"><span data-stu-id="c53af-134">String</span></span>|<span data-ttu-id="c53af-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c53af-135">Key of the entity.</span></span> <span data-ttu-id="c53af-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c53af-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c53af-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c53af-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c53af-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c53af-138">DateTimeOffset</span></span>|<span data-ttu-id="c53af-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="c53af-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c53af-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c53af-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c53af-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c53af-141">roleScopeTagIds</span></span>|<span data-ttu-id="c53af-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="c53af-142">String collection</span></span>|<span data-ttu-id="c53af-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="c53af-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c53af-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c53af-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c53af-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c53af-145">supportsScopeTags</span></span>|<span data-ttu-id="c53af-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c53af-146">Boolean</span></span>|<span data-ttu-id="c53af-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c53af-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c53af-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="c53af-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c53af-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="c53af-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c53af-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c53af-150">This property is read-only.</span></span> <span data-ttu-id="c53af-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c53af-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c53af-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c53af-152">createdDateTime</span></span>|<span data-ttu-id="c53af-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c53af-153">DateTimeOffset</span></span>|<span data-ttu-id="c53af-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="c53af-154">DateTime the object was created.</span></span> <span data-ttu-id="c53af-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c53af-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c53af-156">description</span><span class="sxs-lookup"><span data-stu-id="c53af-156">description</span></span>|<span data-ttu-id="c53af-157">String</span><span class="sxs-lookup"><span data-stu-id="c53af-157">String</span></span>|<span data-ttu-id="c53af-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="c53af-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c53af-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c53af-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c53af-160">displayName</span><span class="sxs-lookup"><span data-stu-id="c53af-160">displayName</span></span>|<span data-ttu-id="c53af-161">String</span><span class="sxs-lookup"><span data-stu-id="c53af-161">String</span></span>|<span data-ttu-id="c53af-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="c53af-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c53af-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c53af-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c53af-164">Version</span><span class="sxs-lookup"><span data-stu-id="c53af-164">version</span></span>|<span data-ttu-id="c53af-165">Int32</span><span class="sxs-lookup"><span data-stu-id="c53af-165">Int32</span></span>|<span data-ttu-id="c53af-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="c53af-166">Version of the device configuration.</span></span> <span data-ttu-id="c53af-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c53af-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c53af-168">omaSettings</span><span class="sxs-lookup"><span data-stu-id="c53af-168">omaSettings</span></span>|<span data-ttu-id="c53af-169">Collection von Objekten des Typs [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c53af-169">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="c53af-170">OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="c53af-170">OMA settings.</span></span> <span data-ttu-id="c53af-171">Diese Sammlung kann bis zu 1000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="c53af-171">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="c53af-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="c53af-172">Response</span></span>
<span data-ttu-id="c53af-173">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c53af-173">If successful, this method returns a `200 OK` response code and an updated [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c53af-174">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c53af-174">Example</span></span>
### <a name="request"></a><span data-ttu-id="c53af-175">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c53af-175">Request</span></span>
<span data-ttu-id="c53af-176">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c53af-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 493

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="c53af-177">Antwort</span><span class="sxs-lookup"><span data-stu-id="c53af-177">Response</span></span>
<span data-ttu-id="c53af-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c53af-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 668

{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
  "id": "d8ae266e-266e-d8ae-6e26-aed86e26aed8",
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





