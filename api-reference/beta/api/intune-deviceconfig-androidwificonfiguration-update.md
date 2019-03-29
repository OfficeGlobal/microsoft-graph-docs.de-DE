---
title: AndroidWiFiConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines androidWiFiConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 60736e87ece7b9e54829d6b556816d52e7f5744a
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30957857"
---
# <a name="update-androidwificonfiguration"></a><span data-ttu-id="54be1-103">AndroidWiFiConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="54be1-103">Update androidWiFiConfiguration</span></span>

> <span data-ttu-id="54be1-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="54be1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54be1-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="54be1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54be1-106">Aktualisieren der Eigenschaften eines [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="54be1-106">Update the properties of a [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54be1-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="54be1-107">Prerequisites</span></span>
<span data-ttu-id="54be1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54be1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54be1-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="54be1-110">Permission type</span></span>|<span data-ttu-id="54be1-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="54be1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54be1-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="54be1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="54be1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54be1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="54be1-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="54be1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54be1-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="54be1-115">Not supported.</span></span>|
|<span data-ttu-id="54be1-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="54be1-116">Application</span></span>|<span data-ttu-id="54be1-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="54be1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="54be1-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="54be1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="54be1-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="54be1-119">Request headers</span></span>
|<span data-ttu-id="54be1-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="54be1-120">Header</span></span>|<span data-ttu-id="54be1-121">Wert</span><span class="sxs-lookup"><span data-stu-id="54be1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54be1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="54be1-122">Authorization</span></span>|<span data-ttu-id="54be1-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="54be1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54be1-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="54be1-124">Accept</span></span>|<span data-ttu-id="54be1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="54be1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54be1-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="54be1-126">Request body</span></span>
<span data-ttu-id="54be1-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="54be1-127">In the request body, supply a JSON representation for the [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object.</span></span>

<span data-ttu-id="54be1-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="54be1-128">The following table shows the properties that are required when you create the [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md).</span></span>

|<span data-ttu-id="54be1-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="54be1-129">Property</span></span>|<span data-ttu-id="54be1-130">Typ</span><span class="sxs-lookup"><span data-stu-id="54be1-130">Type</span></span>|<span data-ttu-id="54be1-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="54be1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54be1-132">id</span><span class="sxs-lookup"><span data-stu-id="54be1-132">id</span></span>|<span data-ttu-id="54be1-133">String</span><span class="sxs-lookup"><span data-stu-id="54be1-133">String</span></span>|<span data-ttu-id="54be1-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="54be1-134">Key of the entity.</span></span> <span data-ttu-id="54be1-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54be1-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54be1-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="54be1-136">lastModifiedDateTime</span></span>|<span data-ttu-id="54be1-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54be1-137">DateTimeOffset</span></span>|<span data-ttu-id="54be1-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="54be1-138">DateTime the object was last modified.</span></span> <span data-ttu-id="54be1-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54be1-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54be1-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="54be1-140">roleScopeTagIds</span></span>|<span data-ttu-id="54be1-141">String collection</span><span class="sxs-lookup"><span data-stu-id="54be1-141">String collection</span></span>|<span data-ttu-id="54be1-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="54be1-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="54be1-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54be1-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54be1-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="54be1-144">supportsScopeTags</span></span>|<span data-ttu-id="54be1-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="54be1-145">Boolean</span></span>|<span data-ttu-id="54be1-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="54be1-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="54be1-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="54be1-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="54be1-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="54be1-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="54be1-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="54be1-149">This property is read-only.</span></span> <span data-ttu-id="54be1-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54be1-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54be1-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="54be1-151">createdDateTime</span></span>|<span data-ttu-id="54be1-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54be1-152">DateTimeOffset</span></span>|<span data-ttu-id="54be1-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="54be1-153">DateTime the object was created.</span></span> <span data-ttu-id="54be1-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54be1-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54be1-155">description</span><span class="sxs-lookup"><span data-stu-id="54be1-155">description</span></span>|<span data-ttu-id="54be1-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="54be1-156">String</span></span>|<span data-ttu-id="54be1-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="54be1-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="54be1-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54be1-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54be1-159">displayName</span><span class="sxs-lookup"><span data-stu-id="54be1-159">displayName</span></span>|<span data-ttu-id="54be1-160">String</span><span class="sxs-lookup"><span data-stu-id="54be1-160">String</span></span>|<span data-ttu-id="54be1-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="54be1-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="54be1-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54be1-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54be1-163">Version</span><span class="sxs-lookup"><span data-stu-id="54be1-163">version</span></span>|<span data-ttu-id="54be1-164">Int32</span><span class="sxs-lookup"><span data-stu-id="54be1-164">Int32</span></span>|<span data-ttu-id="54be1-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="54be1-165">Version of the device configuration.</span></span> <span data-ttu-id="54be1-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54be1-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54be1-167">networkName</span><span class="sxs-lookup"><span data-stu-id="54be1-167">networkName</span></span>|<span data-ttu-id="54be1-168">String</span><span class="sxs-lookup"><span data-stu-id="54be1-168">String</span></span>|<span data-ttu-id="54be1-169">Netzwerk Name</span><span class="sxs-lookup"><span data-stu-id="54be1-169">Network Name</span></span>|
|<span data-ttu-id="54be1-170">SSID</span><span class="sxs-lookup"><span data-stu-id="54be1-170">ssid</span></span>|<span data-ttu-id="54be1-171">String</span><span class="sxs-lookup"><span data-stu-id="54be1-171">String</span></span>|<span data-ttu-id="54be1-172">Dies ist der Name des WLAN-Netzwerks, das auf alle Geräte übertragen wird.</span><span class="sxs-lookup"><span data-stu-id="54be1-172">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="54be1-173">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="54be1-173">connectAutomatically</span></span>|<span data-ttu-id="54be1-174">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="54be1-174">Boolean</span></span>|<span data-ttu-id="54be1-175">Verbinden Sie sich automatisch, wenn sich dieses Netzwerk in Reichweite befindet.</span><span class="sxs-lookup"><span data-stu-id="54be1-175">Connect automatically when this network is in range.</span></span> <span data-ttu-id="54be1-176">Wenn Sie diesen Wert auf true festlegen, wird die Benutzereingabe übersprungen, und das Gerät wird automatisch mit dem WLAN verbunden.</span><span class="sxs-lookup"><span data-stu-id="54be1-176">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="54be1-177">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="54be1-177">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="54be1-178">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="54be1-178">Boolean</span></span>|<span data-ttu-id="54be1-179">Wenn dieser Wert auf "true" festgelegt ist, wird das Gerät gezwungen, eine Verbindung mit einem Netzwerk herzustellen, das seine SSID nicht auf alle Geräte übermittelt.</span><span class="sxs-lookup"><span data-stu-id="54be1-179">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="54be1-180">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="54be1-180">wiFiSecurityType</span></span>|[<span data-ttu-id="54be1-181">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="54be1-181">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="54be1-182">Gibt an, ob der WLAN-Endpunkt einen EAP-basierten Sicherheitstyp verwendet.</span><span class="sxs-lookup"><span data-stu-id="54be1-182">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="54be1-183">Mögliche Werte sind: `open` und `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="54be1-183">Possible values are: `open`, `wpaEnterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="54be1-184">Antwort</span><span class="sxs-lookup"><span data-stu-id="54be1-184">Response</span></span>
<span data-ttu-id="54be1-185">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="54be1-185">If successful, this method returns a `200 OK` response code and an updated [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54be1-186">Beispiel</span><span class="sxs-lookup"><span data-stu-id="54be1-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="54be1-187">Anforderung</span><span class="sxs-lookup"><span data-stu-id="54be1-187">Request</span></span>
<span data-ttu-id="54be1-188">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="54be1-188">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 435

{
  "@odata.type": "#microsoft.graph.androidWiFiConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaEnterprise"
}
```

### <a name="response"></a><span data-ttu-id="54be1-189">Antwort</span><span class="sxs-lookup"><span data-stu-id="54be1-189">Response</span></span>
<span data-ttu-id="54be1-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="54be1-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 607

{
  "@odata.type": "#microsoft.graph.androidWiFiConfiguration",
  "id": "51cfd26f-d26f-51cf-6fd2-cf516fd2cf51",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaEnterprise"
}
```




