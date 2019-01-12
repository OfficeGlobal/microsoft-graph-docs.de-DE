---
title: Aktualisieren von „iosCustomConfiguration“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs iosCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 42f55f63e20dfbfdde4f350ce02100f820c88bbc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978333"
---
# <a name="update-ioscustomconfiguration"></a><span data-ttu-id="2b3ff-103">Aktualisieren von „iosCustomConfiguration“</span><span class="sxs-lookup"><span data-stu-id="2b3ff-103">Update iosCustomConfiguration</span></span>

> <span data-ttu-id="2b3ff-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2b3ff-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2b3ff-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2b3ff-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2b3ff-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2b3ff-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2b3ff-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b3ff-107">Update the properties of a [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2b3ff-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2b3ff-108">Prerequisites</span></span>
<span data-ttu-id="2b3ff-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b3ff-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b3ff-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2b3ff-111">Permission type</span></span>|<span data-ttu-id="2b3ff-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2b3ff-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b3ff-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2b3ff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2b3ff-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b3ff-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2b3ff-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2b3ff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b3ff-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2b3ff-116">Not supported.</span></span>|
|<span data-ttu-id="2b3ff-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2b3ff-117">Application</span></span>|<span data-ttu-id="2b3ff-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2b3ff-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b3ff-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2b3ff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2b3ff-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2b3ff-120">Request headers</span></span>
|<span data-ttu-id="2b3ff-121">Header</span><span class="sxs-lookup"><span data-stu-id="2b3ff-121">Header</span></span>|<span data-ttu-id="2b3ff-122">Wert</span><span class="sxs-lookup"><span data-stu-id="2b3ff-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b3ff-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b3ff-123">Authorization</span></span>|<span data-ttu-id="2b3ff-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2b3ff-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b3ff-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2b3ff-125">Accept</span></span>|<span data-ttu-id="2b3ff-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2b3ff-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b3ff-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2b3ff-127">Request body</span></span>
<span data-ttu-id="2b3ff-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="2b3ff-128">In the request body, supply a JSON representation for the [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>

<span data-ttu-id="2b3ff-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="2b3ff-129">The following table shows the properties that are required when you create the [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span></span>

|<span data-ttu-id="2b3ff-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2b3ff-130">Property</span></span>|<span data-ttu-id="2b3ff-131">Typ</span><span class="sxs-lookup"><span data-stu-id="2b3ff-131">Type</span></span>|<span data-ttu-id="2b3ff-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2b3ff-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b3ff-133">id</span><span class="sxs-lookup"><span data-stu-id="2b3ff-133">id</span></span>|<span data-ttu-id="2b3ff-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2b3ff-134">String</span></span>|<span data-ttu-id="2b3ff-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="2b3ff-135">Key of the entity.</span></span> <span data-ttu-id="2b3ff-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b3ff-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b3ff-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2b3ff-137">lastModifiedDateTime</span></span>|<span data-ttu-id="2b3ff-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b3ff-138">DateTimeOffset</span></span>|<span data-ttu-id="2b3ff-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="2b3ff-139">DateTime the object was last modified.</span></span> <span data-ttu-id="2b3ff-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b3ff-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b3ff-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2b3ff-141">roleScopeTagIds</span></span>|<span data-ttu-id="2b3ff-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="2b3ff-142">String collection</span></span>|<span data-ttu-id="2b3ff-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="2b3ff-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2b3ff-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b3ff-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b3ff-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2b3ff-145">supportsScopeTags</span></span>|<span data-ttu-id="2b3ff-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2b3ff-146">Boolean</span></span>|<span data-ttu-id="2b3ff-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2b3ff-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2b3ff-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="2b3ff-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2b3ff-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="2b3ff-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2b3ff-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2b3ff-150">This property is read-only.</span></span> <span data-ttu-id="2b3ff-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b3ff-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b3ff-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2b3ff-152">createdDateTime</span></span>|<span data-ttu-id="2b3ff-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b3ff-153">DateTimeOffset</span></span>|<span data-ttu-id="2b3ff-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="2b3ff-154">DateTime the object was created.</span></span> <span data-ttu-id="2b3ff-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b3ff-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b3ff-156">description</span><span class="sxs-lookup"><span data-stu-id="2b3ff-156">description</span></span>|<span data-ttu-id="2b3ff-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2b3ff-157">String</span></span>|<span data-ttu-id="2b3ff-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="2b3ff-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2b3ff-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b3ff-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b3ff-160">displayName</span><span class="sxs-lookup"><span data-stu-id="2b3ff-160">displayName</span></span>|<span data-ttu-id="2b3ff-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2b3ff-161">String</span></span>|<span data-ttu-id="2b3ff-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="2b3ff-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2b3ff-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b3ff-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b3ff-164">Version</span><span class="sxs-lookup"><span data-stu-id="2b3ff-164">version</span></span>|<span data-ttu-id="2b3ff-165">Int32</span><span class="sxs-lookup"><span data-stu-id="2b3ff-165">Int32</span></span>|<span data-ttu-id="2b3ff-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="2b3ff-166">Version of the device configuration.</span></span> <span data-ttu-id="2b3ff-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b3ff-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b3ff-168">payloadName</span><span class="sxs-lookup"><span data-stu-id="2b3ff-168">payloadName</span></span>|<span data-ttu-id="2b3ff-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2b3ff-169">String</span></span>|<span data-ttu-id="2b3ff-170">Name, der dem Benutzer angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="2b3ff-170">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="2b3ff-171">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="2b3ff-171">payloadFileName</span></span>|<span data-ttu-id="2b3ff-172">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2b3ff-172">String</span></span>|<span data-ttu-id="2b3ff-173">Name der Nutzlastdatei (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="2b3ff-173">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="2b3ff-174">\*.xml)</span><span class="sxs-lookup"><span data-stu-id="2b3ff-174">\*.xml).</span></span>|
|<span data-ttu-id="2b3ff-175">payload</span><span class="sxs-lookup"><span data-stu-id="2b3ff-175">payload</span></span>|<span data-ttu-id="2b3ff-176">Binär</span><span class="sxs-lookup"><span data-stu-id="2b3ff-176">Binary</span></span>|<span data-ttu-id="2b3ff-177">Nutzlast</span><span class="sxs-lookup"><span data-stu-id="2b3ff-177">Payload.</span></span> <span data-ttu-id="2b3ff-178">(UTF8-codiertes Bytearray)</span><span class="sxs-lookup"><span data-stu-id="2b3ff-178">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="2b3ff-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="2b3ff-179">Response</span></span>
<span data-ttu-id="2b3ff-180">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2b3ff-180">If successful, this method returns a `200 OK` response code and an updated [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b3ff-181">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2b3ff-181">Example</span></span>
### <a name="request"></a><span data-ttu-id="2b3ff-182">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2b3ff-182">Request</span></span>
<span data-ttu-id="2b3ff-183">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2b3ff-183">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 374

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```

### <a name="response"></a><span data-ttu-id="2b3ff-184">Antwort</span><span class="sxs-lookup"><span data-stu-id="2b3ff-184">Response</span></span>
<span data-ttu-id="2b3ff-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2b3ff-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 543

{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
  "id": "f34428e3-28e3-f344-e328-44f3e32844f3",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```





