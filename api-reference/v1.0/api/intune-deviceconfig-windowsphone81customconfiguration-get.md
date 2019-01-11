---
title: windowsPhone81CustomConfiguration abrufen
description: Lesen von Eigenschaften und Beziehungen des windowsPhone81CustomConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 29bd3497b538f2239fc58590f8bc3d3ac01148d6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868238"
---
# <a name="get-windowsphone81customconfiguration"></a><span data-ttu-id="b9c68-103">windowsPhone81CustomConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="b9c68-103">Get windowsPhone81CustomConfiguration</span></span>

> <span data-ttu-id="b9c68-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b9c68-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b9c68-105">Lesen von Eigenschaften und Beziehungen des [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b9c68-105">Read properties and relationships of the [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b9c68-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b9c68-106">Prerequisites</span></span>
<span data-ttu-id="b9c68-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9c68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9c68-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b9c68-109">Permission type</span></span>|<span data-ttu-id="b9c68-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b9c68-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9c68-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b9c68-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b9c68-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9c68-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b9c68-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b9c68-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9c68-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b9c68-114">Not supported.</span></span>|
|<span data-ttu-id="b9c68-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b9c68-115">Application</span></span>|<span data-ttu-id="b9c68-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b9c68-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9c68-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b9c68-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b9c68-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b9c68-118">Optional query parameters</span></span>
<span data-ttu-id="b9c68-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b9c68-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b9c68-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b9c68-120">Request headers</span></span>
|<span data-ttu-id="b9c68-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b9c68-121">Header</span></span>|<span data-ttu-id="b9c68-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b9c68-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9c68-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9c68-123">Authorization</span></span>|<span data-ttu-id="b9c68-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b9c68-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9c68-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b9c68-125">Accept</span></span>|<span data-ttu-id="b9c68-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b9c68-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9c68-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b9c68-127">Request body</span></span>
<span data-ttu-id="b9c68-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b9c68-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9c68-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="b9c68-129">Response</span></span>
<span data-ttu-id="b9c68-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b9c68-130">If successful, this method returns a `200 OK` response code and [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9c68-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b9c68-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="b9c68-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b9c68-132">Request</span></span>
<span data-ttu-id="b9c68-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b9c68-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="b9c68-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="b9c68-134">Response</span></span>
<span data-ttu-id="b9c68-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b9c68-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 632

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
    "id": "0d98693c-693c-0d98-3c69-980d3c69980d",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "omaSettings": [
      {
        "@odata.type": "microsoft.graph.omaSettingInteger",
        "displayName": "Display Name value",
        "description": "Description value",
        "omaUri": "Oma Uri value",
        "value": 5
      }
    ]
  }
}
```



