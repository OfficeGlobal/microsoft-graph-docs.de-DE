---
title: Aktualisieren von „iosCustomConfiguration“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs iosCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e69d7bedf2a1b3a3fcadd8738addfb5665971457
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162566"
---
# <a name="update-ioscustomconfiguration"></a><span data-ttu-id="3c454-103">Aktualisieren von „iosCustomConfiguration“</span><span class="sxs-lookup"><span data-stu-id="3c454-103">Update iosCustomConfiguration</span></span>

> <span data-ttu-id="3c454-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c454-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c454-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="3c454-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c454-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c454-106">Update the properties of a [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c454-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3c454-107">Prerequisites</span></span>
<span data-ttu-id="3c454-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3c454-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3c454-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3c454-110">Permission type</span></span>|<span data-ttu-id="3c454-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3c454-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c454-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3c454-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3c454-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c454-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3c454-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3c454-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c454-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3c454-115">Not supported.</span></span>|
|<span data-ttu-id="3c454-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3c454-116">Application</span></span>|<span data-ttu-id="3c454-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3c454-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c454-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3c454-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="3c454-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3c454-119">Request headers</span></span>
|<span data-ttu-id="3c454-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3c454-120">Header</span></span>|<span data-ttu-id="3c454-121">Wert</span><span class="sxs-lookup"><span data-stu-id="3c454-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c454-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c454-122">Authorization</span></span>|<span data-ttu-id="3c454-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3c454-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c454-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3c454-124">Accept</span></span>|<span data-ttu-id="3c454-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3c454-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c454-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3c454-126">Request body</span></span>
<span data-ttu-id="3c454-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="3c454-127">In the request body, supply a JSON representation for the [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>

<span data-ttu-id="3c454-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="3c454-128">The following table shows the properties that are required when you create the [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span></span>

|<span data-ttu-id="3c454-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3c454-129">Property</span></span>|<span data-ttu-id="3c454-130">Typ</span><span class="sxs-lookup"><span data-stu-id="3c454-130">Type</span></span>|<span data-ttu-id="3c454-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3c454-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c454-132">id</span><span class="sxs-lookup"><span data-stu-id="3c454-132">id</span></span>|<span data-ttu-id="3c454-133">string</span><span class="sxs-lookup"><span data-stu-id="3c454-133">String</span></span>|<span data-ttu-id="3c454-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="3c454-134">Key of the entity.</span></span> <span data-ttu-id="3c454-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c454-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c454-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3c454-136">lastModifiedDateTime</span></span>|<span data-ttu-id="3c454-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c454-137">DateTimeOffset</span></span>|<span data-ttu-id="3c454-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="3c454-138">DateTime the object was last modified.</span></span> <span data-ttu-id="3c454-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c454-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c454-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="3c454-140">roleScopeTagIds</span></span>|<span data-ttu-id="3c454-141">String collection</span><span class="sxs-lookup"><span data-stu-id="3c454-141">String collection</span></span>|<span data-ttu-id="3c454-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="3c454-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3c454-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c454-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c454-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3c454-144">supportsScopeTags</span></span>|<span data-ttu-id="3c454-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c454-145">Boolean</span></span>|<span data-ttu-id="3c454-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c454-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3c454-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="3c454-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3c454-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="3c454-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3c454-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="3c454-149">This property is read-only.</span></span> <span data-ttu-id="3c454-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c454-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c454-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3c454-151">createdDateTime</span></span>|<span data-ttu-id="3c454-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c454-152">DateTimeOffset</span></span>|<span data-ttu-id="3c454-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="3c454-153">DateTime the object was created.</span></span> <span data-ttu-id="3c454-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c454-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c454-155">description</span><span class="sxs-lookup"><span data-stu-id="3c454-155">description</span></span>|<span data-ttu-id="3c454-156">String</span><span class="sxs-lookup"><span data-stu-id="3c454-156">String</span></span>|<span data-ttu-id="3c454-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="3c454-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3c454-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c454-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c454-159">displayName</span><span class="sxs-lookup"><span data-stu-id="3c454-159">displayName</span></span>|<span data-ttu-id="3c454-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3c454-160">String</span></span>|<span data-ttu-id="3c454-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="3c454-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3c454-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c454-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c454-163">Version</span><span class="sxs-lookup"><span data-stu-id="3c454-163">version</span></span>|<span data-ttu-id="3c454-164">Int32</span><span class="sxs-lookup"><span data-stu-id="3c454-164">Int32</span></span>|<span data-ttu-id="3c454-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="3c454-165">Version of the device configuration.</span></span> <span data-ttu-id="3c454-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c454-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c454-167">payloadName</span><span class="sxs-lookup"><span data-stu-id="3c454-167">payloadName</span></span>|<span data-ttu-id="3c454-168">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3c454-168">String</span></span>|<span data-ttu-id="3c454-169">Name, der dem Benutzer angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="3c454-169">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="3c454-170">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="3c454-170">payloadFileName</span></span>|<span data-ttu-id="3c454-171">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3c454-171">String</span></span>|<span data-ttu-id="3c454-172">Name der Nutzlastdatei (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="3c454-172">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="3c454-173">\*.xml)</span><span class="sxs-lookup"><span data-stu-id="3c454-173">\*.xml).</span></span>|
|<span data-ttu-id="3c454-174">payload</span><span class="sxs-lookup"><span data-stu-id="3c454-174">payload</span></span>|<span data-ttu-id="3c454-175">Binär</span><span class="sxs-lookup"><span data-stu-id="3c454-175">Binary</span></span>|<span data-ttu-id="3c454-176">Nutzlast</span><span class="sxs-lookup"><span data-stu-id="3c454-176">Payload.</span></span> <span data-ttu-id="3c454-177">(UTF8-codiertes Bytearray)</span><span class="sxs-lookup"><span data-stu-id="3c454-177">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="3c454-178">Antwort</span><span class="sxs-lookup"><span data-stu-id="3c454-178">Response</span></span>
<span data-ttu-id="3c454-179">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3c454-179">If successful, this method returns a `200 OK` response code and an updated [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c454-180">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3c454-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c454-181">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3c454-181">Request</span></span>
<span data-ttu-id="3c454-182">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3c454-182">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 371

{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="3c454-183">Antwort</span><span class="sxs-lookup"><span data-stu-id="3c454-183">Response</span></span>
<span data-ttu-id="3c454-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3c454-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




