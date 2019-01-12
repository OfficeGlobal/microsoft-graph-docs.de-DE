---
title: managedEBook abrufen
description: Lesen von Eigenschaften und Beziehungen des managedEBook-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 88ebfec3265f467fb3441b6c0d0e9753b489b3c2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950151"
---
# <a name="get-managedebook"></a><span data-ttu-id="ece89-103">managedEBook abrufen</span><span class="sxs-lookup"><span data-stu-id="ece89-103">Get managedEBook</span></span>

> <span data-ttu-id="ece89-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ece89-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ece89-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ece89-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ece89-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ece89-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ece89-107">Lesen von Eigenschaften und Beziehungen des [managedEBook](../resources/intune-books-managedebook.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ece89-107">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ece89-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ece89-108">Prerequisites</span></span>
<span data-ttu-id="ece89-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ece89-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ece89-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ece89-111">Permission type</span></span>|<span data-ttu-id="ece89-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ece89-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ece89-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ece89-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ece89-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ece89-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ece89-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ece89-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ece89-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ece89-116">Not supported.</span></span>|
|<span data-ttu-id="ece89-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ece89-117">Application</span></span>|<span data-ttu-id="ece89-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ece89-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ece89-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ece89-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ece89-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ece89-120">Optional query parameters</span></span>
<span data-ttu-id="ece89-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ece89-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ece89-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ece89-122">Request headers</span></span>
|<span data-ttu-id="ece89-123">Header</span><span class="sxs-lookup"><span data-stu-id="ece89-123">Header</span></span>|<span data-ttu-id="ece89-124">Wert</span><span class="sxs-lookup"><span data-stu-id="ece89-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ece89-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ece89-125">Authorization</span></span>|<span data-ttu-id="ece89-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ece89-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ece89-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ece89-127">Accept</span></span>|<span data-ttu-id="ece89-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ece89-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ece89-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ece89-129">Request body</span></span>
<span data-ttu-id="ece89-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ece89-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ece89-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="ece89-131">Response</span></span>
<span data-ttu-id="ece89-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [managedEBook](../resources/intune-books-managedebook.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ece89-132">If successful, this method returns a `200 OK` response code and [managedEBook](../resources/intune-books-managedebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ece89-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ece89-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="ece89-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ece89-134">Request</span></span>
<span data-ttu-id="ece89-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ece89-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}
```

### <a name="response"></a><span data-ttu-id="ece89-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="ece89-136">Response</span></span>
<span data-ttu-id="ece89-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ece89-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





