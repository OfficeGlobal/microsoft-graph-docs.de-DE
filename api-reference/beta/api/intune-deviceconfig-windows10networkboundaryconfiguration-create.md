---
title: Erstellen von windows10NetworkBoundaryConfiguration
description: Erstellen eines neuen windows10NetworkBoundaryConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b0d0926cda80a18cbf12e4ea5d1cb93669606775
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925994"
---
# <a name="create-windows10networkboundaryconfiguration"></a><span data-ttu-id="80735-103">Erstellen von windows10NetworkBoundaryConfiguration</span><span class="sxs-lookup"><span data-stu-id="80735-103">Create windows10NetworkBoundaryConfiguration</span></span>

> <span data-ttu-id="80735-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="80735-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="80735-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="80735-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="80735-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="80735-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="80735-107">Erstellen eines neuen [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="80735-107">Create a new [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="80735-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="80735-108">Prerequisites</span></span>
<span data-ttu-id="80735-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80735-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80735-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="80735-111">Permission type</span></span>|<span data-ttu-id="80735-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="80735-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80735-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="80735-113">Delegated (work or school account)</span></span>|<span data-ttu-id="80735-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80735-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="80735-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="80735-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80735-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="80735-116">Not supported.</span></span>|
|<span data-ttu-id="80735-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="80735-117">Application</span></span>|<span data-ttu-id="80735-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="80735-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="80735-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="80735-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="80735-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="80735-120">Request headers</span></span>
|<span data-ttu-id="80735-121">Header</span><span class="sxs-lookup"><span data-stu-id="80735-121">Header</span></span>|<span data-ttu-id="80735-122">Wert</span><span class="sxs-lookup"><span data-stu-id="80735-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80735-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="80735-123">Authorization</span></span>|<span data-ttu-id="80735-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="80735-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80735-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="80735-125">Accept</span></span>|<span data-ttu-id="80735-126">application/json</span><span class="sxs-lookup"><span data-stu-id="80735-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80735-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="80735-127">Request body</span></span>
<span data-ttu-id="80735-128">Geben Sie im Textkörper Anforderung für das Objekt windows10NetworkBoundaryConfiguration eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="80735-128">In the request body, supply a JSON representation for the windows10NetworkBoundaryConfiguration object.</span></span>

<span data-ttu-id="80735-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die windows10NetworkBoundaryConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="80735-129">The following table shows the properties that are required when you create the windows10NetworkBoundaryConfiguration.</span></span>

|<span data-ttu-id="80735-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="80735-130">Property</span></span>|<span data-ttu-id="80735-131">Typ</span><span class="sxs-lookup"><span data-stu-id="80735-131">Type</span></span>|<span data-ttu-id="80735-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="80735-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80735-133">id</span><span class="sxs-lookup"><span data-stu-id="80735-133">id</span></span>|<span data-ttu-id="80735-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80735-134">String</span></span>|<span data-ttu-id="80735-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="80735-135">Key of the entity.</span></span> <span data-ttu-id="80735-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80735-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80735-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="80735-137">lastModifiedDateTime</span></span>|<span data-ttu-id="80735-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80735-138">DateTimeOffset</span></span>|<span data-ttu-id="80735-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="80735-139">DateTime the object was last modified.</span></span> <span data-ttu-id="80735-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80735-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80735-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="80735-141">roleScopeTagIds</span></span>|<span data-ttu-id="80735-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="80735-142">String collection</span></span>|<span data-ttu-id="80735-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="80735-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="80735-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80735-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80735-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="80735-145">supportsScopeTags</span></span>|<span data-ttu-id="80735-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="80735-146">Boolean</span></span>|<span data-ttu-id="80735-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="80735-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="80735-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="80735-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="80735-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="80735-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="80735-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="80735-150">This property is read-only.</span></span> <span data-ttu-id="80735-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80735-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80735-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="80735-152">createdDateTime</span></span>|<span data-ttu-id="80735-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80735-153">DateTimeOffset</span></span>|<span data-ttu-id="80735-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="80735-154">DateTime the object was created.</span></span> <span data-ttu-id="80735-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80735-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80735-156">description</span><span class="sxs-lookup"><span data-stu-id="80735-156">description</span></span>|<span data-ttu-id="80735-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80735-157">String</span></span>|<span data-ttu-id="80735-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="80735-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="80735-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80735-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80735-160">displayName</span><span class="sxs-lookup"><span data-stu-id="80735-160">displayName</span></span>|<span data-ttu-id="80735-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80735-161">String</span></span>|<span data-ttu-id="80735-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="80735-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="80735-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80735-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80735-164">Version</span><span class="sxs-lookup"><span data-stu-id="80735-164">version</span></span>|<span data-ttu-id="80735-165">Int32</span><span class="sxs-lookup"><span data-stu-id="80735-165">Int32</span></span>|<span data-ttu-id="80735-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="80735-166">Version of the device configuration.</span></span> <span data-ttu-id="80735-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80735-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80735-168">windowsNetworkIsolationPolicy</span><span class="sxs-lookup"><span data-stu-id="80735-168">windowsNetworkIsolationPolicy</span></span>|[<span data-ttu-id="80735-169">windowsNetworkIsolationPolicy</span><span class="sxs-lookup"><span data-stu-id="80735-169">windowsNetworkIsolationPolicy</span></span>](../resources/intune-deviceconfig-windowsnetworkisolationpolicy.md)|<span data-ttu-id="80735-170">Windows-Isolation Netzwerkrichtlinien</span><span class="sxs-lookup"><span data-stu-id="80735-170">Windows Network Isolation Policy</span></span>|



## <a name="response"></a><span data-ttu-id="80735-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="80735-171">Response</span></span>
<span data-ttu-id="80735-172">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="80735-172">If successful, this method returns a `201 Created` response code and a [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80735-173">Beispiel</span><span class="sxs-lookup"><span data-stu-id="80735-173">Example</span></span>
### <a name="request"></a><span data-ttu-id="80735-174">Anforderung</span><span class="sxs-lookup"><span data-stu-id="80735-174">Request</span></span>
<span data-ttu-id="80735-175">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="80735-175">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1308

{
  "@odata.type": "#microsoft.graph.windows10NetworkBoundaryConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="80735-176">Antwort</span><span class="sxs-lookup"><span data-stu-id="80735-176">Response</span></span>
<span data-ttu-id="80735-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="80735-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





