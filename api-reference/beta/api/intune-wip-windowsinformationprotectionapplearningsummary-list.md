---
title: windowsInformationProtectionAppLearningSummaries auflisten
description: Auflisten von Eigenschaften und Beziehungen der windowsInformationProtectionAppLearningSummary-Objekte.
ms.openlocfilehash: 3d5616b772f3219889c942fe9e65569ecccb25ed
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061011"
---
# <a name="list-windowsinformationprotectionapplearningsummaries"></a><span data-ttu-id="ce680-103">windowsInformationProtectionAppLearningSummaries auflisten</span><span class="sxs-lookup"><span data-stu-id="ce680-103">List windowsInformationProtectionAppLearningSummaries</span></span>

> <span data-ttu-id="ce680-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ce680-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ce680-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ce680-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ce680-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ce680-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ce680-107">Auflisten von Eigenschaften und Beziehungen der [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="ce680-107">List properties and relationships of the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ce680-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ce680-108">Prerequisites</span></span>
<span data-ttu-id="ce680-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce680-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce680-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ce680-111">Permission type</span></span>|<span data-ttu-id="ce680-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ce680-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce680-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ce680-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ce680-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ce680-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ce680-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ce680-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce680-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ce680-116">Not supported.</span></span>|
|<span data-ttu-id="ce680-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ce680-117">Application</span></span>|<span data-ttu-id="ce680-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ce680-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce680-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ce680-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="ce680-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ce680-120">Request headers</span></span>
|<span data-ttu-id="ce680-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ce680-121">Header</span></span>|<span data-ttu-id="ce680-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ce680-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce680-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce680-123">Authorization</span></span>|<span data-ttu-id="ce680-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ce680-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce680-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ce680-125">Accept</span></span>|<span data-ttu-id="ce680-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ce680-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce680-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ce680-127">Request body</span></span>
<span data-ttu-id="ce680-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ce680-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce680-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="ce680-129">Response</span></span>
<span data-ttu-id="ce680-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ce680-130">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce680-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ce680-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="ce680-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ce680-132">Request</span></span>
<span data-ttu-id="ce680-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ce680-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionAppLearningSummaries
```

### <a name="response"></a><span data-ttu-id="ce680-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="ce680-134">Response</span></span>
<span data-ttu-id="ce680-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ce680-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





