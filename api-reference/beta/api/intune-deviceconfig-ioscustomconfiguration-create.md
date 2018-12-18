---
title: Erstellen von „iosCustomConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs iosCustomConfiguration.
author: tfitzmac
ms.openlocfilehash: e22a670316ca7ffb4216c45cab5e8f3e6d7f3d65
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343309"
---
# <a name="create-ioscustomconfiguration"></a><span data-ttu-id="b5565-103">Erstellen von „iosCustomConfiguration“</span><span class="sxs-lookup"><span data-stu-id="b5565-103">Create iosCustomConfiguration</span></span>

> <span data-ttu-id="b5565-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b5565-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b5565-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b5565-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b5565-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b5565-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b5565-107">Diese Methode erstellt ein neues Objekt des Typs [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b5565-107">Create a new [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b5565-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b5565-108">Prerequisites</span></span>
<span data-ttu-id="b5565-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5565-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5565-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b5565-111">Permission type</span></span>|<span data-ttu-id="b5565-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b5565-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5565-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b5565-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b5565-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5565-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b5565-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b5565-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5565-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b5565-116">Not supported.</span></span>|
|<span data-ttu-id="b5565-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b5565-117">Application</span></span>|<span data-ttu-id="b5565-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b5565-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5565-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b5565-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b5565-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b5565-120">Request headers</span></span>
|<span data-ttu-id="b5565-121">Header</span><span class="sxs-lookup"><span data-stu-id="b5565-121">Header</span></span>|<span data-ttu-id="b5565-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b5565-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5565-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="b5565-123">Authorization</span></span>|<span data-ttu-id="b5565-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b5565-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5565-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b5565-125">Accept</span></span>|<span data-ttu-id="b5565-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b5565-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5565-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b5565-127">Request body</span></span>
<span data-ttu-id="b5565-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „iosCustomConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="b5565-128">In the request body, supply a JSON representation for the iosCustomConfiguration object.</span></span>

<span data-ttu-id="b5565-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „iosCustomConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="b5565-129">The following table shows the properties that are required when you create the iosCustomConfiguration.</span></span>

|<span data-ttu-id="b5565-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b5565-130">Property</span></span>|<span data-ttu-id="b5565-131">Typ</span><span class="sxs-lookup"><span data-stu-id="b5565-131">Type</span></span>|<span data-ttu-id="b5565-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b5565-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5565-133">id</span><span class="sxs-lookup"><span data-stu-id="b5565-133">id</span></span>|<span data-ttu-id="b5565-134">String</span><span class="sxs-lookup"><span data-stu-id="b5565-134">String</span></span>|<span data-ttu-id="b5565-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b5565-135">Key of the entity.</span></span> <span data-ttu-id="b5565-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b5565-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5565-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b5565-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b5565-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5565-138">DateTimeOffset</span></span>|<span data-ttu-id="b5565-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b5565-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b5565-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b5565-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5565-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b5565-141">roleScopeTagIds</span></span>|<span data-ttu-id="b5565-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="b5565-142">String collection</span></span>|<span data-ttu-id="b5565-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="b5565-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b5565-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b5565-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5565-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b5565-145">supportsScopeTags</span></span>|<span data-ttu-id="b5565-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="b5565-146">Boolean</span></span>|<span data-ttu-id="b5565-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b5565-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b5565-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="b5565-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b5565-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="b5565-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b5565-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b5565-150">This property is read-only.</span></span> <span data-ttu-id="b5565-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b5565-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5565-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b5565-152">createdDateTime</span></span>|<span data-ttu-id="b5565-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5565-153">DateTimeOffset</span></span>|<span data-ttu-id="b5565-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b5565-154">DateTime the object was created.</span></span> <span data-ttu-id="b5565-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b5565-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5565-156">description</span><span class="sxs-lookup"><span data-stu-id="b5565-156">description</span></span>|<span data-ttu-id="b5565-157">String</span><span class="sxs-lookup"><span data-stu-id="b5565-157">String</span></span>|<span data-ttu-id="b5565-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b5565-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b5565-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b5565-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5565-160">displayName</span><span class="sxs-lookup"><span data-stu-id="b5565-160">displayName</span></span>|<span data-ttu-id="b5565-161">String</span><span class="sxs-lookup"><span data-stu-id="b5565-161">String</span></span>|<span data-ttu-id="b5565-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b5565-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b5565-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b5565-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5565-164">Version</span><span class="sxs-lookup"><span data-stu-id="b5565-164">version</span></span>|<span data-ttu-id="b5565-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b5565-165">Int32</span></span>|<span data-ttu-id="b5565-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="b5565-166">Version of the device configuration.</span></span> <span data-ttu-id="b5565-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b5565-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5565-168">payloadName</span><span class="sxs-lookup"><span data-stu-id="b5565-168">payloadName</span></span>|<span data-ttu-id="b5565-169">String</span><span class="sxs-lookup"><span data-stu-id="b5565-169">String</span></span>|<span data-ttu-id="b5565-170">Name, der dem Benutzer angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="b5565-170">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="b5565-171">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="b5565-171">payloadFileName</span></span>|<span data-ttu-id="b5565-172">String</span><span class="sxs-lookup"><span data-stu-id="b5565-172">String</span></span>|<span data-ttu-id="b5565-173">Name der Nutzlastdatei (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="b5565-173">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="b5565-174">\*.xml)</span><span class="sxs-lookup"><span data-stu-id="b5565-174">\*.xml).</span></span>|
|<span data-ttu-id="b5565-175">payload</span><span class="sxs-lookup"><span data-stu-id="b5565-175">payload</span></span>|<span data-ttu-id="b5565-176">Binär</span><span class="sxs-lookup"><span data-stu-id="b5565-176">Binary</span></span>|<span data-ttu-id="b5565-177">Nutzlast</span><span class="sxs-lookup"><span data-stu-id="b5565-177">Payload.</span></span> <span data-ttu-id="b5565-178">(UTF8-codiertes Bytearray)</span><span class="sxs-lookup"><span data-stu-id="b5565-178">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="b5565-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="b5565-179">Response</span></span>
<span data-ttu-id="b5565-180">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b5565-180">If successful, this method returns a `201 Created` response code and a [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5565-181">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b5565-181">Example</span></span>
### <a name="request"></a><span data-ttu-id="b5565-182">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b5565-182">Request</span></span>
<span data-ttu-id="b5565-183">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b5565-183">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 435

{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="b5565-184">Antwort</span><span class="sxs-lookup"><span data-stu-id="b5565-184">Response</span></span>
<span data-ttu-id="b5565-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b5565-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





