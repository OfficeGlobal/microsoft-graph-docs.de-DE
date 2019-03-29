---
title: Windows10NetworkBoundaryConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines windows10NetworkBoundaryConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6b75190498e5aa82e1ef77dbd815a05d03017a56
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30958704"
---
# <a name="update-windows10networkboundaryconfiguration"></a><span data-ttu-id="91ed6-103">Windows10NetworkBoundaryConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="91ed6-103">Update windows10NetworkBoundaryConfiguration</span></span>

> <span data-ttu-id="91ed6-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="91ed6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91ed6-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="91ed6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91ed6-106">Aktualisieren der Eigenschaften eines [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="91ed6-106">Update the properties of a [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="91ed6-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="91ed6-107">Prerequisites</span></span>
<span data-ttu-id="91ed6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91ed6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91ed6-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="91ed6-110">Permission type</span></span>|<span data-ttu-id="91ed6-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="91ed6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91ed6-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="91ed6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="91ed6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91ed6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="91ed6-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="91ed6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91ed6-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="91ed6-115">Not supported.</span></span>|
|<span data-ttu-id="91ed6-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="91ed6-116">Application</span></span>|<span data-ttu-id="91ed6-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="91ed6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="91ed6-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="91ed6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="91ed6-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="91ed6-119">Request headers</span></span>
|<span data-ttu-id="91ed6-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="91ed6-120">Header</span></span>|<span data-ttu-id="91ed6-121">Wert</span><span class="sxs-lookup"><span data-stu-id="91ed6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91ed6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="91ed6-122">Authorization</span></span>|<span data-ttu-id="91ed6-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="91ed6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91ed6-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="91ed6-124">Accept</span></span>|<span data-ttu-id="91ed6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="91ed6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91ed6-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="91ed6-126">Request body</span></span>
<span data-ttu-id="91ed6-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="91ed6-127">In the request body, supply a JSON representation for the [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object.</span></span>

<span data-ttu-id="91ed6-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="91ed6-128">The following table shows the properties that are required when you create the [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md).</span></span>

|<span data-ttu-id="91ed6-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="91ed6-129">Property</span></span>|<span data-ttu-id="91ed6-130">Typ</span><span class="sxs-lookup"><span data-stu-id="91ed6-130">Type</span></span>|<span data-ttu-id="91ed6-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="91ed6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91ed6-132">id</span><span class="sxs-lookup"><span data-stu-id="91ed6-132">id</span></span>|<span data-ttu-id="91ed6-133">String</span><span class="sxs-lookup"><span data-stu-id="91ed6-133">String</span></span>|<span data-ttu-id="91ed6-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="91ed6-134">Key of the entity.</span></span> <span data-ttu-id="91ed6-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="91ed6-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91ed6-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="91ed6-136">lastModifiedDateTime</span></span>|<span data-ttu-id="91ed6-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91ed6-137">DateTimeOffset</span></span>|<span data-ttu-id="91ed6-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="91ed6-138">DateTime the object was last modified.</span></span> <span data-ttu-id="91ed6-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="91ed6-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91ed6-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="91ed6-140">roleScopeTagIds</span></span>|<span data-ttu-id="91ed6-141">String collection</span><span class="sxs-lookup"><span data-stu-id="91ed6-141">String collection</span></span>|<span data-ttu-id="91ed6-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="91ed6-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="91ed6-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="91ed6-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91ed6-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="91ed6-144">supportsScopeTags</span></span>|<span data-ttu-id="91ed6-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="91ed6-145">Boolean</span></span>|<span data-ttu-id="91ed6-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="91ed6-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="91ed6-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="91ed6-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="91ed6-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="91ed6-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="91ed6-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="91ed6-149">This property is read-only.</span></span> <span data-ttu-id="91ed6-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="91ed6-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91ed6-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="91ed6-151">createdDateTime</span></span>|<span data-ttu-id="91ed6-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91ed6-152">DateTimeOffset</span></span>|<span data-ttu-id="91ed6-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="91ed6-153">DateTime the object was created.</span></span> <span data-ttu-id="91ed6-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="91ed6-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91ed6-155">description</span><span class="sxs-lookup"><span data-stu-id="91ed6-155">description</span></span>|<span data-ttu-id="91ed6-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="91ed6-156">String</span></span>|<span data-ttu-id="91ed6-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="91ed6-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="91ed6-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="91ed6-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91ed6-159">displayName</span><span class="sxs-lookup"><span data-stu-id="91ed6-159">displayName</span></span>|<span data-ttu-id="91ed6-160">String</span><span class="sxs-lookup"><span data-stu-id="91ed6-160">String</span></span>|<span data-ttu-id="91ed6-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="91ed6-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="91ed6-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="91ed6-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91ed6-163">Version</span><span class="sxs-lookup"><span data-stu-id="91ed6-163">version</span></span>|<span data-ttu-id="91ed6-164">Int32</span><span class="sxs-lookup"><span data-stu-id="91ed6-164">Int32</span></span>|<span data-ttu-id="91ed6-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="91ed6-165">Version of the device configuration.</span></span> <span data-ttu-id="91ed6-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="91ed6-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91ed6-167">windowsNetworkIsolationPolicy</span><span class="sxs-lookup"><span data-stu-id="91ed6-167">windowsNetworkIsolationPolicy</span></span>|[<span data-ttu-id="91ed6-168">windowsNetworkIsolationPolicy</span><span class="sxs-lookup"><span data-stu-id="91ed6-168">windowsNetworkIsolationPolicy</span></span>](../resources/intune-deviceconfig-windowsnetworkisolationpolicy.md)|<span data-ttu-id="91ed6-169">Windows-Netzwerk Isolations Richtlinie</span><span class="sxs-lookup"><span data-stu-id="91ed6-169">Windows Network Isolation Policy</span></span>|



## <a name="response"></a><span data-ttu-id="91ed6-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="91ed6-170">Response</span></span>
<span data-ttu-id="91ed6-171">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="91ed6-171">If successful, this method returns a `200 OK` response code and an updated [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91ed6-172">Beispiel</span><span class="sxs-lookup"><span data-stu-id="91ed6-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="91ed6-173">Anforderung</span><span class="sxs-lookup"><span data-stu-id="91ed6-173">Request</span></span>
<span data-ttu-id="91ed6-174">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="91ed6-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1244

{
  "@odata.type": "#microsoft.graph.windows10NetworkBoundaryConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "windowsNetworkIsolationPolicy": {
    "@odata.type": "microsoft.graph.windowsNetworkIsolationPolicy",
    "enterpriseNetworkDomainNames": [
      "Enterprise Network Domain Names value"
    ],
    "enterpriseCloudResources": [
      {
        "@odata.type": "microsoft.graph.proxiedDomain",
        "ipAddressOrFQDN": "Ip Address Or FQDN value",
        "proxy": "Proxy value"
      }
    ],
    "enterpriseIPRanges": [
      {
        "@odata.type": "microsoft.graph.iPv6Range",
        "lowerAddress": "Lower Address value",
        "upperAddress": "Upper Address value"
      }
    ],
    "enterpriseInternalProxyServers": [
      "Enterprise Internal Proxy Servers value"
    ],
    "enterpriseIPRangesAreAuthoritative": true,
    "enterpriseProxyServers": [
      "Enterprise Proxy Servers value"
    ],
    "enterpriseProxyServersAreAuthoritative": true,
    "neutralDomainResources": [
      "Neutral Domain Resources value"
    ]
  }
}
```

### <a name="response"></a><span data-ttu-id="91ed6-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="91ed6-175">Response</span></span>
<span data-ttu-id="91ed6-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="91ed6-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1416

{
  "@odata.type": "#microsoft.graph.windows10NetworkBoundaryConfiguration",
  "id": "afbc9e01-9e01-afbc-019e-bcaf019ebcaf",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "windowsNetworkIsolationPolicy": {
    "@odata.type": "microsoft.graph.windowsNetworkIsolationPolicy",
    "enterpriseNetworkDomainNames": [
      "Enterprise Network Domain Names value"
    ],
    "enterpriseCloudResources": [
      {
        "@odata.type": "microsoft.graph.proxiedDomain",
        "ipAddressOrFQDN": "Ip Address Or FQDN value",
        "proxy": "Proxy value"
      }
    ],
    "enterpriseIPRanges": [
      {
        "@odata.type": "microsoft.graph.iPv6Range",
        "lowerAddress": "Lower Address value",
        "upperAddress": "Upper Address value"
      }
    ],
    "enterpriseInternalProxyServers": [
      "Enterprise Internal Proxy Servers value"
    ],
    "enterpriseIPRangesAreAuthoritative": true,
    "enterpriseProxyServers": [
      "Enterprise Proxy Servers value"
    ],
    "enterpriseProxyServersAreAuthoritative": true,
    "neutralDomainResources": [
      "Neutral Domain Resources value"
    ]
  }
}
```




