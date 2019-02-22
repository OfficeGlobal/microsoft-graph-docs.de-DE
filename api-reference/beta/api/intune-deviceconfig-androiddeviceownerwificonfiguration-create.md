---
title: AndroidDeviceOwnerWiFiConfiguration erstellen
description: Erstellen eines neuen androidDeviceOwnerWiFiConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7062e0bb32643474905d8c26921da6cb631b99b1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147523"
---
# <a name="create-androiddeviceownerwificonfiguration"></a><span data-ttu-id="77e47-103">AndroidDeviceOwnerWiFiConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="77e47-103">Create androidDeviceOwnerWiFiConfiguration</span></span>

> <span data-ttu-id="77e47-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="77e47-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77e47-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="77e47-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77e47-106">Erstellen eines neuen [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="77e47-106">Create a new [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77e47-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="77e47-107">Prerequisites</span></span>
<span data-ttu-id="77e47-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="77e47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="77e47-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="77e47-110">Permission type</span></span>|<span data-ttu-id="77e47-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="77e47-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77e47-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="77e47-112">Delegated (work or school account)</span></span>|<span data-ttu-id="77e47-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77e47-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="77e47-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="77e47-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77e47-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="77e47-115">Not supported.</span></span>|
|<span data-ttu-id="77e47-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="77e47-116">Application</span></span>|<span data-ttu-id="77e47-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="77e47-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="77e47-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="77e47-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="77e47-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="77e47-119">Request headers</span></span>
|<span data-ttu-id="77e47-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="77e47-120">Header</span></span>|<span data-ttu-id="77e47-121">Wert</span><span class="sxs-lookup"><span data-stu-id="77e47-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77e47-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="77e47-122">Authorization</span></span>|<span data-ttu-id="77e47-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="77e47-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77e47-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="77e47-124">Accept</span></span>|<span data-ttu-id="77e47-125">application/json</span><span class="sxs-lookup"><span data-stu-id="77e47-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77e47-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="77e47-126">Request body</span></span>
<span data-ttu-id="77e47-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das androidDeviceOwnerWiFiConfiguration-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="77e47-127">In the request body, supply a JSON representation for the androidDeviceOwnerWiFiConfiguration object.</span></span>

<span data-ttu-id="77e47-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der androidDeviceOwnerWiFiConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="77e47-128">The following table shows the properties that are required when you create the androidDeviceOwnerWiFiConfiguration.</span></span>

|<span data-ttu-id="77e47-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="77e47-129">Property</span></span>|<span data-ttu-id="77e47-130">Typ</span><span class="sxs-lookup"><span data-stu-id="77e47-130">Type</span></span>|<span data-ttu-id="77e47-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="77e47-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77e47-132">id</span><span class="sxs-lookup"><span data-stu-id="77e47-132">id</span></span>|<span data-ttu-id="77e47-133">string</span><span class="sxs-lookup"><span data-stu-id="77e47-133">String</span></span>|<span data-ttu-id="77e47-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="77e47-134">Key of the entity.</span></span> <span data-ttu-id="77e47-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77e47-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77e47-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="77e47-136">lastModifiedDateTime</span></span>|<span data-ttu-id="77e47-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77e47-137">DateTimeOffset</span></span>|<span data-ttu-id="77e47-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="77e47-138">DateTime the object was last modified.</span></span> <span data-ttu-id="77e47-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77e47-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77e47-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="77e47-140">roleScopeTagIds</span></span>|<span data-ttu-id="77e47-141">String collection</span><span class="sxs-lookup"><span data-stu-id="77e47-141">String collection</span></span>|<span data-ttu-id="77e47-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="77e47-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="77e47-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77e47-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77e47-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="77e47-144">supportsScopeTags</span></span>|<span data-ttu-id="77e47-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="77e47-145">Boolean</span></span>|<span data-ttu-id="77e47-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="77e47-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="77e47-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="77e47-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="77e47-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="77e47-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="77e47-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="77e47-149">This property is read-only.</span></span> <span data-ttu-id="77e47-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77e47-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77e47-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="77e47-151">createdDateTime</span></span>|<span data-ttu-id="77e47-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77e47-152">DateTimeOffset</span></span>|<span data-ttu-id="77e47-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="77e47-153">DateTime the object was created.</span></span> <span data-ttu-id="77e47-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77e47-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77e47-155">description</span><span class="sxs-lookup"><span data-stu-id="77e47-155">description</span></span>|<span data-ttu-id="77e47-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="77e47-156">String</span></span>|<span data-ttu-id="77e47-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="77e47-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="77e47-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77e47-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77e47-159">displayName</span><span class="sxs-lookup"><span data-stu-id="77e47-159">displayName</span></span>|<span data-ttu-id="77e47-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="77e47-160">String</span></span>|<span data-ttu-id="77e47-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="77e47-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="77e47-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77e47-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77e47-163">Version</span><span class="sxs-lookup"><span data-stu-id="77e47-163">version</span></span>|<span data-ttu-id="77e47-164">Int32</span><span class="sxs-lookup"><span data-stu-id="77e47-164">Int32</span></span>|<span data-ttu-id="77e47-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="77e47-165">Version of the device configuration.</span></span> <span data-ttu-id="77e47-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77e47-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77e47-167">networkName</span><span class="sxs-lookup"><span data-stu-id="77e47-167">networkName</span></span>|<span data-ttu-id="77e47-168">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="77e47-168">String</span></span>|<span data-ttu-id="77e47-169">Netzwerk Name</span><span class="sxs-lookup"><span data-stu-id="77e47-169">Network Name</span></span>|
|<span data-ttu-id="77e47-170">SSID</span><span class="sxs-lookup"><span data-stu-id="77e47-170">ssid</span></span>|<span data-ttu-id="77e47-171">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="77e47-171">String</span></span>|<span data-ttu-id="77e47-172">Dies ist der Name des WLAN-Netzwerks, das auf alle Geräte übertragen wird.</span><span class="sxs-lookup"><span data-stu-id="77e47-172">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="77e47-173">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="77e47-173">connectAutomatically</span></span>|<span data-ttu-id="77e47-174">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="77e47-174">Boolean</span></span>|<span data-ttu-id="77e47-175">Verbinden Sie sich automatisch, wenn sich dieses Netzwerk in Reichweite befindet.</span><span class="sxs-lookup"><span data-stu-id="77e47-175">Connect automatically when this network is in range.</span></span> <span data-ttu-id="77e47-176">Wenn Sie diesen Wert auf true festlegen, wird die Benutzereingabe übersprungen, und das Gerät wird automatisch mit dem WLAN verbunden.</span><span class="sxs-lookup"><span data-stu-id="77e47-176">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="77e47-177">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="77e47-177">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="77e47-178">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="77e47-178">Boolean</span></span>|<span data-ttu-id="77e47-179">Wenn dieser Wert auf "true" festgelegt ist, wird das Gerät gezwungen, eine Verbindung mit einem Netzwerk herzustellen, das seine SSID nicht auf alle Geräte übermittelt.</span><span class="sxs-lookup"><span data-stu-id="77e47-179">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="77e47-180">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="77e47-180">wiFiSecurityType</span></span>|[<span data-ttu-id="77e47-181">androidDeviceOwnerWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="77e47-181">androidDeviceOwnerWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androiddeviceownerwifisecuritytype.md)|<span data-ttu-id="77e47-182">Gibt an, ob der WLAN-Endpunkt einen EAP-basierten Sicherheitstyp verwendet.</span><span class="sxs-lookup"><span data-stu-id="77e47-182">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="77e47-183">Mögliche Werte sind: `open`, `wep` und `wpaPersonal`.</span><span class="sxs-lookup"><span data-stu-id="77e47-183">Possible values are: `open`, `wep`, `wpaPersonal`.</span></span>|
|<span data-ttu-id="77e47-184">PresharedKey wurde</span><span class="sxs-lookup"><span data-stu-id="77e47-184">preSharedKey</span></span>|<span data-ttu-id="77e47-185">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="77e47-185">String</span></span>|<span data-ttu-id="77e47-186">Dies ist der vorinstallierte Schlüssel für ein persönliches WPA-Wi-Fi-Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="77e47-186">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="77e47-187">preSharedKeyIsSet</span><span class="sxs-lookup"><span data-stu-id="77e47-187">preSharedKeyIsSet</span></span>|<span data-ttu-id="77e47-188">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="77e47-188">Boolean</span></span>|<span data-ttu-id="77e47-189">Dies ist der vorinstallierte Schlüssel für ein persönliches WPA-Wi-Fi-Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="77e47-189">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="77e47-190">Antwort</span><span class="sxs-lookup"><span data-stu-id="77e47-190">Response</span></span>
<span data-ttu-id="77e47-191">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="77e47-191">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77e47-192">Beispiel</span><span class="sxs-lookup"><span data-stu-id="77e47-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="77e47-193">Anforderung</span><span class="sxs-lookup"><span data-stu-id="77e47-193">Request</span></span>
<span data-ttu-id="77e47-194">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="77e47-194">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 509

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerWiFiConfiguration",
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
  "wiFiSecurityType": "wep",
  "preSharedKey": "Pre Shared Key value",
  "preSharedKeyIsSet": true
}
```

### <a name="response"></a><span data-ttu-id="77e47-195">Antwort</span><span class="sxs-lookup"><span data-stu-id="77e47-195">Response</span></span>
<span data-ttu-id="77e47-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="77e47-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 681

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerWiFiConfiguration",
  "id": "8d25beba-beba-8d25-babe-258dbabe258d",
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
  "wiFiSecurityType": "wep",
  "preSharedKey": "Pre Shared Key value",
  "preSharedKeyIsSet": true
}
```




