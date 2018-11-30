---
title: mobileThreatDefenseConnectors auflisten
description: Listet die Eigenschaften und Beziehungen von Objekten des Typs mobileThreatDefenseConnector auf.
ms.openlocfilehash: 12bec14500ab482730cc1c3247a571f4f93a292e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019572"
---
# <a name="list-mobilethreatdefenseconnectors"></a><span data-ttu-id="2759e-103">mobileThreatDefenseConnectors auflisten</span><span class="sxs-lookup"><span data-stu-id="2759e-103">List mobileThreatDefenseConnectors</span></span>

> <span data-ttu-id="2759e-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2759e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2759e-105">Listet die Eigenschaften und Beziehungen von Objekten des Typs [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) auf.</span><span class="sxs-lookup"><span data-stu-id="2759e-105">List properties and relationships of the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2759e-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2759e-106">Prerequisites</span></span>
<span data-ttu-id="2759e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2759e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2759e-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2759e-109">Permission type</span></span>|<span data-ttu-id="2759e-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2759e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2759e-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2759e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2759e-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2759e-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="2759e-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2759e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2759e-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2759e-114">Not supported.</span></span>|
|<span data-ttu-id="2759e-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2759e-115">Application</span></span>|<span data-ttu-id="2759e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2759e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2759e-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2759e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="2759e-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2759e-118">Request headers</span></span>
|<span data-ttu-id="2759e-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2759e-119">Header</span></span>|<span data-ttu-id="2759e-120">Wert</span><span class="sxs-lookup"><span data-stu-id="2759e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2759e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2759e-121">Authorization</span></span>|<span data-ttu-id="2759e-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2759e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2759e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="2759e-123">Accept</span></span>|<span data-ttu-id="2759e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2759e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2759e-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2759e-125">Request body</span></span>
<span data-ttu-id="2759e-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2759e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2759e-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="2759e-127">Response</span></span>
<span data-ttu-id="2759e-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2759e-128">If successful, this method returns a `200 OK` response code and a collection of [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2759e-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2759e-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="2759e-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2759e-130">Request</span></span>
<span data-ttu-id="2759e-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2759e-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/mobileThreatDefenseConnectors
```

### <a name="response"></a><span data-ttu-id="2759e-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="2759e-132">Response</span></span>
<span data-ttu-id="2759e-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2759e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 536

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
      "id": "e4bede14-de14-e4be-14de-bee414debee4",
      "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
      "partnerState": "available",
      "androidEnabled": true,
      "iosEnabled": true,
      "androidDeviceBlockedOnMissingPartnerData": true,
      "iosDeviceBlockedOnMissingPartnerData": true,
      "partnerUnsupportedOsVersionBlocked": true,
      "partnerUnresponsivenessThresholdInDays": 6
    }
  ]
}
```



