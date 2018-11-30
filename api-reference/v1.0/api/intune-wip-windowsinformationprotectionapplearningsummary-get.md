---
title: windowsInformationProtectionAppLearningSummary abrufen
description: Lesen von Eigenschaften und Beziehungen des windowsInformationProtectionAppLearningSummary-Objekts.
ms.openlocfilehash: 48031664a5a8a1351a51f32fe94f9c071e79f918
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018608"
---
# <a name="get-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="6d541-103">windowsInformationProtectionAppLearningSummary abrufen</span><span class="sxs-lookup"><span data-stu-id="6d541-103">Get windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="6d541-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6d541-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6d541-105">Lesen von Eigenschaften und Beziehungen des [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6d541-105">Read properties and relationships of the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6d541-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6d541-106">Prerequisites</span></span>
<span data-ttu-id="6d541-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d541-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d541-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6d541-109">Permission type</span></span>|<span data-ttu-id="6d541-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6d541-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d541-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6d541-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6d541-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6d541-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6d541-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6d541-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d541-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6d541-114">Not supported.</span></span>|
|<span data-ttu-id="6d541-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6d541-115">Application</span></span>|<span data-ttu-id="6d541-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6d541-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d541-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6d541-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6d541-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="6d541-118">Optional query parameters</span></span>
<span data-ttu-id="6d541-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6d541-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6d541-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6d541-120">Request headers</span></span>
|<span data-ttu-id="6d541-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6d541-121">Header</span></span>|<span data-ttu-id="6d541-122">Wert</span><span class="sxs-lookup"><span data-stu-id="6d541-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d541-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d541-123">Authorization</span></span>|<span data-ttu-id="6d541-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6d541-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d541-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6d541-125">Accept</span></span>|<span data-ttu-id="6d541-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6d541-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d541-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6d541-127">Request body</span></span>
<span data-ttu-id="6d541-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6d541-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d541-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="6d541-129">Response</span></span>
<span data-ttu-id="6d541-130">Wenn erfolgreich, gibt diese Methode den `200 OK`-Antwortcode und das [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6d541-130">If successful, this method returns a `200 OK` response code and [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d541-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6d541-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="6d541-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6d541-132">Request</span></span>
<span data-ttu-id="6d541-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6d541-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

### <a name="response"></a><span data-ttu-id="6d541-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="6d541-134">Response</span></span>
<span data-ttu-id="6d541-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6d541-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 269

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
    "id": "063baf50-af50-063b-50af-3b0650af3b06",
    "applicationName": "Application Name value",
    "applicationType": "desktop",
    "deviceCount": 11
  }
}
```



