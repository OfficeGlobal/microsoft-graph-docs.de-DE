---
title: mobileThreatDefenseConnector abrufen
description: Liest die Eigenschaften und Beziehungen von Objekten des Typs mobileThreatDefenseConnector.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f8668ba21a4135cf15edf5d6b211859d072060e9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148692"
---
# <a name="get-mobilethreatdefenseconnector"></a><span data-ttu-id="e3993-103">mobileThreatDefenseConnector abrufen</span><span class="sxs-lookup"><span data-stu-id="e3993-103">Get mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="e3993-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e3993-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3993-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e3993-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3993-106">Liest die Eigenschaften und Beziehungen von Objekten des Typs [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="e3993-106">Read properties and relationships of the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e3993-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e3993-107">Prerequisites</span></span>
<span data-ttu-id="e3993-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e3993-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e3993-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e3993-110">Permission type</span></span>|<span data-ttu-id="e3993-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e3993-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3993-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e3993-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e3993-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3993-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="e3993-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e3993-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3993-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e3993-115">Not supported.</span></span>|
|<span data-ttu-id="e3993-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e3993-116">Application</span></span>|<span data-ttu-id="e3993-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e3993-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3993-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e3993-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e3993-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e3993-119">Optional query parameters</span></span>
<span data-ttu-id="e3993-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e3993-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e3993-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e3993-121">Request headers</span></span>
|<span data-ttu-id="e3993-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e3993-122">Header</span></span>|<span data-ttu-id="e3993-123">Wert</span><span class="sxs-lookup"><span data-stu-id="e3993-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3993-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3993-124">Authorization</span></span>|<span data-ttu-id="e3993-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e3993-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3993-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e3993-126">Accept</span></span>|<span data-ttu-id="e3993-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e3993-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3993-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e3993-128">Request body</span></span>
<span data-ttu-id="e3993-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e3993-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3993-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="e3993-130">Response</span></span>
<span data-ttu-id="e3993-131">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e3993-131">If successful, this method returns a `200 OK` response code and [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3993-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e3993-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e3993-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e3993-133">Request</span></span>
<span data-ttu-id="e3993-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e3993-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

### <a name="response"></a><span data-ttu-id="e3993-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="e3993-135">Response</span></span>
<span data-ttu-id="e3993-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e3993-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 720

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
    "id": "e4bede14-de14-e4be-14de-bee414debee4",
    "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
    "partnerState": "available",
    "androidEnabled": true,
    "iosEnabled": true,
    "windowsEnabled": true,
    "macEnabled": true,
    "androidDeviceBlockedOnMissingPartnerData": true,
    "iosDeviceBlockedOnMissingPartnerData": true,
    "windowsDeviceBlockedOnMissingPartnerData": true,
    "macDeviceBlockedOnMissingPartnerData": true,
    "partnerUnsupportedOsVersionBlocked": true,
    "partnerUnresponsivenessThresholdInDays": 6,
    "allowPartnerToCollectIOSApplicationMetadata": true
  }
}
```




