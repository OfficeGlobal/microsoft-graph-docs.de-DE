---
title: Auflisten von „managedEBook“
description: Auflisten von Eigenschaften und Beziehungen der managedEBook-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 851d5bc4b507abfdc7ee78ed35f4c0d0fa59d813
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30983939"
---
# <a name="list-managedebooks"></a><span data-ttu-id="e6914-103">Auflisten von „managedEBook“</span><span class="sxs-lookup"><span data-stu-id="e6914-103">List managedEBooks</span></span>

> <span data-ttu-id="e6914-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e6914-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6914-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e6914-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6914-106">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [managedEBook](../resources/intune-books-managedebook.md) auf.</span><span class="sxs-lookup"><span data-stu-id="e6914-106">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e6914-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e6914-107">Prerequisites</span></span>
<span data-ttu-id="e6914-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6914-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6914-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e6914-110">Permission type</span></span>|<span data-ttu-id="e6914-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e6914-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6914-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e6914-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e6914-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e6914-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e6914-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e6914-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6914-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e6914-115">Not supported.</span></span>|
|<span data-ttu-id="e6914-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e6914-116">Application</span></span>|<span data-ttu-id="e6914-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e6914-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6914-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e6914-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="e6914-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e6914-119">Request headers</span></span>
|<span data-ttu-id="e6914-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e6914-120">Header</span></span>|<span data-ttu-id="e6914-121">Wert</span><span class="sxs-lookup"><span data-stu-id="e6914-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6914-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6914-122">Authorization</span></span>|<span data-ttu-id="e6914-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e6914-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6914-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e6914-124">Accept</span></span>|<span data-ttu-id="e6914-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e6914-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6914-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e6914-126">Request body</span></span>
<span data-ttu-id="e6914-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e6914-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6914-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="e6914-128">Response</span></span>
<span data-ttu-id="e6914-129">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [managedEBook](../resources/intune-books-managedebook.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e6914-129">If successful, this method returns a `200 OK` response code and a collection of [managedEBook](../resources/intune-books-managedebook.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6914-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e6914-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e6914-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e6914-131">Request</span></span>
<span data-ttu-id="e6914-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e6914-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks
```

### <a name="response"></a><span data-ttu-id="e6914-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="e6914-133">Response</span></span>
<span data-ttu-id="e6914-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e6914-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




