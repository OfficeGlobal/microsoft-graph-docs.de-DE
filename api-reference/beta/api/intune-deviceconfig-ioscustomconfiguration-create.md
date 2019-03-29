---
title: Erstellen von „iosCustomConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs iosCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3badf925afc6a665734661d17fa371a4a1460df9
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30976799"
---
# <a name="create-ioscustomconfiguration"></a><span data-ttu-id="4ba2d-103">Erstellen von „iosCustomConfiguration“</span><span class="sxs-lookup"><span data-stu-id="4ba2d-103">Create iosCustomConfiguration</span></span>

> <span data-ttu-id="4ba2d-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4ba2d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ba2d-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="4ba2d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ba2d-106">Diese Methode erstellt ein neues Objekt des Typs [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4ba2d-106">Create a new [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4ba2d-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4ba2d-107">Prerequisites</span></span>
<span data-ttu-id="4ba2d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ba2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ba2d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4ba2d-110">Permission type</span></span>|<span data-ttu-id="4ba2d-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4ba2d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ba2d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4ba2d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4ba2d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ba2d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4ba2d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4ba2d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ba2d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4ba2d-115">Not supported.</span></span>|
|<span data-ttu-id="4ba2d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4ba2d-116">Application</span></span>|<span data-ttu-id="4ba2d-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4ba2d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ba2d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4ba2d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4ba2d-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4ba2d-119">Request headers</span></span>
|<span data-ttu-id="4ba2d-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4ba2d-120">Header</span></span>|<span data-ttu-id="4ba2d-121">Wert</span><span class="sxs-lookup"><span data-stu-id="4ba2d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ba2d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ba2d-122">Authorization</span></span>|<span data-ttu-id="4ba2d-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4ba2d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ba2d-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4ba2d-124">Accept</span></span>|<span data-ttu-id="4ba2d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4ba2d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ba2d-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4ba2d-126">Request body</span></span>
<span data-ttu-id="4ba2d-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „iosCustomConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="4ba2d-127">In the request body, supply a JSON representation for the iosCustomConfiguration object.</span></span>

<span data-ttu-id="4ba2d-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „iosCustomConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="4ba2d-128">The following table shows the properties that are required when you create the iosCustomConfiguration.</span></span>

|<span data-ttu-id="4ba2d-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4ba2d-129">Property</span></span>|<span data-ttu-id="4ba2d-130">Typ</span><span class="sxs-lookup"><span data-stu-id="4ba2d-130">Type</span></span>|<span data-ttu-id="4ba2d-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4ba2d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ba2d-132">id</span><span class="sxs-lookup"><span data-stu-id="4ba2d-132">id</span></span>|<span data-ttu-id="4ba2d-133">String</span><span class="sxs-lookup"><span data-stu-id="4ba2d-133">String</span></span>|<span data-ttu-id="4ba2d-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="4ba2d-134">Key of the entity.</span></span> <span data-ttu-id="4ba2d-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4ba2d-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ba2d-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4ba2d-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4ba2d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ba2d-137">DateTimeOffset</span></span>|<span data-ttu-id="4ba2d-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="4ba2d-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4ba2d-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4ba2d-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ba2d-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="4ba2d-140">roleScopeTagIds</span></span>|<span data-ttu-id="4ba2d-141">String collection</span><span class="sxs-lookup"><span data-stu-id="4ba2d-141">String collection</span></span>|<span data-ttu-id="4ba2d-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="4ba2d-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4ba2d-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4ba2d-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ba2d-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4ba2d-144">supportsScopeTags</span></span>|<span data-ttu-id="4ba2d-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4ba2d-145">Boolean</span></span>|<span data-ttu-id="4ba2d-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4ba2d-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4ba2d-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="4ba2d-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4ba2d-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="4ba2d-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4ba2d-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="4ba2d-149">This property is read-only.</span></span> <span data-ttu-id="4ba2d-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4ba2d-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ba2d-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4ba2d-151">createdDateTime</span></span>|<span data-ttu-id="4ba2d-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ba2d-152">DateTimeOffset</span></span>|<span data-ttu-id="4ba2d-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="4ba2d-153">DateTime the object was created.</span></span> <span data-ttu-id="4ba2d-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4ba2d-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ba2d-155">description</span><span class="sxs-lookup"><span data-stu-id="4ba2d-155">description</span></span>|<span data-ttu-id="4ba2d-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4ba2d-156">String</span></span>|<span data-ttu-id="4ba2d-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="4ba2d-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4ba2d-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4ba2d-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ba2d-159">displayName</span><span class="sxs-lookup"><span data-stu-id="4ba2d-159">displayName</span></span>|<span data-ttu-id="4ba2d-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4ba2d-160">String</span></span>|<span data-ttu-id="4ba2d-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="4ba2d-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4ba2d-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4ba2d-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ba2d-163">Version</span><span class="sxs-lookup"><span data-stu-id="4ba2d-163">version</span></span>|<span data-ttu-id="4ba2d-164">Int32</span><span class="sxs-lookup"><span data-stu-id="4ba2d-164">Int32</span></span>|<span data-ttu-id="4ba2d-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="4ba2d-165">Version of the device configuration.</span></span> <span data-ttu-id="4ba2d-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4ba2d-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ba2d-167">payloadName</span><span class="sxs-lookup"><span data-stu-id="4ba2d-167">payloadName</span></span>|<span data-ttu-id="4ba2d-168">String</span><span class="sxs-lookup"><span data-stu-id="4ba2d-168">String</span></span>|<span data-ttu-id="4ba2d-169">Name, der dem Benutzer angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="4ba2d-169">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="4ba2d-170">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="4ba2d-170">payloadFileName</span></span>|<span data-ttu-id="4ba2d-171">String</span><span class="sxs-lookup"><span data-stu-id="4ba2d-171">String</span></span>|<span data-ttu-id="4ba2d-172">Name der Nutzlastdatei (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="4ba2d-172">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="4ba2d-173">\*.xml)</span><span class="sxs-lookup"><span data-stu-id="4ba2d-173">\*.xml).</span></span>|
|<span data-ttu-id="4ba2d-174">payload</span><span class="sxs-lookup"><span data-stu-id="4ba2d-174">payload</span></span>|<span data-ttu-id="4ba2d-175">Binär</span><span class="sxs-lookup"><span data-stu-id="4ba2d-175">Binary</span></span>|<span data-ttu-id="4ba2d-176">Nutzlast</span><span class="sxs-lookup"><span data-stu-id="4ba2d-176">Payload.</span></span> <span data-ttu-id="4ba2d-177">(UTF8-codiertes Bytearray)</span><span class="sxs-lookup"><span data-stu-id="4ba2d-177">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="4ba2d-178">Antwort</span><span class="sxs-lookup"><span data-stu-id="4ba2d-178">Response</span></span>
<span data-ttu-id="4ba2d-179">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="4ba2d-179">If successful, this method returns a `201 Created` response code and a [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ba2d-180">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4ba2d-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="4ba2d-181">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4ba2d-181">Request</span></span>
<span data-ttu-id="4ba2d-182">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4ba2d-182">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="4ba2d-183">Antwort</span><span class="sxs-lookup"><span data-stu-id="4ba2d-183">Response</span></span>
<span data-ttu-id="4ba2d-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4ba2d-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




