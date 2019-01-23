---
title: Erstellen von „iosCustomConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs iosCustomConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7b5461d7267a2aa9b0d27439ee98217e82ab886c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421347"
---
# <a name="create-ioscustomconfiguration"></a><span data-ttu-id="e3e0e-103">Erstellen von „iosCustomConfiguration“</span><span class="sxs-lookup"><span data-stu-id="e3e0e-103">Create iosCustomConfiguration</span></span>

> <span data-ttu-id="e3e0e-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="e3e0e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e3e0e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e3e0e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e3e0e-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e3e0e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3e0e-107">Diese Methode erstellt ein neues Objekt des Typs [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e3e0e-107">Create a new [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e3e0e-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e3e0e-108">Prerequisites</span></span>
<span data-ttu-id="e3e0e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e3e0e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e3e0e-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e3e0e-111">Permission type</span></span>|<span data-ttu-id="e3e0e-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e3e0e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3e0e-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e3e0e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e3e0e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3e0e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e3e0e-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e3e0e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3e0e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e3e0e-116">Not supported.</span></span>|
|<span data-ttu-id="e3e0e-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e3e0e-117">Application</span></span>|<span data-ttu-id="e3e0e-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e3e0e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3e0e-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e3e0e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e3e0e-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e3e0e-120">Request headers</span></span>
|<span data-ttu-id="e3e0e-121">Header</span><span class="sxs-lookup"><span data-stu-id="e3e0e-121">Header</span></span>|<span data-ttu-id="e3e0e-122">Wert</span><span class="sxs-lookup"><span data-stu-id="e3e0e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3e0e-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="e3e0e-123">Authorization</span></span>|<span data-ttu-id="e3e0e-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e3e0e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3e0e-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e3e0e-125">Accept</span></span>|<span data-ttu-id="e3e0e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e3e0e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3e0e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e3e0e-127">Request body</span></span>
<span data-ttu-id="e3e0e-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „iosCustomConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="e3e0e-128">In the request body, supply a JSON representation for the iosCustomConfiguration object.</span></span>

<span data-ttu-id="e3e0e-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „iosCustomConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="e3e0e-129">The following table shows the properties that are required when you create the iosCustomConfiguration.</span></span>

|<span data-ttu-id="e3e0e-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e3e0e-130">Property</span></span>|<span data-ttu-id="e3e0e-131">Typ</span><span class="sxs-lookup"><span data-stu-id="e3e0e-131">Type</span></span>|<span data-ttu-id="e3e0e-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e3e0e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3e0e-133">id</span><span class="sxs-lookup"><span data-stu-id="e3e0e-133">id</span></span>|<span data-ttu-id="e3e0e-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e3e0e-134">String</span></span>|<span data-ttu-id="e3e0e-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="e3e0e-135">Key of the entity.</span></span> <span data-ttu-id="e3e0e-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e3e0e-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e3e0e-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e3e0e-137">lastModifiedDateTime</span></span>|<span data-ttu-id="e3e0e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3e0e-138">DateTimeOffset</span></span>|<span data-ttu-id="e3e0e-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="e3e0e-139">DateTime the object was last modified.</span></span> <span data-ttu-id="e3e0e-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e3e0e-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e3e0e-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e3e0e-141">roleScopeTagIds</span></span>|<span data-ttu-id="e3e0e-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="e3e0e-142">String collection</span></span>|<span data-ttu-id="e3e0e-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="e3e0e-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e3e0e-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e3e0e-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e3e0e-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e3e0e-145">supportsScopeTags</span></span>|<span data-ttu-id="e3e0e-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3e0e-146">Boolean</span></span>|<span data-ttu-id="e3e0e-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e3e0e-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e3e0e-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="e3e0e-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e3e0e-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="e3e0e-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e3e0e-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e3e0e-150">This property is read-only.</span></span> <span data-ttu-id="e3e0e-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e3e0e-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e3e0e-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e3e0e-152">createdDateTime</span></span>|<span data-ttu-id="e3e0e-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3e0e-153">DateTimeOffset</span></span>|<span data-ttu-id="e3e0e-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="e3e0e-154">DateTime the object was created.</span></span> <span data-ttu-id="e3e0e-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e3e0e-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e3e0e-156">description</span><span class="sxs-lookup"><span data-stu-id="e3e0e-156">description</span></span>|<span data-ttu-id="e3e0e-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e3e0e-157">String</span></span>|<span data-ttu-id="e3e0e-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="e3e0e-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e3e0e-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e3e0e-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e3e0e-160">displayName</span><span class="sxs-lookup"><span data-stu-id="e3e0e-160">displayName</span></span>|<span data-ttu-id="e3e0e-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e3e0e-161">String</span></span>|<span data-ttu-id="e3e0e-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="e3e0e-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e3e0e-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e3e0e-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e3e0e-164">Version</span><span class="sxs-lookup"><span data-stu-id="e3e0e-164">version</span></span>|<span data-ttu-id="e3e0e-165">Int32</span><span class="sxs-lookup"><span data-stu-id="e3e0e-165">Int32</span></span>|<span data-ttu-id="e3e0e-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="e3e0e-166">Version of the device configuration.</span></span> <span data-ttu-id="e3e0e-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e3e0e-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e3e0e-168">payloadName</span><span class="sxs-lookup"><span data-stu-id="e3e0e-168">payloadName</span></span>|<span data-ttu-id="e3e0e-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e3e0e-169">String</span></span>|<span data-ttu-id="e3e0e-170">Name, der dem Benutzer angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="e3e0e-170">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="e3e0e-171">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="e3e0e-171">payloadFileName</span></span>|<span data-ttu-id="e3e0e-172">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e3e0e-172">String</span></span>|<span data-ttu-id="e3e0e-173">Name der Nutzlastdatei (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="e3e0e-173">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="e3e0e-174">\*.xml)</span><span class="sxs-lookup"><span data-stu-id="e3e0e-174">\*.xml).</span></span>|
|<span data-ttu-id="e3e0e-175">payload</span><span class="sxs-lookup"><span data-stu-id="e3e0e-175">payload</span></span>|<span data-ttu-id="e3e0e-176">Binär</span><span class="sxs-lookup"><span data-stu-id="e3e0e-176">Binary</span></span>|<span data-ttu-id="e3e0e-177">Nutzlast</span><span class="sxs-lookup"><span data-stu-id="e3e0e-177">Payload.</span></span> <span data-ttu-id="e3e0e-178">(UTF8-codiertes Bytearray)</span><span class="sxs-lookup"><span data-stu-id="e3e0e-178">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="e3e0e-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="e3e0e-179">Response</span></span>
<span data-ttu-id="e3e0e-180">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e3e0e-180">If successful, this method returns a `201 Created` response code and a [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3e0e-181">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e3e0e-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="e3e0e-182">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e3e0e-182">Request</span></span>
<span data-ttu-id="e3e0e-183">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e3e0e-183">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e3e0e-184">Antwort</span><span class="sxs-lookup"><span data-stu-id="e3e0e-184">Response</span></span>
<span data-ttu-id="e3e0e-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e3e0e-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




