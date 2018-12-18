---
title: AndroidWorkProfileWiFiConfiguration aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AndroidWorkProfileWiFiConfiguration-Objekts.
author: tfitzmac
ms.openlocfilehash: 8a14017d7af930e33ad2be4d42e451dd306eac17
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27363711"
---
# <a name="update-androidworkprofilewificonfiguration"></a><span data-ttu-id="0da90-103">AndroidWorkProfileWiFiConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0da90-103">Update androidWorkProfileWiFiConfiguration</span></span>

> <span data-ttu-id="0da90-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0da90-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0da90-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0da90-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0da90-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0da90-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0da90-107">Aktualisieren Sie die Eigenschaften eines [AndroidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="0da90-107">Update the properties of a [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0da90-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0da90-108">Prerequisites</span></span>
<span data-ttu-id="0da90-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0da90-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0da90-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0da90-111">Permission type</span></span>|<span data-ttu-id="0da90-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0da90-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0da90-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0da90-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0da90-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0da90-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0da90-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0da90-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0da90-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0da90-116">Not supported.</span></span>|
|<span data-ttu-id="0da90-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0da90-117">Application</span></span>|<span data-ttu-id="0da90-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0da90-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0da90-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0da90-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0da90-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0da90-120">Request headers</span></span>
|<span data-ttu-id="0da90-121">Header</span><span class="sxs-lookup"><span data-stu-id="0da90-121">Header</span></span>|<span data-ttu-id="0da90-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0da90-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0da90-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="0da90-123">Authorization</span></span>|<span data-ttu-id="0da90-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0da90-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0da90-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0da90-125">Accept</span></span>|<span data-ttu-id="0da90-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0da90-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0da90-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0da90-127">Request body</span></span>
<span data-ttu-id="0da90-128">Geben Sie im Textkörper Anforderung für das Objekt [AndroidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="0da90-128">In the request body, supply a JSON representation for the [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) object.</span></span>

<span data-ttu-id="0da90-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [AndroidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="0da90-129">The following table shows the properties that are required when you create the [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md).</span></span>

|<span data-ttu-id="0da90-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0da90-130">Property</span></span>|<span data-ttu-id="0da90-131">Typ</span><span class="sxs-lookup"><span data-stu-id="0da90-131">Type</span></span>|<span data-ttu-id="0da90-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0da90-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0da90-133">id</span><span class="sxs-lookup"><span data-stu-id="0da90-133">id</span></span>|<span data-ttu-id="0da90-134">String</span><span class="sxs-lookup"><span data-stu-id="0da90-134">String</span></span>|<span data-ttu-id="0da90-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="0da90-135">Key of the entity.</span></span> <span data-ttu-id="0da90-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0da90-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0da90-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0da90-137">lastModifiedDateTime</span></span>|<span data-ttu-id="0da90-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0da90-138">DateTimeOffset</span></span>|<span data-ttu-id="0da90-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="0da90-139">DateTime the object was last modified.</span></span> <span data-ttu-id="0da90-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0da90-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0da90-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0da90-141">roleScopeTagIds</span></span>|<span data-ttu-id="0da90-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="0da90-142">String collection</span></span>|<span data-ttu-id="0da90-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="0da90-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0da90-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0da90-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0da90-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0da90-145">supportsScopeTags</span></span>|<span data-ttu-id="0da90-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="0da90-146">Boolean</span></span>|<span data-ttu-id="0da90-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0da90-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0da90-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="0da90-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0da90-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="0da90-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0da90-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0da90-150">This property is read-only.</span></span> <span data-ttu-id="0da90-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0da90-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0da90-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0da90-152">createdDateTime</span></span>|<span data-ttu-id="0da90-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0da90-153">DateTimeOffset</span></span>|<span data-ttu-id="0da90-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="0da90-154">DateTime the object was created.</span></span> <span data-ttu-id="0da90-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0da90-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0da90-156">description</span><span class="sxs-lookup"><span data-stu-id="0da90-156">description</span></span>|<span data-ttu-id="0da90-157">String</span><span class="sxs-lookup"><span data-stu-id="0da90-157">String</span></span>|<span data-ttu-id="0da90-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="0da90-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0da90-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0da90-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0da90-160">displayName</span><span class="sxs-lookup"><span data-stu-id="0da90-160">displayName</span></span>|<span data-ttu-id="0da90-161">String</span><span class="sxs-lookup"><span data-stu-id="0da90-161">String</span></span>|<span data-ttu-id="0da90-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="0da90-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0da90-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0da90-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0da90-164">Version</span><span class="sxs-lookup"><span data-stu-id="0da90-164">version</span></span>|<span data-ttu-id="0da90-165">Int32</span><span class="sxs-lookup"><span data-stu-id="0da90-165">Int32</span></span>|<span data-ttu-id="0da90-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="0da90-166">Version of the device configuration.</span></span> <span data-ttu-id="0da90-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0da90-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0da90-168">Netzwerkname</span><span class="sxs-lookup"><span data-stu-id="0da90-168">networkName</span></span>|<span data-ttu-id="0da90-169">String</span><span class="sxs-lookup"><span data-stu-id="0da90-169">String</span></span>|<span data-ttu-id="0da90-170">Netzwerkname</span><span class="sxs-lookup"><span data-stu-id="0da90-170">Network Name</span></span>|
|<span data-ttu-id="0da90-171">SSID</span><span class="sxs-lookup"><span data-stu-id="0da90-171">ssid</span></span>|<span data-ttu-id="0da90-172">String</span><span class="sxs-lookup"><span data-stu-id="0da90-172">String</span></span>|<span data-ttu-id="0da90-173">Dies ist der Name des Netzwerks Wi-Fi, die an alle Geräte gesendet wird.</span><span class="sxs-lookup"><span data-stu-id="0da90-173">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="0da90-174">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="0da90-174">connectAutomatically</span></span>|<span data-ttu-id="0da90-175">Boolesch</span><span class="sxs-lookup"><span data-stu-id="0da90-175">Boolean</span></span>|<span data-ttu-id="0da90-176">Verbinden Sie automatisch, wenn dieses Netzwerk im Bereich befindet.</span><span class="sxs-lookup"><span data-stu-id="0da90-176">Connect automatically when this network is in range.</span></span> <span data-ttu-id="0da90-177">Eine Einstellung auf "true" überspringt die Aufforderung der Benutzer und automatisch mit Wi-Fi-Netzwerk verbinden.</span><span class="sxs-lookup"><span data-stu-id="0da90-177">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="0da90-178">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="0da90-178">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="0da90-179">Boolesch</span><span class="sxs-lookup"><span data-stu-id="0da90-179">Boolean</span></span>|<span data-ttu-id="0da90-180">Bei Festlegung auf true festgelegt ist, dieses Profil erzwingt, dass das Gerät für die Verbindung mit einem Netzwerk SSID nicht, die an alle Geräte seine.</span><span class="sxs-lookup"><span data-stu-id="0da90-180">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="0da90-181">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="0da90-181">wiFiSecurityType</span></span>|[<span data-ttu-id="0da90-182">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="0da90-182">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="0da90-183">Gibt an, ob Wi-Fi-Endpunkt einen EAP-basierte Sicherheitstyp verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="0da90-183">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="0da90-184">Mögliche Werte sind: `open` und `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="0da90-184">Possible values are: `open`, `wpaEnterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="0da90-185">Antwort</span><span class="sxs-lookup"><span data-stu-id="0da90-185">Response</span></span>
<span data-ttu-id="0da90-186">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AndroidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="0da90-186">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0da90-187">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0da90-187">Example</span></span>
### <a name="request"></a><span data-ttu-id="0da90-188">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0da90-188">Request</span></span>
<span data-ttu-id="0da90-189">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0da90-189">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 436

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="0da90-190">Antwort</span><span class="sxs-lookup"><span data-stu-id="0da90-190">Response</span></span>
<span data-ttu-id="0da90-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0da90-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 618

{
  "@odata.type": "#microsoft.graph.androidWorkProfileWiFiConfiguration",
  "id": "8400d131-d131-8400-31d1-008431d10084",
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





