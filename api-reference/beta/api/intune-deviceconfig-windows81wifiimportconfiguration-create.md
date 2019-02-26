---
title: Windows81WifiImportConfiguration erstellen
description: Erstellen eines neuen windows81WifiImportConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0a4006be31fb792415d217e016474284a68c85af
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153536"
---
# <a name="create-windows81wifiimportconfiguration"></a><span data-ttu-id="17cd2-103">Windows81WifiImportConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="17cd2-103">Create windows81WifiImportConfiguration</span></span>

> <span data-ttu-id="17cd2-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="17cd2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17cd2-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="17cd2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17cd2-106">Erstellen eines neuen [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="17cd2-106">Create a new [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17cd2-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="17cd2-107">Prerequisites</span></span>
<span data-ttu-id="17cd2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="17cd2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="17cd2-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="17cd2-110">Permission type</span></span>|<span data-ttu-id="17cd2-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="17cd2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17cd2-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="17cd2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="17cd2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17cd2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="17cd2-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="17cd2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17cd2-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="17cd2-115">Not supported.</span></span>|
|<span data-ttu-id="17cd2-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="17cd2-116">Application</span></span>|<span data-ttu-id="17cd2-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="17cd2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="17cd2-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="17cd2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="17cd2-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="17cd2-119">Request headers</span></span>
|<span data-ttu-id="17cd2-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="17cd2-120">Header</span></span>|<span data-ttu-id="17cd2-121">Wert</span><span class="sxs-lookup"><span data-stu-id="17cd2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17cd2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="17cd2-122">Authorization</span></span>|<span data-ttu-id="17cd2-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="17cd2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17cd2-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="17cd2-124">Accept</span></span>|<span data-ttu-id="17cd2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="17cd2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17cd2-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="17cd2-126">Request body</span></span>
<span data-ttu-id="17cd2-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das windows81WifiImportConfiguration-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="17cd2-127">In the request body, supply a JSON representation for the windows81WifiImportConfiguration object.</span></span>

<span data-ttu-id="17cd2-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windows81WifiImportConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="17cd2-128">The following table shows the properties that are required when you create the windows81WifiImportConfiguration.</span></span>

|<span data-ttu-id="17cd2-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="17cd2-129">Property</span></span>|<span data-ttu-id="17cd2-130">Typ</span><span class="sxs-lookup"><span data-stu-id="17cd2-130">Type</span></span>|<span data-ttu-id="17cd2-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="17cd2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17cd2-132">id</span><span class="sxs-lookup"><span data-stu-id="17cd2-132">id</span></span>|<span data-ttu-id="17cd2-133">string</span><span class="sxs-lookup"><span data-stu-id="17cd2-133">String</span></span>|<span data-ttu-id="17cd2-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="17cd2-134">Key of the entity.</span></span> <span data-ttu-id="17cd2-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17cd2-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17cd2-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="17cd2-136">lastModifiedDateTime</span></span>|<span data-ttu-id="17cd2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17cd2-137">DateTimeOffset</span></span>|<span data-ttu-id="17cd2-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="17cd2-138">DateTime the object was last modified.</span></span> <span data-ttu-id="17cd2-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17cd2-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17cd2-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="17cd2-140">roleScopeTagIds</span></span>|<span data-ttu-id="17cd2-141">String collection</span><span class="sxs-lookup"><span data-stu-id="17cd2-141">String collection</span></span>|<span data-ttu-id="17cd2-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="17cd2-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="17cd2-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17cd2-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17cd2-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="17cd2-144">supportsScopeTags</span></span>|<span data-ttu-id="17cd2-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="17cd2-145">Boolean</span></span>|<span data-ttu-id="17cd2-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="17cd2-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="17cd2-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="17cd2-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="17cd2-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="17cd2-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="17cd2-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="17cd2-149">This property is read-only.</span></span> <span data-ttu-id="17cd2-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17cd2-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17cd2-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="17cd2-151">createdDateTime</span></span>|<span data-ttu-id="17cd2-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17cd2-152">DateTimeOffset</span></span>|<span data-ttu-id="17cd2-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="17cd2-153">DateTime the object was created.</span></span> <span data-ttu-id="17cd2-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17cd2-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17cd2-155">description</span><span class="sxs-lookup"><span data-stu-id="17cd2-155">description</span></span>|<span data-ttu-id="17cd2-156">String</span><span class="sxs-lookup"><span data-stu-id="17cd2-156">String</span></span>|<span data-ttu-id="17cd2-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="17cd2-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="17cd2-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17cd2-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17cd2-159">displayName</span><span class="sxs-lookup"><span data-stu-id="17cd2-159">displayName</span></span>|<span data-ttu-id="17cd2-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="17cd2-160">String</span></span>|<span data-ttu-id="17cd2-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="17cd2-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="17cd2-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17cd2-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17cd2-163">Version</span><span class="sxs-lookup"><span data-stu-id="17cd2-163">version</span></span>|<span data-ttu-id="17cd2-164">Int32</span><span class="sxs-lookup"><span data-stu-id="17cd2-164">Int32</span></span>|<span data-ttu-id="17cd2-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="17cd2-165">Version of the device configuration.</span></span> <span data-ttu-id="17cd2-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17cd2-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17cd2-167">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="17cd2-167">payloadFileName</span></span>|<span data-ttu-id="17cd2-168">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="17cd2-168">String</span></span>|<span data-ttu-id="17cd2-169">Name der Nutzlastdatei (\*. Xml).</span><span class="sxs-lookup"><span data-stu-id="17cd2-169">Payload file name (\*.xml).</span></span>|
|<span data-ttu-id="17cd2-170">Profilname</span><span class="sxs-lookup"><span data-stu-id="17cd2-170">profileName</span></span>|<span data-ttu-id="17cd2-171">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="17cd2-171">String</span></span>|<span data-ttu-id="17cd2-172">Der Profilname, der auf der Benutzeroberfläche angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="17cd2-172">Profile name displayed in the UI.</span></span>|
|<span data-ttu-id="17cd2-173">payload</span><span class="sxs-lookup"><span data-stu-id="17cd2-173">payload</span></span>|<span data-ttu-id="17cd2-174">Binär</span><span class="sxs-lookup"><span data-stu-id="17cd2-174">Binary</span></span>|<span data-ttu-id="17cd2-175">Nutzlast</span><span class="sxs-lookup"><span data-stu-id="17cd2-175">Payload.</span></span> <span data-ttu-id="17cd2-176">(UTF8-codiertes Bytearray).</span><span class="sxs-lookup"><span data-stu-id="17cd2-176">(UTF8 encoded byte array).</span></span> <span data-ttu-id="17cd2-177">Hierbei handelt es sich um die XML-Datei, die auf dem Gerät gespeichert ist, das Sie zum Herstellen einer Verbindung mit dem WLAN-Endpunkt verwendet haben.</span><span class="sxs-lookup"><span data-stu-id="17cd2-177">This is the XML file saved on the device you used to connect to the Wi-Fi endpoint.</span></span>|



## <a name="response"></a><span data-ttu-id="17cd2-178">Antwort</span><span class="sxs-lookup"><span data-stu-id="17cd2-178">Response</span></span>
<span data-ttu-id="17cd2-179">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="17cd2-179">If successful, this method returns a `201 Created` response code and a [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17cd2-180">Beispiel</span><span class="sxs-lookup"><span data-stu-id="17cd2-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="17cd2-181">Anforderung</span><span class="sxs-lookup"><span data-stu-id="17cd2-181">Request</span></span>
<span data-ttu-id="17cd2-182">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="17cd2-182">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 381

{
  "@odata.type": "#microsoft.graph.windows81WifiImportConfiguration",
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

### <a name="response"></a><span data-ttu-id="17cd2-183">Antwort</span><span class="sxs-lookup"><span data-stu-id="17cd2-183">Response</span></span>
<span data-ttu-id="17cd2-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="17cd2-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




