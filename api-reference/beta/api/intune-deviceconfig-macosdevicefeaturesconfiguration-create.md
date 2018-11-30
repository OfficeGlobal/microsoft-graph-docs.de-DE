---
title: Erstellen von „macOSDeviceFeaturesConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs macOSDeviceFeaturesConfiguration.
ms.openlocfilehash: 5bd8bda5b019fee81a50c117218264975883461a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060461"
---
# <a name="create-macosdevicefeaturesconfiguration"></a><span data-ttu-id="019b7-103">Erstellen von „macOSDeviceFeaturesConfiguration“</span><span class="sxs-lookup"><span data-stu-id="019b7-103">Create macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="019b7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="019b7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="019b7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="019b7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="019b7-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="019b7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="019b7-107">Diese Methode erstellt ein neues Objekt des Typs [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="019b7-107">Create a new [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="019b7-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="019b7-108">Prerequisites</span></span>
<span data-ttu-id="019b7-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="019b7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="019b7-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="019b7-111">Permission type</span></span>|<span data-ttu-id="019b7-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="019b7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="019b7-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="019b7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="019b7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="019b7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="019b7-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="019b7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="019b7-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="019b7-116">Not supported.</span></span>|
|<span data-ttu-id="019b7-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="019b7-117">Application</span></span>|<span data-ttu-id="019b7-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="019b7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="019b7-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="019b7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="019b7-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="019b7-120">Request headers</span></span>
|<span data-ttu-id="019b7-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="019b7-121">Header</span></span>|<span data-ttu-id="019b7-122">Wert</span><span class="sxs-lookup"><span data-stu-id="019b7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="019b7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="019b7-123">Authorization</span></span>|<span data-ttu-id="019b7-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="019b7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="019b7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="019b7-125">Accept</span></span>|<span data-ttu-id="019b7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="019b7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="019b7-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="019b7-127">Request body</span></span>
<span data-ttu-id="019b7-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „macOSDeviceFeaturesConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="019b7-128">In the request body, supply a JSON representation for the macOSDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="019b7-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „macOSDeviceFeaturesConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="019b7-129">The following table shows the properties that are required when you create the macOSDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="019b7-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="019b7-130">Property</span></span>|<span data-ttu-id="019b7-131">Typ</span><span class="sxs-lookup"><span data-stu-id="019b7-131">Type</span></span>|<span data-ttu-id="019b7-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="019b7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="019b7-133">id</span><span class="sxs-lookup"><span data-stu-id="019b7-133">id</span></span>|<span data-ttu-id="019b7-134">String</span><span class="sxs-lookup"><span data-stu-id="019b7-134">String</span></span>|<span data-ttu-id="019b7-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="019b7-135">Key of the entity.</span></span> <span data-ttu-id="019b7-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="019b7-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="019b7-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="019b7-137">lastModifiedDateTime</span></span>|<span data-ttu-id="019b7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="019b7-138">DateTimeOffset</span></span>|<span data-ttu-id="019b7-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="019b7-139">DateTime the object was last modified.</span></span> <span data-ttu-id="019b7-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="019b7-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="019b7-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="019b7-141">roleScopeTagIds</span></span>|<span data-ttu-id="019b7-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="019b7-142">String collection</span></span>|<span data-ttu-id="019b7-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="019b7-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="019b7-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="019b7-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="019b7-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="019b7-145">supportsScopeTags</span></span>|<span data-ttu-id="019b7-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="019b7-146">Boolean</span></span>|<span data-ttu-id="019b7-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="019b7-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="019b7-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="019b7-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="019b7-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="019b7-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="019b7-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="019b7-150">This property is read-only.</span></span> <span data-ttu-id="019b7-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="019b7-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="019b7-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="019b7-152">createdDateTime</span></span>|<span data-ttu-id="019b7-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="019b7-153">DateTimeOffset</span></span>|<span data-ttu-id="019b7-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="019b7-154">DateTime the object was created.</span></span> <span data-ttu-id="019b7-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="019b7-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="019b7-156">description</span><span class="sxs-lookup"><span data-stu-id="019b7-156">description</span></span>|<span data-ttu-id="019b7-157">String</span><span class="sxs-lookup"><span data-stu-id="019b7-157">String</span></span>|<span data-ttu-id="019b7-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="019b7-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="019b7-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="019b7-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="019b7-160">displayName</span><span class="sxs-lookup"><span data-stu-id="019b7-160">displayName</span></span>|<span data-ttu-id="019b7-161">String</span><span class="sxs-lookup"><span data-stu-id="019b7-161">String</span></span>|<span data-ttu-id="019b7-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="019b7-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="019b7-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="019b7-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="019b7-164">Version</span><span class="sxs-lookup"><span data-stu-id="019b7-164">version</span></span>|<span data-ttu-id="019b7-165">Int32</span><span class="sxs-lookup"><span data-stu-id="019b7-165">Int32</span></span>|<span data-ttu-id="019b7-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="019b7-166">Version of the device configuration.</span></span> <span data-ttu-id="019b7-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="019b7-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="019b7-168">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="019b7-168">airPrintDestinations</span></span>|<span data-ttu-id="019b7-169">[AirPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="019b7-169">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="019b7-170">Ein Array von AirPrint aus, die immer angezeigt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="019b7-170">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="019b7-171">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="019b7-171">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="019b7-172">Geerbt von [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="019b7-172">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|



## <a name="response"></a><span data-ttu-id="019b7-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="019b7-173">Response</span></span>
<span data-ttu-id="019b7-174">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="019b7-174">If successful, this method returns a `201 Created` response code and a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="019b7-175">Beispiel</span><span class="sxs-lookup"><span data-stu-id="019b7-175">Example</span></span>
### <a name="request"></a><span data-ttu-id="019b7-176">Anforderung</span><span class="sxs-lookup"><span data-stu-id="019b7-176">Request</span></span>
<span data-ttu-id="019b7-177">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="019b7-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 564

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "airPrintDestinations": [
    {
      "@odata.type": "microsoft.graph.airPrintDestination",
      "ipAddress": "Ip Address value",
      "resourcePath": "Resource Path value",
      "port": 4,
      "forceTls": true
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="019b7-178">Antwort</span><span class="sxs-lookup"><span data-stu-id="019b7-178">Response</span></span>
<span data-ttu-id="019b7-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="019b7-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 672

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "id": "49fa957d-957d-49fa-7d95-fa497d95fa49",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "airPrintDestinations": [
    {
      "@odata.type": "microsoft.graph.airPrintDestination",
      "ipAddress": "Ip Address value",
      "resourcePath": "Resource Path value",
      "port": 4,
      "forceTls": true
    }
  ]
}
```





