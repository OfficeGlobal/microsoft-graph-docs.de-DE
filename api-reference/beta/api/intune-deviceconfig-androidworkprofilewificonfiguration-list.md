---
title: Liste androidWorkProfileWiFiConfigurations
description: Listeneigenschaften und Beziehungen der AndroidWorkProfileWiFiConfiguration-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 843828309dda03236b4d5ab516928ae1af9d4853
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27973797"
---
# <a name="list-androidworkprofilewificonfigurations"></a><span data-ttu-id="2181a-103">Liste androidWorkProfileWiFiConfigurations</span><span class="sxs-lookup"><span data-stu-id="2181a-103">List androidWorkProfileWiFiConfigurations</span></span>

> <span data-ttu-id="2181a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2181a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2181a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2181a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2181a-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2181a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2181a-107">Listeneigenschaften und Beziehungen der [AndroidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="2181a-107">List properties and relationships of the [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2181a-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2181a-108">Prerequisites</span></span>
<span data-ttu-id="2181a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2181a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2181a-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2181a-111">Permission type</span></span>|<span data-ttu-id="2181a-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2181a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2181a-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2181a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2181a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2181a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2181a-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2181a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2181a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2181a-116">Not supported.</span></span>|
|<span data-ttu-id="2181a-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2181a-117">Application</span></span>|<span data-ttu-id="2181a-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2181a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2181a-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2181a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2181a-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2181a-120">Request headers</span></span>
|<span data-ttu-id="2181a-121">Header</span><span class="sxs-lookup"><span data-stu-id="2181a-121">Header</span></span>|<span data-ttu-id="2181a-122">Wert</span><span class="sxs-lookup"><span data-stu-id="2181a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2181a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2181a-123">Authorization</span></span>|<span data-ttu-id="2181a-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2181a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2181a-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2181a-125">Accept</span></span>|<span data-ttu-id="2181a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2181a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2181a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2181a-127">Request body</span></span>
<span data-ttu-id="2181a-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2181a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2181a-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="2181a-129">Response</span></span>
<span data-ttu-id="2181a-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [AndroidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2181a-130">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2181a-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2181a-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="2181a-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2181a-132">Request</span></span>
<span data-ttu-id="2181a-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2181a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="2181a-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="2181a-134">Response</span></span>
<span data-ttu-id="2181a-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2181a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 715

{
  "value": [
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
  ]
}
```





