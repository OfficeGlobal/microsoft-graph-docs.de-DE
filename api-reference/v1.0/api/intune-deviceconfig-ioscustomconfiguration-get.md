---
title: iosCustomConfiguration abrufen
description: Lesen von Eigenschaften und Beziehungen des iosCustomConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2905797ccf1645537af15c90cc0c370981c3c251
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917097"
---
# <a name="get-ioscustomconfiguration"></a><span data-ttu-id="ea1b0-103">iosCustomConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="ea1b0-103">Get iosCustomConfiguration</span></span>

> <span data-ttu-id="ea1b0-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ea1b0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ea1b0-105">Lesen von Eigenschaften und Beziehungen des [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ea1b0-105">Read properties and relationships of the [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ea1b0-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ea1b0-106">Prerequisites</span></span>
<span data-ttu-id="ea1b0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea1b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea1b0-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ea1b0-109">Permission type</span></span>|<span data-ttu-id="ea1b0-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ea1b0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea1b0-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ea1b0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ea1b0-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ea1b0-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ea1b0-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ea1b0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea1b0-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ea1b0-114">Not supported.</span></span>|
|<span data-ttu-id="ea1b0-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ea1b0-115">Application</span></span>|<span data-ttu-id="ea1b0-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ea1b0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea1b0-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ea1b0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ea1b0-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ea1b0-118">Optional query parameters</span></span>
<span data-ttu-id="ea1b0-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ea1b0-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ea1b0-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ea1b0-120">Request headers</span></span>
|<span data-ttu-id="ea1b0-121">Header</span><span class="sxs-lookup"><span data-stu-id="ea1b0-121">Header</span></span>|<span data-ttu-id="ea1b0-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ea1b0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea1b0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea1b0-123">Authorization</span></span>|<span data-ttu-id="ea1b0-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ea1b0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea1b0-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ea1b0-125">Accept</span></span>|<span data-ttu-id="ea1b0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ea1b0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea1b0-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ea1b0-127">Request body</span></span>
<span data-ttu-id="ea1b0-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ea1b0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea1b0-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="ea1b0-129">Response</span></span>
<span data-ttu-id="ea1b0-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ea1b0-130">If successful, this method returns a `200 OK` response code and [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea1b0-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ea1b0-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="ea1b0-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ea1b0-132">Request</span></span>
<span data-ttu-id="ea1b0-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ea1b0-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="ea1b0-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="ea1b0-134">Response</span></span>
<span data-ttu-id="ea1b0-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ea1b0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 490

{
  "value": {
    "@odata.type": "#microsoft.graph.iosCustomConfiguration",
    "id": "f34428e3-28e3-f344-e328-44f3e32844f3",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "payloadName": "Payload Name value",
    "payloadFileName": "Payload File Name value",
    "payload": "cGF5bG9hZA=="
  }
}
```



