---
title: Erstellen von „macOSCustomConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs macOSCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fb162edf796b14969eb6ba6efda5c3ea28ec06ce
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167235"
---
# <a name="create-macoscustomconfiguration"></a><span data-ttu-id="730b7-103">Erstellen von „macOSCustomConfiguration“</span><span class="sxs-lookup"><span data-stu-id="730b7-103">Create macOSCustomConfiguration</span></span>

> <span data-ttu-id="730b7-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="730b7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="730b7-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="730b7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="730b7-106">Diese Methode erstellt ein neues Objekt des Typs [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="730b7-106">Create a new [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="730b7-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="730b7-107">Prerequisites</span></span>
<span data-ttu-id="730b7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="730b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="730b7-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="730b7-110">Permission type</span></span>|<span data-ttu-id="730b7-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="730b7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="730b7-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="730b7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="730b7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="730b7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="730b7-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="730b7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="730b7-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="730b7-115">Not supported.</span></span>|
|<span data-ttu-id="730b7-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="730b7-116">Application</span></span>|<span data-ttu-id="730b7-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="730b7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="730b7-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="730b7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="730b7-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="730b7-119">Request headers</span></span>
|<span data-ttu-id="730b7-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="730b7-120">Header</span></span>|<span data-ttu-id="730b7-121">Wert</span><span class="sxs-lookup"><span data-stu-id="730b7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="730b7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="730b7-122">Authorization</span></span>|<span data-ttu-id="730b7-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="730b7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="730b7-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="730b7-124">Accept</span></span>|<span data-ttu-id="730b7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="730b7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="730b7-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="730b7-126">Request body</span></span>
<span data-ttu-id="730b7-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „macOSCustomConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="730b7-127">In the request body, supply a JSON representation for the macOSCustomConfiguration object.</span></span>

<span data-ttu-id="730b7-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „macOSCustomConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="730b7-128">The following table shows the properties that are required when you create the macOSCustomConfiguration.</span></span>

|<span data-ttu-id="730b7-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="730b7-129">Property</span></span>|<span data-ttu-id="730b7-130">Typ</span><span class="sxs-lookup"><span data-stu-id="730b7-130">Type</span></span>|<span data-ttu-id="730b7-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="730b7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="730b7-132">id</span><span class="sxs-lookup"><span data-stu-id="730b7-132">id</span></span>|<span data-ttu-id="730b7-133">string</span><span class="sxs-lookup"><span data-stu-id="730b7-133">String</span></span>|<span data-ttu-id="730b7-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="730b7-134">Key of the entity.</span></span> <span data-ttu-id="730b7-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="730b7-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="730b7-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="730b7-136">lastModifiedDateTime</span></span>|<span data-ttu-id="730b7-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="730b7-137">DateTimeOffset</span></span>|<span data-ttu-id="730b7-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="730b7-138">DateTime the object was last modified.</span></span> <span data-ttu-id="730b7-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="730b7-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="730b7-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="730b7-140">roleScopeTagIds</span></span>|<span data-ttu-id="730b7-141">String collection</span><span class="sxs-lookup"><span data-stu-id="730b7-141">String collection</span></span>|<span data-ttu-id="730b7-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="730b7-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="730b7-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="730b7-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="730b7-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="730b7-144">supportsScopeTags</span></span>|<span data-ttu-id="730b7-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="730b7-145">Boolean</span></span>|<span data-ttu-id="730b7-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="730b7-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="730b7-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="730b7-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="730b7-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="730b7-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="730b7-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="730b7-149">This property is read-only.</span></span> <span data-ttu-id="730b7-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="730b7-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="730b7-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="730b7-151">createdDateTime</span></span>|<span data-ttu-id="730b7-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="730b7-152">DateTimeOffset</span></span>|<span data-ttu-id="730b7-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="730b7-153">DateTime the object was created.</span></span> <span data-ttu-id="730b7-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="730b7-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="730b7-155">description</span><span class="sxs-lookup"><span data-stu-id="730b7-155">description</span></span>|<span data-ttu-id="730b7-156">String</span><span class="sxs-lookup"><span data-stu-id="730b7-156">String</span></span>|<span data-ttu-id="730b7-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="730b7-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="730b7-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="730b7-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="730b7-159">displayName</span><span class="sxs-lookup"><span data-stu-id="730b7-159">displayName</span></span>|<span data-ttu-id="730b7-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="730b7-160">String</span></span>|<span data-ttu-id="730b7-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="730b7-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="730b7-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="730b7-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="730b7-163">Version</span><span class="sxs-lookup"><span data-stu-id="730b7-163">version</span></span>|<span data-ttu-id="730b7-164">Int32</span><span class="sxs-lookup"><span data-stu-id="730b7-164">Int32</span></span>|<span data-ttu-id="730b7-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="730b7-165">Version of the device configuration.</span></span> <span data-ttu-id="730b7-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="730b7-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="730b7-167">payloadName</span><span class="sxs-lookup"><span data-stu-id="730b7-167">payloadName</span></span>|<span data-ttu-id="730b7-168">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="730b7-168">String</span></span>|<span data-ttu-id="730b7-169">Name, der dem Benutzer angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="730b7-169">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="730b7-170">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="730b7-170">payloadFileName</span></span>|<span data-ttu-id="730b7-171">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="730b7-171">String</span></span>|<span data-ttu-id="730b7-172">Name der Nutzlastdatei (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="730b7-172">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="730b7-173">\*.xml)</span><span class="sxs-lookup"><span data-stu-id="730b7-173">\*.xml).</span></span>|
|<span data-ttu-id="730b7-174">payload</span><span class="sxs-lookup"><span data-stu-id="730b7-174">payload</span></span>|<span data-ttu-id="730b7-175">Binär</span><span class="sxs-lookup"><span data-stu-id="730b7-175">Binary</span></span>|<span data-ttu-id="730b7-176">Nutzlast</span><span class="sxs-lookup"><span data-stu-id="730b7-176">Payload.</span></span> <span data-ttu-id="730b7-177">(UTF8-codiertes Bytearray)</span><span class="sxs-lookup"><span data-stu-id="730b7-177">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="730b7-178">Antwort</span><span class="sxs-lookup"><span data-stu-id="730b7-178">Response</span></span>
<span data-ttu-id="730b7-179">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="730b7-179">If successful, this method returns a `201 Created` response code and a [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="730b7-180">Beispiel</span><span class="sxs-lookup"><span data-stu-id="730b7-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="730b7-181">Anforderung</span><span class="sxs-lookup"><span data-stu-id="730b7-181">Request</span></span>
<span data-ttu-id="730b7-182">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="730b7-182">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 373

{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="730b7-183">Antwort</span><span class="sxs-lookup"><span data-stu-id="730b7-183">Response</span></span>
<span data-ttu-id="730b7-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="730b7-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 545

{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
  "id": "a253835d-835d-a253-5d83-53a25d8353a2",
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




