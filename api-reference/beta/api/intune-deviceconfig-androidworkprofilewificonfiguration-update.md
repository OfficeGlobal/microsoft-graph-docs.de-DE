---
title: AndroidWorkProfileWiFiConfiguration aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AndroidWorkProfileWiFiConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 229ace77c5e921c77a988608d7c2dacce5fc1bf4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983051"
---
# <a name="update-androidworkprofilewificonfiguration"></a><span data-ttu-id="237c5-103">AndroidWorkProfileWiFiConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="237c5-103">Update androidWorkProfileWiFiConfiguration</span></span>

> <span data-ttu-id="237c5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="237c5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="237c5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="237c5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="237c5-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="237c5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="237c5-107">Aktualisieren Sie die Eigenschaften eines [AndroidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="237c5-107">Update the properties of a [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="237c5-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="237c5-108">Prerequisites</span></span>
<span data-ttu-id="237c5-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="237c5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="237c5-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="237c5-111">Permission type</span></span>|<span data-ttu-id="237c5-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="237c5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="237c5-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="237c5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="237c5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="237c5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="237c5-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="237c5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="237c5-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="237c5-116">Not supported.</span></span>|
|<span data-ttu-id="237c5-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="237c5-117">Application</span></span>|<span data-ttu-id="237c5-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="237c5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="237c5-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="237c5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="237c5-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="237c5-120">Request headers</span></span>
|<span data-ttu-id="237c5-121">Header</span><span class="sxs-lookup"><span data-stu-id="237c5-121">Header</span></span>|<span data-ttu-id="237c5-122">Wert</span><span class="sxs-lookup"><span data-stu-id="237c5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="237c5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="237c5-123">Authorization</span></span>|<span data-ttu-id="237c5-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="237c5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="237c5-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="237c5-125">Accept</span></span>|<span data-ttu-id="237c5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="237c5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="237c5-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="237c5-127">Request body</span></span>
<span data-ttu-id="237c5-128">Geben Sie im Textkörper Anforderung für das Objekt [AndroidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="237c5-128">In the request body, supply a JSON representation for the [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) object.</span></span>

<span data-ttu-id="237c5-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [AndroidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="237c5-129">The following table shows the properties that are required when you create the [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md).</span></span>

|<span data-ttu-id="237c5-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="237c5-130">Property</span></span>|<span data-ttu-id="237c5-131">Typ</span><span class="sxs-lookup"><span data-stu-id="237c5-131">Type</span></span>|<span data-ttu-id="237c5-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="237c5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="237c5-133">id</span><span class="sxs-lookup"><span data-stu-id="237c5-133">id</span></span>|<span data-ttu-id="237c5-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="237c5-134">String</span></span>|<span data-ttu-id="237c5-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="237c5-135">Key of the entity.</span></span> <span data-ttu-id="237c5-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="237c5-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="237c5-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="237c5-137">lastModifiedDateTime</span></span>|<span data-ttu-id="237c5-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="237c5-138">DateTimeOffset</span></span>|<span data-ttu-id="237c5-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="237c5-139">DateTime the object was last modified.</span></span> <span data-ttu-id="237c5-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="237c5-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="237c5-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="237c5-141">roleScopeTagIds</span></span>|<span data-ttu-id="237c5-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="237c5-142">String collection</span></span>|<span data-ttu-id="237c5-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="237c5-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="237c5-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="237c5-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="237c5-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="237c5-145">supportsScopeTags</span></span>|<span data-ttu-id="237c5-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="237c5-146">Boolean</span></span>|<span data-ttu-id="237c5-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="237c5-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="237c5-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="237c5-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="237c5-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="237c5-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="237c5-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="237c5-150">This property is read-only.</span></span> <span data-ttu-id="237c5-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="237c5-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="237c5-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="237c5-152">createdDateTime</span></span>|<span data-ttu-id="237c5-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="237c5-153">DateTimeOffset</span></span>|<span data-ttu-id="237c5-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="237c5-154">DateTime the object was created.</span></span> <span data-ttu-id="237c5-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="237c5-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="237c5-156">description</span><span class="sxs-lookup"><span data-stu-id="237c5-156">description</span></span>|<span data-ttu-id="237c5-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="237c5-157">String</span></span>|<span data-ttu-id="237c5-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="237c5-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="237c5-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="237c5-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="237c5-160">displayName</span><span class="sxs-lookup"><span data-stu-id="237c5-160">displayName</span></span>|<span data-ttu-id="237c5-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="237c5-161">String</span></span>|<span data-ttu-id="237c5-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="237c5-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="237c5-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="237c5-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="237c5-164">Version</span><span class="sxs-lookup"><span data-stu-id="237c5-164">version</span></span>|<span data-ttu-id="237c5-165">Int32</span><span class="sxs-lookup"><span data-stu-id="237c5-165">Int32</span></span>|<span data-ttu-id="237c5-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="237c5-166">Version of the device configuration.</span></span> <span data-ttu-id="237c5-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="237c5-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="237c5-168">Netzwerkname</span><span class="sxs-lookup"><span data-stu-id="237c5-168">networkName</span></span>|<span data-ttu-id="237c5-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="237c5-169">String</span></span>|<span data-ttu-id="237c5-170">Netzwerkname</span><span class="sxs-lookup"><span data-stu-id="237c5-170">Network Name</span></span>|
|<span data-ttu-id="237c5-171">SSID</span><span class="sxs-lookup"><span data-stu-id="237c5-171">ssid</span></span>|<span data-ttu-id="237c5-172">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="237c5-172">String</span></span>|<span data-ttu-id="237c5-173">Dies ist der Name des Netzwerks Wi-Fi, die an alle Geräte gesendet wird.</span><span class="sxs-lookup"><span data-stu-id="237c5-173">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="237c5-174">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="237c5-174">connectAutomatically</span></span>|<span data-ttu-id="237c5-175">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="237c5-175">Boolean</span></span>|<span data-ttu-id="237c5-176">Verbinden Sie automatisch, wenn dieses Netzwerk im Bereich befindet.</span><span class="sxs-lookup"><span data-stu-id="237c5-176">Connect automatically when this network is in range.</span></span> <span data-ttu-id="237c5-177">Eine Einstellung auf "true" überspringt die Aufforderung der Benutzer und automatisch mit Wi-Fi-Netzwerk verbinden.</span><span class="sxs-lookup"><span data-stu-id="237c5-177">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="237c5-178">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="237c5-178">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="237c5-179">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="237c5-179">Boolean</span></span>|<span data-ttu-id="237c5-180">Bei Festlegung auf true festgelegt ist, dieses Profil erzwingt, dass das Gerät für die Verbindung mit einem Netzwerk SSID nicht, die an alle Geräte seine.</span><span class="sxs-lookup"><span data-stu-id="237c5-180">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="237c5-181">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="237c5-181">wiFiSecurityType</span></span>|[<span data-ttu-id="237c5-182">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="237c5-182">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="237c5-183">Gibt an, ob Wi-Fi-Endpunkt einen EAP-basierte Sicherheitstyp verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="237c5-183">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="237c5-184">Mögliche Werte sind: `open` und `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="237c5-184">Possible values are: `open`, `wpaEnterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="237c5-185">Antwort</span><span class="sxs-lookup"><span data-stu-id="237c5-185">Response</span></span>
<span data-ttu-id="237c5-186">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AndroidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="237c5-186">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="237c5-187">Beispiel</span><span class="sxs-lookup"><span data-stu-id="237c5-187">Example</span></span>
### <a name="request"></a><span data-ttu-id="237c5-188">Anforderung</span><span class="sxs-lookup"><span data-stu-id="237c5-188">Request</span></span>
<span data-ttu-id="237c5-189">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="237c5-189">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="237c5-190">Antwort</span><span class="sxs-lookup"><span data-stu-id="237c5-190">Response</span></span>
<span data-ttu-id="237c5-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="237c5-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





