---
title: Auflisten von „managedEBook“
description: Auflisten von Eigenschaften und Beziehungen der managedEBook-Objekte.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: baf4b7275d9c6709a2d8959d2f82b806d0df01f4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807070"
---
# <a name="list-managedebooks"></a><span data-ttu-id="af1b2-103">Auflisten von „managedEBook“</span><span class="sxs-lookup"><span data-stu-id="af1b2-103">List managedEBooks</span></span>

> <span data-ttu-id="af1b2-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="af1b2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="af1b2-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [managedEBook](../resources/intune-books-managedebook.md) auf.</span><span class="sxs-lookup"><span data-stu-id="af1b2-105">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="af1b2-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="af1b2-106">Prerequisites</span></span>
<span data-ttu-id="af1b2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af1b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af1b2-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="af1b2-109">Permission type</span></span>|<span data-ttu-id="af1b2-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="af1b2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af1b2-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="af1b2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="af1b2-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="af1b2-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="af1b2-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="af1b2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af1b2-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="af1b2-114">Not supported.</span></span>|
|<span data-ttu-id="af1b2-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="af1b2-115">Application</span></span>|<span data-ttu-id="af1b2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="af1b2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="af1b2-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="af1b2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="af1b2-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="af1b2-118">Request headers</span></span>
|<span data-ttu-id="af1b2-119">Header</span><span class="sxs-lookup"><span data-stu-id="af1b2-119">Header</span></span>|<span data-ttu-id="af1b2-120">Wert</span><span class="sxs-lookup"><span data-stu-id="af1b2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af1b2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="af1b2-121">Authorization</span></span>|<span data-ttu-id="af1b2-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="af1b2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af1b2-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="af1b2-123">Accept</span></span>|<span data-ttu-id="af1b2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="af1b2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af1b2-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="af1b2-125">Request body</span></span>
<span data-ttu-id="af1b2-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="af1b2-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af1b2-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="af1b2-127">Response</span></span>
<span data-ttu-id="af1b2-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [managedEBook](../resources/intune-books-managedebook.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="af1b2-128">If successful, this method returns a `200 OK` response code and a collection of [managedEBook](../resources/intune-books-managedebook.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af1b2-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="af1b2-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="af1b2-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="af1b2-130">Request</span></span>
<span data-ttu-id="af1b2-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="af1b2-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks
```

### <a name="response"></a><span data-ttu-id="af1b2-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="af1b2-132">Response</span></span>
<span data-ttu-id="af1b2-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="af1b2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 756

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedEBook",
      "id": "1fbd3558-3558-1fbd-5835-bd1f5835bd1f",
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
      "privacyInformationUrl": "https://example.com/privacyInformationUrl/"
    }
  ]
}
```



