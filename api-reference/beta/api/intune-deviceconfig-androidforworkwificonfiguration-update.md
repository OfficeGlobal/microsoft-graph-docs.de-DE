---
title: AndroidForWorkWiFiConfiguration aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AndroidForWorkWiFiConfiguration-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 50716b9e8dfc3a7e4952244afe87e28d310906c5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413129"
---
# <a name="update-androidforworkwificonfiguration"></a><span data-ttu-id="f821d-103">AndroidForWorkWiFiConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f821d-103">Update androidForWorkWiFiConfiguration</span></span>

> <span data-ttu-id="f821d-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="f821d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f821d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f821d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f821d-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f821d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f821d-107">Aktualisieren Sie die Eigenschaften eines [AndroidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f821d-107">Update the properties of a [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f821d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f821d-108">Prerequisites</span></span>
<span data-ttu-id="f821d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f821d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f821d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f821d-111">Permission type</span></span>|<span data-ttu-id="f821d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f821d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f821d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f821d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f821d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f821d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f821d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f821d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f821d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f821d-116">Not supported.</span></span>|
|<span data-ttu-id="f821d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f821d-117">Application</span></span>|<span data-ttu-id="f821d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f821d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f821d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f821d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f821d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f821d-120">Request headers</span></span>
|<span data-ttu-id="f821d-121">Header</span><span class="sxs-lookup"><span data-stu-id="f821d-121">Header</span></span>|<span data-ttu-id="f821d-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f821d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f821d-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="f821d-123">Authorization</span></span>|<span data-ttu-id="f821d-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f821d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f821d-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f821d-125">Accept</span></span>|<span data-ttu-id="f821d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f821d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f821d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f821d-127">Request body</span></span>
<span data-ttu-id="f821d-128">Geben Sie im Textkörper Anforderung für das Objekt [AndroidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="f821d-128">In the request body, supply a JSON representation for the [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object.</span></span>

<span data-ttu-id="f821d-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [AndroidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="f821d-129">The following table shows the properties that are required when you create the [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).</span></span>

|<span data-ttu-id="f821d-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f821d-130">Property</span></span>|<span data-ttu-id="f821d-131">Typ</span><span class="sxs-lookup"><span data-stu-id="f821d-131">Type</span></span>|<span data-ttu-id="f821d-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f821d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f821d-133">id</span><span class="sxs-lookup"><span data-stu-id="f821d-133">id</span></span>|<span data-ttu-id="f821d-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f821d-134">String</span></span>|<span data-ttu-id="f821d-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="f821d-135">Key of the entity.</span></span> <span data-ttu-id="f821d-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f821d-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f821d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f821d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f821d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f821d-138">DateTimeOffset</span></span>|<span data-ttu-id="f821d-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="f821d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f821d-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f821d-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f821d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f821d-141">roleScopeTagIds</span></span>|<span data-ttu-id="f821d-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="f821d-142">String collection</span></span>|<span data-ttu-id="f821d-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="f821d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f821d-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f821d-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f821d-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f821d-145">supportsScopeTags</span></span>|<span data-ttu-id="f821d-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="f821d-146">Boolean</span></span>|<span data-ttu-id="f821d-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f821d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f821d-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="f821d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f821d-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="f821d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f821d-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f821d-150">This property is read-only.</span></span> <span data-ttu-id="f821d-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f821d-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f821d-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f821d-152">createdDateTime</span></span>|<span data-ttu-id="f821d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f821d-153">DateTimeOffset</span></span>|<span data-ttu-id="f821d-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="f821d-154">DateTime the object was created.</span></span> <span data-ttu-id="f821d-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f821d-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f821d-156">description</span><span class="sxs-lookup"><span data-stu-id="f821d-156">description</span></span>|<span data-ttu-id="f821d-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f821d-157">String</span></span>|<span data-ttu-id="f821d-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="f821d-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f821d-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f821d-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f821d-160">displayName</span><span class="sxs-lookup"><span data-stu-id="f821d-160">displayName</span></span>|<span data-ttu-id="f821d-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f821d-161">String</span></span>|<span data-ttu-id="f821d-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="f821d-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f821d-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f821d-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f821d-164">Version</span><span class="sxs-lookup"><span data-stu-id="f821d-164">version</span></span>|<span data-ttu-id="f821d-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f821d-165">Int32</span></span>|<span data-ttu-id="f821d-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="f821d-166">Version of the device configuration.</span></span> <span data-ttu-id="f821d-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f821d-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f821d-168">Netzwerkname</span><span class="sxs-lookup"><span data-stu-id="f821d-168">networkName</span></span>|<span data-ttu-id="f821d-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f821d-169">String</span></span>|<span data-ttu-id="f821d-170">Netzwerkname</span><span class="sxs-lookup"><span data-stu-id="f821d-170">Network Name</span></span>|
|<span data-ttu-id="f821d-171">SSID</span><span class="sxs-lookup"><span data-stu-id="f821d-171">ssid</span></span>|<span data-ttu-id="f821d-172">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f821d-172">String</span></span>|<span data-ttu-id="f821d-173">Dies ist der Name des Netzwerks Wi-Fi, die an alle Geräte gesendet wird.</span><span class="sxs-lookup"><span data-stu-id="f821d-173">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="f821d-174">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="f821d-174">connectAutomatically</span></span>|<span data-ttu-id="f821d-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="f821d-175">Boolean</span></span>|<span data-ttu-id="f821d-176">Verbinden Sie automatisch, wenn dieses Netzwerk im Bereich befindet.</span><span class="sxs-lookup"><span data-stu-id="f821d-176">Connect automatically when this network is in range.</span></span> <span data-ttu-id="f821d-177">Eine Einstellung auf "true" überspringt die Aufforderung der Benutzer und automatisch mit Wi-Fi-Netzwerk verbinden.</span><span class="sxs-lookup"><span data-stu-id="f821d-177">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="f821d-178">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="f821d-178">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="f821d-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="f821d-179">Boolean</span></span>|<span data-ttu-id="f821d-180">Bei Festlegung auf true festgelegt ist, dieses Profil erzwingt, dass das Gerät für die Verbindung mit einem Netzwerk SSID nicht, die an alle Geräte seine.</span><span class="sxs-lookup"><span data-stu-id="f821d-180">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="f821d-181">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="f821d-181">wiFiSecurityType</span></span>|[<span data-ttu-id="f821d-182">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="f821d-182">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="f821d-183">Gibt an, ob Wi-Fi-Endpunkt einen EAP-basierte Sicherheitstyp verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="f821d-183">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="f821d-184">Mögliche Werte sind: `open` und `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="f821d-184">Possible values are: `open`, `wpaEnterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="f821d-185">Antwort</span><span class="sxs-lookup"><span data-stu-id="f821d-185">Response</span></span>
<span data-ttu-id="f821d-186">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AndroidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="f821d-186">If successful, this method returns a `200 OK` response code and an updated [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f821d-187">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f821d-187">Example</span></span>

### <a name="request"></a><span data-ttu-id="f821d-188">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f821d-188">Request</span></span>
<span data-ttu-id="f821d-189">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f821d-189">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 442

{
  "@odata.type": "#microsoft.graph.androidForWorkWiFiConfiguration",
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

### <a name="response"></a><span data-ttu-id="f821d-190">Antwort</span><span class="sxs-lookup"><span data-stu-id="f821d-190">Response</span></span>
<span data-ttu-id="f821d-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f821d-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 614

{
  "@odata.type": "#microsoft.graph.androidForWorkWiFiConfiguration",
  "id": "58bcfe05-fe05-58bc-05fe-bc5805febc58",
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




