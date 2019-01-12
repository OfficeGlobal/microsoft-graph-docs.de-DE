---
title: Abrufen von „deviceManagementExchangeConnector“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs deviceManagementExchangeConnector.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a05b99257bb20de184815f662a4ace63bdb44e57
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960084"
---
# <a name="get-devicemanagementexchangeconnector"></a><span data-ttu-id="b3ab2-103">Abrufen von „deviceManagementExchangeConnector“</span><span class="sxs-lookup"><span data-stu-id="b3ab2-103">Get deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="b3ab2-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b3ab2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b3ab2-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="b3ab2-105">Read properties and relationships of the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b3ab2-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b3ab2-106">Prerequisites</span></span>
<span data-ttu-id="b3ab2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3ab2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3ab2-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b3ab2-109">Permission type</span></span>|<span data-ttu-id="b3ab2-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b3ab2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3ab2-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b3ab2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b3ab2-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b3ab2-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="b3ab2-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b3ab2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3ab2-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b3ab2-114">Not supported.</span></span>|
|<span data-ttu-id="b3ab2-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b3ab2-115">Application</span></span>|<span data-ttu-id="b3ab2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b3ab2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3ab2-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b3ab2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b3ab2-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b3ab2-118">Optional query parameters</span></span>
<span data-ttu-id="b3ab2-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b3ab2-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b3ab2-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b3ab2-120">Request headers</span></span>
|<span data-ttu-id="b3ab2-121">Header</span><span class="sxs-lookup"><span data-stu-id="b3ab2-121">Header</span></span>|<span data-ttu-id="b3ab2-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b3ab2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3ab2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3ab2-123">Authorization</span></span>|<span data-ttu-id="b3ab2-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b3ab2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3ab2-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b3ab2-125">Accept</span></span>|<span data-ttu-id="b3ab2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b3ab2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3ab2-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b3ab2-127">Request body</span></span>
<span data-ttu-id="b3ab2-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b3ab2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3ab2-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="b3ab2-129">Response</span></span>
<span data-ttu-id="b3ab2-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b3ab2-130">If successful, this method returns a `200 OK` response code and [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3ab2-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b3ab2-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="b3ab2-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b3ab2-132">Request</span></span>
<span data-ttu-id="b3ab2-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b3ab2-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
```

### <a name="response"></a><span data-ttu-id="b3ab2-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="b3ab2-134">Response</span></span>
<span data-ttu-id="b3ab2-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b3ab2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 580

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
    "id": "e11c1de8-1de8-e11c-e81d-1ce1e81d1ce1",
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
    "status": "connectionPending",
    "primarySmtpAddress": "Primary Smtp Address value",
    "serverName": "Server Name value",
    "connectorServerName": "Connector Server Name value",
    "exchangeConnectorType": "hosted",
    "version": "Version value",
    "exchangeAlias": "Exchange Alias value",
    "exchangeOrganization": "Exchange Organization value"
  }
}
```



