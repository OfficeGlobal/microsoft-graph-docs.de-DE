---
title: managedEBook abrufen
description: Lesen von Eigenschaften und Beziehungen des managedEBook-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 02dbbccae1e3ba04cf087b1509c69fe2500e8854
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30965025"
---
# <a name="get-managedebook"></a><span data-ttu-id="b79cf-103">managedEBook abrufen</span><span class="sxs-lookup"><span data-stu-id="b79cf-103">Get managedEBook</span></span>

> <span data-ttu-id="b79cf-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b79cf-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b79cf-105">Lesen von Eigenschaften und Beziehungen des [managedEBook](../resources/intune-books-managedebook.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b79cf-105">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b79cf-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b79cf-106">Prerequisites</span></span>
<span data-ttu-id="b79cf-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b79cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b79cf-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b79cf-109">Permission type</span></span>|<span data-ttu-id="b79cf-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b79cf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b79cf-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b79cf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b79cf-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b79cf-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b79cf-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b79cf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b79cf-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b79cf-114">Not supported.</span></span>|
|<span data-ttu-id="b79cf-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b79cf-115">Application</span></span>|<span data-ttu-id="b79cf-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b79cf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b79cf-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b79cf-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b79cf-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b79cf-118">Optional query parameters</span></span>
<span data-ttu-id="b79cf-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b79cf-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b79cf-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b79cf-120">Request headers</span></span>
|<span data-ttu-id="b79cf-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b79cf-121">Header</span></span>|<span data-ttu-id="b79cf-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b79cf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b79cf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b79cf-123">Authorization</span></span>|<span data-ttu-id="b79cf-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b79cf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b79cf-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b79cf-125">Accept</span></span>|<span data-ttu-id="b79cf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b79cf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b79cf-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b79cf-127">Request body</span></span>
<span data-ttu-id="b79cf-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b79cf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b79cf-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="b79cf-129">Response</span></span>
<span data-ttu-id="b79cf-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [managedEBook](../resources/intune-books-managedebook.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b79cf-130">If successful, this method returns a `200 OK` response code and [managedEBook](../resources/intune-books-managedebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b79cf-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b79cf-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b79cf-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b79cf-132">Request</span></span>
<span data-ttu-id="b79cf-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b79cf-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}
```

### <a name="response"></a><span data-ttu-id="b79cf-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="b79cf-134">Response</span></span>
<span data-ttu-id="b79cf-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b79cf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 712

{
  "value": {
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
}
```



