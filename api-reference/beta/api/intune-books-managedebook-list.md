---
title: Auflisten von „managedEBook“
description: Auflisten von Eigenschaften und Beziehungen der managedEBook-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3eee20e8db6518ac55420e9b6606196b0499d712
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164463"
---
# <a name="list-managedebooks"></a><span data-ttu-id="1221c-103">Auflisten von „managedEBook“</span><span class="sxs-lookup"><span data-stu-id="1221c-103">List managedEBooks</span></span>

> <span data-ttu-id="1221c-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1221c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1221c-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="1221c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1221c-106">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [managedEBook](../resources/intune-books-managedebook.md) auf.</span><span class="sxs-lookup"><span data-stu-id="1221c-106">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1221c-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1221c-107">Prerequisites</span></span>
<span data-ttu-id="1221c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1221c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1221c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1221c-110">Permission type</span></span>|<span data-ttu-id="1221c-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1221c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1221c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1221c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1221c-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1221c-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="1221c-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1221c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1221c-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1221c-115">Not supported.</span></span>|
|<span data-ttu-id="1221c-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1221c-116">Application</span></span>|<span data-ttu-id="1221c-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1221c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1221c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1221c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="1221c-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1221c-119">Request headers</span></span>
|<span data-ttu-id="1221c-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1221c-120">Header</span></span>|<span data-ttu-id="1221c-121">Wert</span><span class="sxs-lookup"><span data-stu-id="1221c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1221c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1221c-122">Authorization</span></span>|<span data-ttu-id="1221c-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1221c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1221c-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1221c-124">Accept</span></span>|<span data-ttu-id="1221c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1221c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1221c-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1221c-126">Request body</span></span>
<span data-ttu-id="1221c-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1221c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1221c-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="1221c-128">Response</span></span>
<span data-ttu-id="1221c-129">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [managedEBook](../resources/intune-books-managedebook.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1221c-129">If successful, this method returns a `200 OK` response code and a collection of [managedEBook](../resources/intune-books-managedebook.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1221c-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1221c-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="1221c-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1221c-131">Request</span></span>
<span data-ttu-id="1221c-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1221c-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks
```

### <a name="response"></a><span data-ttu-id="1221c-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="1221c-133">Response</span></span>
<span data-ttu-id="1221c-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1221c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




