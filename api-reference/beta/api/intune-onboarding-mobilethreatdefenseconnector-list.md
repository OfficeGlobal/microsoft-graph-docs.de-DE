---
title: mobileThreatDefenseConnectors auflisten
description: Listet die Eigenschaften und Beziehungen von Objekten des Typs mobileThreatDefenseConnector auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ebed9f772c7892982bcb101e7ebc1a69b7e32e1d
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30983631"
---
# <a name="list-mobilethreatdefenseconnectors"></a><span data-ttu-id="00b10-103">mobileThreatDefenseConnectors auflisten</span><span class="sxs-lookup"><span data-stu-id="00b10-103">List mobileThreatDefenseConnectors</span></span>

> <span data-ttu-id="00b10-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="00b10-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00b10-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="00b10-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00b10-106">Listet die Eigenschaften und Beziehungen von Objekten des Typs [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) auf.</span><span class="sxs-lookup"><span data-stu-id="00b10-106">List properties and relationships of the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="00b10-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="00b10-107">Prerequisites</span></span>
<span data-ttu-id="00b10-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00b10-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00b10-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="00b10-110">Permission type</span></span>|<span data-ttu-id="00b10-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="00b10-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00b10-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="00b10-112">Delegated (work or school account)</span></span>|<span data-ttu-id="00b10-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="00b10-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="00b10-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="00b10-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00b10-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="00b10-115">Not supported.</span></span>|
|<span data-ttu-id="00b10-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="00b10-116">Application</span></span>|<span data-ttu-id="00b10-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="00b10-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="00b10-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="00b10-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="00b10-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="00b10-119">Request headers</span></span>
|<span data-ttu-id="00b10-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="00b10-120">Header</span></span>|<span data-ttu-id="00b10-121">Wert</span><span class="sxs-lookup"><span data-stu-id="00b10-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00b10-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="00b10-122">Authorization</span></span>|<span data-ttu-id="00b10-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="00b10-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00b10-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="00b10-124">Accept</span></span>|<span data-ttu-id="00b10-125">application/json</span><span class="sxs-lookup"><span data-stu-id="00b10-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00b10-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="00b10-126">Request body</span></span>
<span data-ttu-id="00b10-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="00b10-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00b10-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="00b10-128">Response</span></span>
<span data-ttu-id="00b10-129">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="00b10-129">If successful, this method returns a `200 OK` response code and a collection of [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00b10-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="00b10-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="00b10-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="00b10-131">Request</span></span>
<span data-ttu-id="00b10-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="00b10-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors
```

### <a name="response"></a><span data-ttu-id="00b10-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="00b10-133">Response</span></span>
<span data-ttu-id="00b10-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="00b10-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 764

{
  "value": [
    {
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
  ]
}
```




