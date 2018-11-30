---
title: deviceManagementExchangeConnectors auflisten
description: Auflisten von Eigenschaften und Beziehungen der deviceManagementExchangeConnector-Objekte.
ms.openlocfilehash: bece85c7bd68adaf0cf3f514c24dc603ac0e33e1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019163"
---
# <a name="list-devicemanagementexchangeconnectors"></a><span data-ttu-id="f77ec-103">deviceManagementExchangeConnectors auflisten</span><span class="sxs-lookup"><span data-stu-id="f77ec-103">List deviceManagementExchangeConnectors</span></span>

> <span data-ttu-id="f77ec-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f77ec-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f77ec-105">Auflisten von Eigenschaften und Beziehungen der [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="f77ec-105">List properties and relationships of the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f77ec-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f77ec-106">Prerequisites</span></span>
<span data-ttu-id="f77ec-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f77ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f77ec-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f77ec-109">Permission type</span></span>|<span data-ttu-id="f77ec-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f77ec-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f77ec-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f77ec-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f77ec-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f77ec-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="f77ec-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f77ec-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f77ec-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f77ec-114">Not supported.</span></span>|
|<span data-ttu-id="f77ec-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f77ec-115">Application</span></span>|<span data-ttu-id="f77ec-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f77ec-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f77ec-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f77ec-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="f77ec-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f77ec-118">Request headers</span></span>
|<span data-ttu-id="f77ec-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f77ec-119">Header</span></span>|<span data-ttu-id="f77ec-120">Wert</span><span class="sxs-lookup"><span data-stu-id="f77ec-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f77ec-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f77ec-121">Authorization</span></span>|<span data-ttu-id="f77ec-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f77ec-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f77ec-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f77ec-123">Accept</span></span>|<span data-ttu-id="f77ec-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f77ec-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f77ec-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f77ec-125">Request body</span></span>
<span data-ttu-id="f77ec-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f77ec-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f77ec-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="f77ec-127">Response</span></span>
<span data-ttu-id="f77ec-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Sammlung von Objekten des Typs [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f77ec-128">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f77ec-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f77ec-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="f77ec-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f77ec-130">Request</span></span>
<span data-ttu-id="f77ec-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f77ec-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors
```

### <a name="response"></a><span data-ttu-id="f77ec-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="f77ec-132">Response</span></span>
<span data-ttu-id="f77ec-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f77ec-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 616

{
  "value": [
    {
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
  ]
}
```


