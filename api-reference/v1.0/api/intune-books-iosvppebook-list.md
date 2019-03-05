---
title: Auflisten von „iosVppEBook“
description: Listet die Eigenschaften und Beziehungen von Objekten des Typs iosVppEBook auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2f21ed4efab8548ebb972d441639256eb914029d
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256798"
---
# <a name="list-iosvppebooks"></a><span data-ttu-id="e3e6e-103">Auflisten von „iosVppEBook“</span><span class="sxs-lookup"><span data-stu-id="e3e6e-103">List iosVppEBooks</span></span>

> <span data-ttu-id="e3e6e-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e3e6e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3e6e-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [iosVppEBook](../resources/intune-books-iosvppebook.md) auf.</span><span class="sxs-lookup"><span data-stu-id="e3e6e-105">List properties and relationships of the [iosVppEBook](../resources/intune-books-iosvppebook.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e3e6e-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e3e6e-106">Prerequisites</span></span>
<span data-ttu-id="e3e6e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e3e6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e3e6e-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e3e6e-109">Permission type</span></span>|<span data-ttu-id="e3e6e-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e3e6e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3e6e-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e3e6e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e3e6e-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3e6e-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e3e6e-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e3e6e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3e6e-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e3e6e-114">Not supported.</span></span>|
|<span data-ttu-id="e3e6e-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e3e6e-115">Application</span></span>|<span data-ttu-id="e3e6e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e3e6e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3e6e-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e3e6e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="e3e6e-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e3e6e-118">Request headers</span></span>
|<span data-ttu-id="e3e6e-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e3e6e-119">Header</span></span>|<span data-ttu-id="e3e6e-120">Wert</span><span class="sxs-lookup"><span data-stu-id="e3e6e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3e6e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3e6e-121">Authorization</span></span>|<span data-ttu-id="e3e6e-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e3e6e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3e6e-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e3e6e-123">Accept</span></span>|<span data-ttu-id="e3e6e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e3e6e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3e6e-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e3e6e-125">Request body</span></span>
<span data-ttu-id="e3e6e-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e3e6e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3e6e-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="e3e6e-127">Response</span></span>
<span data-ttu-id="e3e6e-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [iosVppEBook](../resources/intune-books-iosvppebook.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e3e6e-128">If successful, this method returns a `200 OK` response code and a collection of [iosVppEBook](../resources/intune-books-iosvppebook.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3e6e-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e3e6e-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="e3e6e-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e3e6e-130">Request</span></span>
<span data-ttu-id="e3e6e-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e3e6e-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks
```

### <a name="response"></a><span data-ttu-id="e3e6e-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="e3e6e-132">Response</span></span>
<span data-ttu-id="e3e6e-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e3e6e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1097

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosVppEBook",
      "id": "3b9f627e-627e-3b9f-7e62-9f3b7e629f3b",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisher": "Publisher value",
      "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00",
      "largeCover": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "informationUrl": "https://example.com/informationUrl/",
      "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
      "vppTokenId": "9148ac60-ac60-9148-60ac-489160ac4891",
      "appleId": "Apple Id value",
      "vppOrganizationName": "Vpp Organization Name value",
      "genres": [
        "Genres value"
      ],
      "language": "Language value",
      "seller": "Seller value",
      "totalLicenseCount": 1,
      "usedLicenseCount": 0
    }
  ]
}
```



