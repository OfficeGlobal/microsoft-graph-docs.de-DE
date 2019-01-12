---
title: Windows81WifiImportConfiguration aktualisieren
description: Aktualisieren Sie die Eigenschaften eines windows81WifiImportConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 139a7d5df0227dfcf002f484a975b6d78227107f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914374"
---
# <a name="update-windows81wifiimportconfiguration"></a><span data-ttu-id="c1d83-103">Windows81WifiImportConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="c1d83-103">Update windows81WifiImportConfiguration</span></span>

> <span data-ttu-id="c1d83-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c1d83-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c1d83-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c1d83-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c1d83-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c1d83-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c1d83-107">Aktualisieren Sie die Eigenschaften eines [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c1d83-107">Update the properties of a [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c1d83-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c1d83-108">Prerequisites</span></span>
<span data-ttu-id="c1d83-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1d83-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1d83-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c1d83-111">Permission type</span></span>|<span data-ttu-id="c1d83-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c1d83-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1d83-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c1d83-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c1d83-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1d83-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c1d83-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c1d83-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1d83-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c1d83-116">Not supported.</span></span>|
|<span data-ttu-id="c1d83-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c1d83-117">Application</span></span>|<span data-ttu-id="c1d83-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c1d83-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1d83-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1d83-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c1d83-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c1d83-120">Request headers</span></span>
|<span data-ttu-id="c1d83-121">Header</span><span class="sxs-lookup"><span data-stu-id="c1d83-121">Header</span></span>|<span data-ttu-id="c1d83-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c1d83-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1d83-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1d83-123">Authorization</span></span>|<span data-ttu-id="c1d83-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c1d83-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1d83-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c1d83-125">Accept</span></span>|<span data-ttu-id="c1d83-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c1d83-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1d83-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c1d83-127">Request body</span></span>
<span data-ttu-id="c1d83-128">Geben Sie im Textkörper Anforderung für das Objekt [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="c1d83-128">In the request body, supply a JSON representation for the [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object.</span></span>

<span data-ttu-id="c1d83-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="c1d83-129">The following table shows the properties that are required when you create the [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md).</span></span>

|<span data-ttu-id="c1d83-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c1d83-130">Property</span></span>|<span data-ttu-id="c1d83-131">Typ</span><span class="sxs-lookup"><span data-stu-id="c1d83-131">Type</span></span>|<span data-ttu-id="c1d83-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c1d83-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1d83-133">id</span><span class="sxs-lookup"><span data-stu-id="c1d83-133">id</span></span>|<span data-ttu-id="c1d83-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1d83-134">String</span></span>|<span data-ttu-id="c1d83-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c1d83-135">Key of the entity.</span></span> <span data-ttu-id="c1d83-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1d83-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1d83-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c1d83-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c1d83-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1d83-138">DateTimeOffset</span></span>|<span data-ttu-id="c1d83-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="c1d83-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c1d83-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1d83-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1d83-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c1d83-141">roleScopeTagIds</span></span>|<span data-ttu-id="c1d83-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="c1d83-142">String collection</span></span>|<span data-ttu-id="c1d83-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="c1d83-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c1d83-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1d83-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1d83-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c1d83-145">supportsScopeTags</span></span>|<span data-ttu-id="c1d83-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c1d83-146">Boolean</span></span>|<span data-ttu-id="c1d83-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c1d83-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c1d83-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="c1d83-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c1d83-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="c1d83-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c1d83-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c1d83-150">This property is read-only.</span></span> <span data-ttu-id="c1d83-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1d83-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1d83-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c1d83-152">createdDateTime</span></span>|<span data-ttu-id="c1d83-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1d83-153">DateTimeOffset</span></span>|<span data-ttu-id="c1d83-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="c1d83-154">DateTime the object was created.</span></span> <span data-ttu-id="c1d83-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1d83-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1d83-156">description</span><span class="sxs-lookup"><span data-stu-id="c1d83-156">description</span></span>|<span data-ttu-id="c1d83-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1d83-157">String</span></span>|<span data-ttu-id="c1d83-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="c1d83-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c1d83-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1d83-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1d83-160">displayName</span><span class="sxs-lookup"><span data-stu-id="c1d83-160">displayName</span></span>|<span data-ttu-id="c1d83-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1d83-161">String</span></span>|<span data-ttu-id="c1d83-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="c1d83-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c1d83-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1d83-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1d83-164">Version</span><span class="sxs-lookup"><span data-stu-id="c1d83-164">version</span></span>|<span data-ttu-id="c1d83-165">Int32</span><span class="sxs-lookup"><span data-stu-id="c1d83-165">Int32</span></span>|<span data-ttu-id="c1d83-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="c1d83-166">Version of the device configuration.</span></span> <span data-ttu-id="c1d83-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1d83-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1d83-168">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="c1d83-168">payloadFileName</span></span>|<span data-ttu-id="c1d83-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1d83-169">String</span></span>|<span data-ttu-id="c1d83-170">Name der Nutzlast (\*.XML).</span><span class="sxs-lookup"><span data-stu-id="c1d83-170">Payload file name (\*.xml).</span></span>|
|<span data-ttu-id="c1d83-171">Profilname</span><span class="sxs-lookup"><span data-stu-id="c1d83-171">profileName</span></span>|<span data-ttu-id="c1d83-172">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1d83-172">String</span></span>|<span data-ttu-id="c1d83-173">Name der Benutzerprofildienst in der Benutzeroberfläche angezeigt.</span><span class="sxs-lookup"><span data-stu-id="c1d83-173">Profile name displayed in the UI.</span></span>|
|<span data-ttu-id="c1d83-174">payload</span><span class="sxs-lookup"><span data-stu-id="c1d83-174">payload</span></span>|<span data-ttu-id="c1d83-175">Binär</span><span class="sxs-lookup"><span data-stu-id="c1d83-175">Binary</span></span>|<span data-ttu-id="c1d83-176">Nutzlast</span><span class="sxs-lookup"><span data-stu-id="c1d83-176">Payload.</span></span> <span data-ttu-id="c1d83-177">(UTF8 codiert Byte-Array).</span><span class="sxs-lookup"><span data-stu-id="c1d83-177">(UTF8 encoded byte array).</span></span> <span data-ttu-id="c1d83-178">Dies ist der XML-Datei gespeichert haben, auf dem Gerät, die, das Sie an den Endpunkt Wi-Fi-Verbindung verwendet.</span><span class="sxs-lookup"><span data-stu-id="c1d83-178">This is the XML file saved on the device you used to connect to the Wi-Fi endpoint.</span></span>|



## <a name="response"></a><span data-ttu-id="c1d83-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1d83-179">Response</span></span>
<span data-ttu-id="c1d83-180">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="c1d83-180">If successful, this method returns a `200 OK` response code and an updated [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1d83-181">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c1d83-181">Example</span></span>
### <a name="request"></a><span data-ttu-id="c1d83-182">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1d83-182">Request</span></span>
<span data-ttu-id="c1d83-183">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c1d83-183">Here is an example of the request.</span></span>
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
  "payloadFileName": "Payload File Name value",
  "profileName": "Profile Name value",
  "payload": "cGF5bG9hZA=="
}
```

### <a name="response"></a><span data-ttu-id="c1d83-184">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1d83-184">Response</span></span>
<span data-ttu-id="c1d83-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c1d83-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 553

{
  "@odata.type": "#microsoft.graph.windows81WifiImportConfiguration",
  "id": "534a2f07-2f07-534a-072f-4a53072f4a53",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadFileName": "Payload File Name value",
  "profileName": "Profile Name value",
  "payload": "cGF5bG9hZA=="
}
```





