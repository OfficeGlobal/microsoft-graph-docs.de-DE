---
title: AndroidDeviceOwnerWiFiConfiguration aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AndroidDeviceOwnerWiFiConfiguration-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d102cac2a2e2b56a02b5be6027843fb71e7e375a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414473"
---
# <a name="update-androiddeviceownerwificonfiguration"></a><span data-ttu-id="3cccb-103">AndroidDeviceOwnerWiFiConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="3cccb-103">Update androidDeviceOwnerWiFiConfiguration</span></span>

> <span data-ttu-id="3cccb-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="3cccb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3cccb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3cccb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3cccb-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3cccb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3cccb-107">Aktualisieren Sie die Eigenschaften eines [AndroidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="3cccb-107">Update the properties of a [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3cccb-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3cccb-108">Prerequisites</span></span>
<span data-ttu-id="3cccb-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3cccb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3cccb-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3cccb-111">Permission type</span></span>|<span data-ttu-id="3cccb-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3cccb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3cccb-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3cccb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3cccb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cccb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3cccb-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3cccb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3cccb-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3cccb-116">Not supported.</span></span>|
|<span data-ttu-id="3cccb-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3cccb-117">Application</span></span>|<span data-ttu-id="3cccb-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3cccb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3cccb-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3cccb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="3cccb-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3cccb-120">Request headers</span></span>
|<span data-ttu-id="3cccb-121">Header</span><span class="sxs-lookup"><span data-stu-id="3cccb-121">Header</span></span>|<span data-ttu-id="3cccb-122">Wert</span><span class="sxs-lookup"><span data-stu-id="3cccb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3cccb-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="3cccb-123">Authorization</span></span>|<span data-ttu-id="3cccb-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3cccb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3cccb-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3cccb-125">Accept</span></span>|<span data-ttu-id="3cccb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3cccb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3cccb-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3cccb-127">Request body</span></span>
<span data-ttu-id="3cccb-128">Geben Sie im Textkörper Anforderung für das Objekt [AndroidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="3cccb-128">In the request body, supply a JSON representation for the [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object.</span></span>

<span data-ttu-id="3cccb-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [AndroidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="3cccb-129">The following table shows the properties that are required when you create the [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md).</span></span>

|<span data-ttu-id="3cccb-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3cccb-130">Property</span></span>|<span data-ttu-id="3cccb-131">Typ</span><span class="sxs-lookup"><span data-stu-id="3cccb-131">Type</span></span>|<span data-ttu-id="3cccb-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3cccb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3cccb-133">id</span><span class="sxs-lookup"><span data-stu-id="3cccb-133">id</span></span>|<span data-ttu-id="3cccb-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3cccb-134">String</span></span>|<span data-ttu-id="3cccb-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="3cccb-135">Key of the entity.</span></span> <span data-ttu-id="3cccb-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3cccb-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3cccb-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3cccb-137">lastModifiedDateTime</span></span>|<span data-ttu-id="3cccb-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3cccb-138">DateTimeOffset</span></span>|<span data-ttu-id="3cccb-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="3cccb-139">DateTime the object was last modified.</span></span> <span data-ttu-id="3cccb-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3cccb-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3cccb-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3cccb-141">roleScopeTagIds</span></span>|<span data-ttu-id="3cccb-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="3cccb-142">String collection</span></span>|<span data-ttu-id="3cccb-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="3cccb-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3cccb-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3cccb-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3cccb-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3cccb-145">supportsScopeTags</span></span>|<span data-ttu-id="3cccb-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="3cccb-146">Boolean</span></span>|<span data-ttu-id="3cccb-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3cccb-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3cccb-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="3cccb-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3cccb-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="3cccb-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3cccb-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="3cccb-150">This property is read-only.</span></span> <span data-ttu-id="3cccb-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3cccb-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3cccb-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3cccb-152">createdDateTime</span></span>|<span data-ttu-id="3cccb-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3cccb-153">DateTimeOffset</span></span>|<span data-ttu-id="3cccb-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="3cccb-154">DateTime the object was created.</span></span> <span data-ttu-id="3cccb-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3cccb-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3cccb-156">description</span><span class="sxs-lookup"><span data-stu-id="3cccb-156">description</span></span>|<span data-ttu-id="3cccb-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3cccb-157">String</span></span>|<span data-ttu-id="3cccb-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="3cccb-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3cccb-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3cccb-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3cccb-160">displayName</span><span class="sxs-lookup"><span data-stu-id="3cccb-160">displayName</span></span>|<span data-ttu-id="3cccb-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3cccb-161">String</span></span>|<span data-ttu-id="3cccb-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="3cccb-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3cccb-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3cccb-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3cccb-164">Version</span><span class="sxs-lookup"><span data-stu-id="3cccb-164">version</span></span>|<span data-ttu-id="3cccb-165">Int32</span><span class="sxs-lookup"><span data-stu-id="3cccb-165">Int32</span></span>|<span data-ttu-id="3cccb-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="3cccb-166">Version of the device configuration.</span></span> <span data-ttu-id="3cccb-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3cccb-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3cccb-168">Netzwerkname</span><span class="sxs-lookup"><span data-stu-id="3cccb-168">networkName</span></span>|<span data-ttu-id="3cccb-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3cccb-169">String</span></span>|<span data-ttu-id="3cccb-170">Netzwerkname</span><span class="sxs-lookup"><span data-stu-id="3cccb-170">Network Name</span></span>|
|<span data-ttu-id="3cccb-171">SSID</span><span class="sxs-lookup"><span data-stu-id="3cccb-171">ssid</span></span>|<span data-ttu-id="3cccb-172">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3cccb-172">String</span></span>|<span data-ttu-id="3cccb-173">Dies ist der Name des Netzwerks Wi-Fi, die an alle Geräte gesendet wird.</span><span class="sxs-lookup"><span data-stu-id="3cccb-173">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="3cccb-174">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="3cccb-174">connectAutomatically</span></span>|<span data-ttu-id="3cccb-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="3cccb-175">Boolean</span></span>|<span data-ttu-id="3cccb-176">Verbinden Sie automatisch, wenn dieses Netzwerk im Bereich befindet.</span><span class="sxs-lookup"><span data-stu-id="3cccb-176">Connect automatically when this network is in range.</span></span> <span data-ttu-id="3cccb-177">Eine Einstellung auf "true" überspringt die Aufforderung der Benutzer und automatisch mit Wi-Fi-Netzwerk verbinden.</span><span class="sxs-lookup"><span data-stu-id="3cccb-177">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="3cccb-178">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="3cccb-178">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="3cccb-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="3cccb-179">Boolean</span></span>|<span data-ttu-id="3cccb-180">Bei Festlegung auf true festgelegt ist, dieses Profil erzwingt, dass das Gerät für die Verbindung mit einem Netzwerk SSID nicht, die an alle Geräte seine.</span><span class="sxs-lookup"><span data-stu-id="3cccb-180">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="3cccb-181">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="3cccb-181">wiFiSecurityType</span></span>|[<span data-ttu-id="3cccb-182">androidDeviceOwnerWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="3cccb-182">androidDeviceOwnerWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androiddeviceownerwifisecuritytype.md)|<span data-ttu-id="3cccb-183">Gibt an, ob Wi-Fi-Endpunkt einen EAP-basierte Sicherheitstyp verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="3cccb-183">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="3cccb-184">Mögliche Werte sind: `open`, `wep` und `wpaPersonal`.</span><span class="sxs-lookup"><span data-stu-id="3cccb-184">Possible values are: `open`, `wep`, `wpaPersonal`.</span></span>|
|<span data-ttu-id="3cccb-185">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="3cccb-185">preSharedKey</span></span>|<span data-ttu-id="3cccb-186">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3cccb-186">String</span></span>|<span data-ttu-id="3cccb-187">Dies ist die vorinstallierten Schlüssel für WPA persönliche Wi-Fi-Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="3cccb-187">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="3cccb-188">preSharedKeyIsSet</span><span class="sxs-lookup"><span data-stu-id="3cccb-188">preSharedKeyIsSet</span></span>|<span data-ttu-id="3cccb-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="3cccb-189">Boolean</span></span>|<span data-ttu-id="3cccb-190">Dies ist die vorinstallierten Schlüssel für WPA persönliche Wi-Fi-Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="3cccb-190">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="3cccb-191">Antwort</span><span class="sxs-lookup"><span data-stu-id="3cccb-191">Response</span></span>
<span data-ttu-id="3cccb-192">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AndroidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="3cccb-192">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3cccb-193">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3cccb-193">Example</span></span>

### <a name="request"></a><span data-ttu-id="3cccb-194">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3cccb-194">Request</span></span>
<span data-ttu-id="3cccb-195">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3cccb-195">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="3cccb-196">Antwort</span><span class="sxs-lookup"><span data-stu-id="3cccb-196">Response</span></span>
<span data-ttu-id="3cccb-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3cccb-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




