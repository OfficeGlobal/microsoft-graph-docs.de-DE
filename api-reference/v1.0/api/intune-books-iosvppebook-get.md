---
title: iosVppEBook abrufen
description: Liest die Eigenschaften und Beziehungen von Objekten des Typs iosVppEBook.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0213d300116c96cacece538223c4af32152491de
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260711"
---
# <a name="get-iosvppebook"></a><span data-ttu-id="b0922-103">iosVppEBook abrufen</span><span class="sxs-lookup"><span data-stu-id="b0922-103">Get iosVppEBook</span></span>

> <span data-ttu-id="b0922-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b0922-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0922-105">Liest die Eigenschaften und Beziehungen von Objekten des Typs [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="b0922-105">Read properties and relationships of the [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b0922-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b0922-106">Prerequisites</span></span>
<span data-ttu-id="b0922-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b0922-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b0922-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b0922-109">Permission type</span></span>|<span data-ttu-id="b0922-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b0922-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0922-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b0922-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b0922-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b0922-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b0922-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b0922-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0922-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b0922-114">Not supported.</span></span>|
|<span data-ttu-id="b0922-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b0922-115">Application</span></span>|<span data-ttu-id="b0922-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b0922-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0922-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b0922-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b0922-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b0922-118">Optional query parameters</span></span>
<span data-ttu-id="b0922-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b0922-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b0922-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b0922-120">Request headers</span></span>
|<span data-ttu-id="b0922-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b0922-121">Header</span></span>|<span data-ttu-id="b0922-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b0922-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0922-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0922-123">Authorization</span></span>|<span data-ttu-id="b0922-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b0922-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0922-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b0922-125">Accept</span></span>|<span data-ttu-id="b0922-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b0922-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0922-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b0922-127">Request body</span></span>
<span data-ttu-id="b0922-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b0922-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0922-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="b0922-129">Response</span></span>
<span data-ttu-id="b0922-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [iosVppEBook](../resources/intune-books-iosvppebook.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b0922-130">If successful, this method returns a `200 OK` response code and [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0922-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b0922-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0922-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b0922-132">Request</span></span>
<span data-ttu-id="b0922-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b0922-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}
```

### <a name="response"></a><span data-ttu-id="b0922-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="b0922-134">Response</span></span>
<span data-ttu-id="b0922-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b0922-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1033

{
  "value": {
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
}
```



