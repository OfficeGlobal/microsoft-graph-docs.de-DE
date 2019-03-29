---
title: mobileThreatDefenseConnectors auflisten
description: Listet die Eigenschaften und Beziehungen von Objekten des Typs mobileThreatDefenseConnector auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 103c9bd84c1c7c798b008c394ec855aaf6e0c89d
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30969820"
---
# <a name="list-mobilethreatdefenseconnectors"></a><span data-ttu-id="e8230-103">mobileThreatDefenseConnectors auflisten</span><span class="sxs-lookup"><span data-stu-id="e8230-103">List mobileThreatDefenseConnectors</span></span>

> <span data-ttu-id="e8230-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e8230-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8230-105">Listet die Eigenschaften und Beziehungen von Objekten des Typs [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) auf.</span><span class="sxs-lookup"><span data-stu-id="e8230-105">List properties and relationships of the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8230-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e8230-106">Prerequisites</span></span>
<span data-ttu-id="e8230-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8230-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8230-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e8230-109">Permission type</span></span>|<span data-ttu-id="e8230-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e8230-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8230-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e8230-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e8230-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8230-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="e8230-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e8230-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8230-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e8230-114">Not supported.</span></span>|
|<span data-ttu-id="e8230-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e8230-115">Application</span></span>|<span data-ttu-id="e8230-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e8230-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8230-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e8230-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="e8230-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e8230-118">Request headers</span></span>
|<span data-ttu-id="e8230-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e8230-119">Header</span></span>|<span data-ttu-id="e8230-120">Wert</span><span class="sxs-lookup"><span data-stu-id="e8230-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8230-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8230-121">Authorization</span></span>|<span data-ttu-id="e8230-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e8230-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8230-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e8230-123">Accept</span></span>|<span data-ttu-id="e8230-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e8230-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8230-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e8230-125">Request body</span></span>
<span data-ttu-id="e8230-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e8230-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8230-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="e8230-127">Response</span></span>
<span data-ttu-id="e8230-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e8230-128">If successful, this method returns a `200 OK` response code and a collection of [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8230-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e8230-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8230-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e8230-130">Request</span></span>
<span data-ttu-id="e8230-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e8230-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/mobileThreatDefenseConnectors
```

### <a name="response"></a><span data-ttu-id="e8230-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="e8230-132">Response</span></span>
<span data-ttu-id="e8230-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e8230-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



