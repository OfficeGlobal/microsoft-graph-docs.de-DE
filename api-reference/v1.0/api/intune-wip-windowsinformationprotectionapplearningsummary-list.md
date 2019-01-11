---
title: windowsInformationProtectionAppLearningSummaries auflisten
description: Auflisten von Eigenschaften und Beziehungen der windowsInformationProtectionAppLearningSummary-Objekte.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a17427af37bf5adbc4c4511d08434df6db87397e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830632"
---
# <a name="list-windowsinformationprotectionapplearningsummaries"></a><span data-ttu-id="6a443-103">windowsInformationProtectionAppLearningSummaries auflisten</span><span class="sxs-lookup"><span data-stu-id="6a443-103">List windowsInformationProtectionAppLearningSummaries</span></span>

> <span data-ttu-id="6a443-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6a443-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6a443-105">Auflisten von Eigenschaften und Beziehungen der [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="6a443-105">List properties and relationships of the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6a443-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6a443-106">Prerequisites</span></span>
<span data-ttu-id="6a443-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a443-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a443-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6a443-109">Permission type</span></span>|<span data-ttu-id="6a443-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6a443-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a443-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6a443-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6a443-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a443-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6a443-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6a443-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a443-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6a443-114">Not supported.</span></span>|
|<span data-ttu-id="6a443-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6a443-115">Application</span></span>|<span data-ttu-id="6a443-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6a443-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a443-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6a443-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="6a443-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6a443-118">Request headers</span></span>
|<span data-ttu-id="6a443-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6a443-119">Header</span></span>|<span data-ttu-id="6a443-120">Wert</span><span class="sxs-lookup"><span data-stu-id="6a443-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a443-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a443-121">Authorization</span></span>|<span data-ttu-id="6a443-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6a443-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a443-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6a443-123">Accept</span></span>|<span data-ttu-id="6a443-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6a443-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a443-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6a443-125">Request body</span></span>
<span data-ttu-id="6a443-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6a443-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a443-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="6a443-127">Response</span></span>
<span data-ttu-id="6a443-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6a443-128">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a443-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6a443-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="6a443-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6a443-130">Request</span></span>
<span data-ttu-id="6a443-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6a443-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionAppLearningSummaries
```

### <a name="response"></a><span data-ttu-id="6a443-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="6a443-132">Response</span></span>
<span data-ttu-id="6a443-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6a443-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 293

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
      "id": "063baf50-af50-063b-50af-3b0650af3b06",
      "applicationName": "Application Name value",
      "applicationType": "desktop",
      "deviceCount": 11
    }
  ]
}
```



