---
title: Liste windows81VpnConfigurations
description: Listeneigenschaften und Beziehungen der windows81VpnConfiguration-Objekte.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1082e803324c1064d3caab8ffdada8d0a330e860
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886555"
---
# <a name="list-windows81vpnconfigurations"></a><span data-ttu-id="ff97d-103">Liste windows81VpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="ff97d-103">List windows81VpnConfigurations</span></span>

> <span data-ttu-id="ff97d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ff97d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff97d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ff97d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ff97d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ff97d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ff97d-107">Listeneigenschaften und Beziehungen der [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="ff97d-107">List properties and relationships of the [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ff97d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ff97d-108">Prerequisites</span></span>
<span data-ttu-id="ff97d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff97d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff97d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ff97d-111">Permission type</span></span>|<span data-ttu-id="ff97d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ff97d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff97d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ff97d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ff97d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ff97d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ff97d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ff97d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff97d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ff97d-116">Not supported.</span></span>|
|<span data-ttu-id="ff97d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ff97d-117">Application</span></span>|<span data-ttu-id="ff97d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ff97d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff97d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ff97d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ff97d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ff97d-120">Request headers</span></span>
|<span data-ttu-id="ff97d-121">Header</span><span class="sxs-lookup"><span data-stu-id="ff97d-121">Header</span></span>|<span data-ttu-id="ff97d-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ff97d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff97d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff97d-123">Authorization</span></span>|<span data-ttu-id="ff97d-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ff97d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff97d-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ff97d-125">Accept</span></span>|<span data-ttu-id="ff97d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ff97d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff97d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ff97d-127">Request body</span></span>
<span data-ttu-id="ff97d-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ff97d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff97d-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="ff97d-129">Response</span></span>
<span data-ttu-id="ff97d-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ff97d-130">If successful, this method returns a `200 OK` response code and a collection of [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff97d-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ff97d-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="ff97d-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ff97d-132">Request</span></span>
<span data-ttu-id="ff97d-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ff97d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="ff97d-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="ff97d-134">Response</span></span>
<span data-ttu-id="ff97d-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ff97d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1352

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows81VpnConfiguration",
      "id": "6aa07da3-7da3-6aa0-a37d-a06aa37da06a",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "connectionName": "Connection Name value",
      "servers": [
        {
          "@odata.type": "microsoft.graph.vpnServer",
          "description": "Description value",
          "address": "Address value",
          "isDefaultServer": true
        }
      ],
      "customXml": "Y3VzdG9tWG1s",
      "applyOnlyToWindows81": true,
      "connectionType": "f5EdgeClient",
      "loginGroupOrDomain": "Login Group Or Domain value",
      "enableSplitTunneling": true,
      "proxyServer": {
        "@odata.type": "microsoft.graph.windows81VpnProxyServer",
        "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
        "address": "Address value",
        "port": 4,
        "automaticallyDetectProxySettings": true,
        "bypassProxyServerForLocalAddress": true
      }
    }
  ]
}
```





