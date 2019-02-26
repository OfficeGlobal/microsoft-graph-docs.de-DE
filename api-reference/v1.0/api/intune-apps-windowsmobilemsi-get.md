---
title: windowsMobileMSI abrufen
description: Liest die Eigenschaften und Beziehungen von Objekten des Typs windowsMobileMSI.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ab0084e9ab434cd642c5909e54ffde86372538e0
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257659"
---
# <a name="get-windowsmobilemsi"></a><span data-ttu-id="181b9-103">windowsMobileMSI abrufen</span><span class="sxs-lookup"><span data-stu-id="181b9-103">Get windowsMobileMSI</span></span>

> <span data-ttu-id="181b9-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="181b9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="181b9-105">Liest die Eigenschaften und Beziehungen von Objekten des Typs [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="181b9-105">Read properties and relationships of the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="181b9-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="181b9-106">Prerequisites</span></span>
<span data-ttu-id="181b9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="181b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="181b9-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="181b9-109">Permission type</span></span>|<span data-ttu-id="181b9-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="181b9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="181b9-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="181b9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="181b9-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="181b9-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="181b9-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="181b9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="181b9-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="181b9-114">Not supported.</span></span>|
|<span data-ttu-id="181b9-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="181b9-115">Application</span></span>|<span data-ttu-id="181b9-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="181b9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="181b9-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="181b9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="181b9-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="181b9-118">Optional query parameters</span></span>
<span data-ttu-id="181b9-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="181b9-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="181b9-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="181b9-120">Request headers</span></span>
|<span data-ttu-id="181b9-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="181b9-121">Header</span></span>|<span data-ttu-id="181b9-122">Wert</span><span class="sxs-lookup"><span data-stu-id="181b9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="181b9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="181b9-123">Authorization</span></span>|<span data-ttu-id="181b9-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="181b9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="181b9-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="181b9-125">Accept</span></span>|<span data-ttu-id="181b9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="181b9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="181b9-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="181b9-127">Request body</span></span>
<span data-ttu-id="181b9-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="181b9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="181b9-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="181b9-129">Response</span></span>
<span data-ttu-id="181b9-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="181b9-130">If successful, this method returns a `200 OK` response code and [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="181b9-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="181b9-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="181b9-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="181b9-132">Request</span></span>
<span data-ttu-id="181b9-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="181b9-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="181b9-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="181b9-134">Response</span></span>
<span data-ttu-id="181b9-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="181b9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1098

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsMobileMSI",
    "id": "aa453e5d-3e5d-aa45-5d3e-45aa5d3e45aa",
    "displayName": "Display Name value",
    "description": "Description value",
    "publisher": "Publisher value",
    "largeIcon": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "isFeatured": true,
    "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
    "informationUrl": "https://example.com/informationUrl/",
    "owner": "Owner value",
    "developer": "Developer value",
    "notes": "Notes value",
    "publishingState": "processing",
    "committedContentVersion": "Committed Content Version value",
    "fileName": "File Name value",
    "size": 4,
    "commandLine": "Command Line value",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "ignoreVersionDetection": true
  }
}
```



