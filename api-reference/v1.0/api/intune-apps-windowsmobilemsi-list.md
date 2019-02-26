---
title: Auflisten von „windowsMobileMSI“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs windowsMobileMSI auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ead9d9f74c7969fd5e8853dd581872e20a9f1ee5
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252532"
---
# <a name="list-windowsmobilemsis"></a><span data-ttu-id="ae310-103">Auflisten von „windowsMobileMSI“</span><span class="sxs-lookup"><span data-stu-id="ae310-103">List windowsMobileMSIs</span></span>

> <span data-ttu-id="ae310-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ae310-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae310-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) auf.</span><span class="sxs-lookup"><span data-stu-id="ae310-105">List properties and relationships of the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae310-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ae310-106">Prerequisites</span></span>
<span data-ttu-id="ae310-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ae310-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ae310-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ae310-109">Permission type</span></span>|<span data-ttu-id="ae310-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ae310-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae310-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ae310-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ae310-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae310-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ae310-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ae310-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae310-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ae310-114">Not supported.</span></span>|
|<span data-ttu-id="ae310-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ae310-115">Application</span></span>|<span data-ttu-id="ae310-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ae310-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae310-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ae310-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="ae310-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ae310-118">Request headers</span></span>
|<span data-ttu-id="ae310-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ae310-119">Header</span></span>|<span data-ttu-id="ae310-120">Wert</span><span class="sxs-lookup"><span data-stu-id="ae310-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae310-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae310-121">Authorization</span></span>|<span data-ttu-id="ae310-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ae310-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae310-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ae310-123">Accept</span></span>|<span data-ttu-id="ae310-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ae310-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae310-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ae310-125">Request body</span></span>
<span data-ttu-id="ae310-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ae310-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae310-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="ae310-127">Response</span></span>
<span data-ttu-id="ae310-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ae310-128">If successful, this method returns a `200 OK` response code and a collection of [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae310-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ae310-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae310-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ae310-130">Request</span></span>
<span data-ttu-id="ae310-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ae310-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="ae310-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="ae310-132">Response</span></span>
<span data-ttu-id="ae310-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ae310-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1164

{
  "value": [
    {
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
  ]
}
```



