---
title: mobileThreatDefenseConnector abrufen
description: Liest die Eigenschaften und Beziehungen von Objekten des Typs mobileThreatDefenseConnector.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 88465dc4ddea56aa304d944276b284bcc4d987fb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395062"
---
# <a name="get-mobilethreatdefenseconnector"></a><span data-ttu-id="742d3-103">mobileThreatDefenseConnector abrufen</span><span class="sxs-lookup"><span data-stu-id="742d3-103">Get mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="742d3-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="742d3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="742d3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="742d3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="742d3-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="742d3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="742d3-107">Liest die Eigenschaften und Beziehungen von Objekten des Typs [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="742d3-107">Read properties and relationships of the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="742d3-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="742d3-108">Prerequisites</span></span>
<span data-ttu-id="742d3-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="742d3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="742d3-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="742d3-111">Permission type</span></span>|<span data-ttu-id="742d3-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="742d3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="742d3-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="742d3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="742d3-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="742d3-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="742d3-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="742d3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="742d3-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="742d3-116">Not supported.</span></span>|
|<span data-ttu-id="742d3-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="742d3-117">Application</span></span>|<span data-ttu-id="742d3-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="742d3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="742d3-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="742d3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="742d3-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="742d3-120">Optional query parameters</span></span>
<span data-ttu-id="742d3-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="742d3-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="742d3-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="742d3-122">Request headers</span></span>
|<span data-ttu-id="742d3-123">Header</span><span class="sxs-lookup"><span data-stu-id="742d3-123">Header</span></span>|<span data-ttu-id="742d3-124">Wert</span><span class="sxs-lookup"><span data-stu-id="742d3-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="742d3-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="742d3-125">Authorization</span></span>|<span data-ttu-id="742d3-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="742d3-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="742d3-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="742d3-127">Accept</span></span>|<span data-ttu-id="742d3-128">application/json</span><span class="sxs-lookup"><span data-stu-id="742d3-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="742d3-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="742d3-129">Request body</span></span>
<span data-ttu-id="742d3-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="742d3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="742d3-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="742d3-131">Response</span></span>
<span data-ttu-id="742d3-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="742d3-132">If successful, this method returns a `200 OK` response code and [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="742d3-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="742d3-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="742d3-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="742d3-134">Request</span></span>
<span data-ttu-id="742d3-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="742d3-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

### <a name="response"></a><span data-ttu-id="742d3-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="742d3-136">Response</span></span>
<span data-ttu-id="742d3-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="742d3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




