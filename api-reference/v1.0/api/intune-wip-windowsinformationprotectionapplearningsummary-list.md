---
title: windowsInformationProtectionAppLearningSummaries auflisten
description: Auflisten von Eigenschaften und Beziehungen der windowsInformationProtectionAppLearningSummary-Objekte.
author: tfitzmac
ms.openlocfilehash: 6fb2a4a9378ab7e5e0ce06ad896409cff95d0fdf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319313"
---
# <a name="list-windowsinformationprotectionapplearningsummaries"></a><span data-ttu-id="54d55-103">windowsInformationProtectionAppLearningSummaries auflisten</span><span class="sxs-lookup"><span data-stu-id="54d55-103">List windowsInformationProtectionAppLearningSummaries</span></span>

> <span data-ttu-id="54d55-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="54d55-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="54d55-105">Auflisten von Eigenschaften und Beziehungen der [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="54d55-105">List properties and relationships of the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="54d55-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="54d55-106">Prerequisites</span></span>
<span data-ttu-id="54d55-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54d55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54d55-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="54d55-109">Permission type</span></span>|<span data-ttu-id="54d55-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="54d55-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54d55-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="54d55-111">Delegated (work or school account)</span></span>|<span data-ttu-id="54d55-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="54d55-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="54d55-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="54d55-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54d55-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="54d55-114">Not supported.</span></span>|
|<span data-ttu-id="54d55-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="54d55-115">Application</span></span>|<span data-ttu-id="54d55-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="54d55-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="54d55-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="54d55-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="54d55-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="54d55-118">Request headers</span></span>
|<span data-ttu-id="54d55-119">Header</span><span class="sxs-lookup"><span data-stu-id="54d55-119">Header</span></span>|<span data-ttu-id="54d55-120">Wert</span><span class="sxs-lookup"><span data-stu-id="54d55-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54d55-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="54d55-121">Authorization</span></span>|<span data-ttu-id="54d55-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="54d55-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54d55-123">Accept</span><span class="sxs-lookup"><span data-stu-id="54d55-123">Accept</span></span>|<span data-ttu-id="54d55-124">application/json</span><span class="sxs-lookup"><span data-stu-id="54d55-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54d55-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="54d55-125">Request body</span></span>
<span data-ttu-id="54d55-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="54d55-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54d55-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="54d55-127">Response</span></span>
<span data-ttu-id="54d55-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="54d55-128">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54d55-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="54d55-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="54d55-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="54d55-130">Request</span></span>
<span data-ttu-id="54d55-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="54d55-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionAppLearningSummaries
```

### <a name="response"></a><span data-ttu-id="54d55-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="54d55-132">Response</span></span>
<span data-ttu-id="54d55-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="54d55-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



