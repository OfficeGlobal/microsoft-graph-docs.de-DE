---
title: mobileThreatDefenseConnector abrufen
description: Liest die Eigenschaften und Beziehungen von Objekten des Typs mobileThreatDefenseConnector.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d3329c7f48e94773658649caf939b4e90c816cd2
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259066"
---
# <a name="get-mobilethreatdefenseconnector"></a><span data-ttu-id="0f4b0-103">mobileThreatDefenseConnector abrufen</span><span class="sxs-lookup"><span data-stu-id="0f4b0-103">Get mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="0f4b0-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="0f4b0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f4b0-105">Liest die Eigenschaften und Beziehungen von Objekten des Typs [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="0f4b0-105">Read properties and relationships of the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f4b0-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0f4b0-106">Prerequisites</span></span>
<span data-ttu-id="0f4b0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0f4b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0f4b0-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0f4b0-109">Permission type</span></span>|<span data-ttu-id="0f4b0-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0f4b0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f4b0-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0f4b0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0f4b0-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="0f4b0-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="0f4b0-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0f4b0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f4b0-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0f4b0-114">Not supported.</span></span>|
|<span data-ttu-id="0f4b0-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0f4b0-115">Application</span></span>|<span data-ttu-id="0f4b0-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0f4b0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f4b0-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0f4b0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0f4b0-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="0f4b0-118">Optional query parameters</span></span>
<span data-ttu-id="0f4b0-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0f4b0-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0f4b0-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0f4b0-120">Request headers</span></span>
|<span data-ttu-id="0f4b0-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0f4b0-121">Header</span></span>|<span data-ttu-id="0f4b0-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0f4b0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f4b0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f4b0-123">Authorization</span></span>|<span data-ttu-id="0f4b0-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0f4b0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f4b0-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0f4b0-125">Accept</span></span>|<span data-ttu-id="0f4b0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0f4b0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f4b0-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0f4b0-127">Request body</span></span>
<span data-ttu-id="0f4b0-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0f4b0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0f4b0-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="0f4b0-129">Response</span></span>
<span data-ttu-id="0f4b0-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0f4b0-130">If successful, this method returns a `200 OK` response code and [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f4b0-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0f4b0-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f4b0-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0f4b0-132">Request</span></span>
<span data-ttu-id="0f4b0-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0f4b0-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

### <a name="response"></a><span data-ttu-id="0f4b0-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="0f4b0-134">Response</span></span>
<span data-ttu-id="0f4b0-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0f4b0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 502

{
  "value": {
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
}
```



