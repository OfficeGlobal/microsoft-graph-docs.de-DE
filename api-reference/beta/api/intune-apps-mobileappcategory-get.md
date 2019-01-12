---
title: Abrufen von „mobileAppCategory“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs mobileAppCategory.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 50cb03496561a0b6d0c1d34405822d66b3e6cca6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956185"
---
# <a name="get-mobileappcategory"></a><span data-ttu-id="f5412-103">Abrufen von „mobileAppCategory“</span><span class="sxs-lookup"><span data-stu-id="f5412-103">Get mobileAppCategory</span></span>

> <span data-ttu-id="f5412-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f5412-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f5412-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f5412-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f5412-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f5412-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f5412-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="f5412-107">Read properties and relationships of the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f5412-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f5412-108">Prerequisites</span></span>
<span data-ttu-id="f5412-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5412-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5412-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f5412-111">Permission type</span></span>|<span data-ttu-id="f5412-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f5412-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5412-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f5412-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f5412-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f5412-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f5412-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f5412-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5412-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f5412-116">Not supported.</span></span>|
|<span data-ttu-id="f5412-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f5412-117">Application</span></span>|<span data-ttu-id="f5412-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f5412-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5412-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f5412-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/categories/{mobileAppCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f5412-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f5412-120">Optional query parameters</span></span>
<span data-ttu-id="f5412-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f5412-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f5412-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f5412-122">Request headers</span></span>
|<span data-ttu-id="f5412-123">Header</span><span class="sxs-lookup"><span data-stu-id="f5412-123">Header</span></span>|<span data-ttu-id="f5412-124">Wert</span><span class="sxs-lookup"><span data-stu-id="f5412-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f5412-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5412-125">Authorization</span></span>|<span data-ttu-id="f5412-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f5412-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f5412-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f5412-127">Accept</span></span>|<span data-ttu-id="f5412-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f5412-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5412-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f5412-129">Request body</span></span>
<span data-ttu-id="f5412-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f5412-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5412-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="f5412-131">Response</span></span>
<span data-ttu-id="f5412-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f5412-132">If successful, this method returns a `200 OK` response code and [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5412-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f5412-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="f5412-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f5412-134">Request</span></span>
<span data-ttu-id="f5412-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f5412-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
```

### <a name="response"></a><span data-ttu-id="f5412-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="f5412-136">Response</span></span>
<span data-ttu-id="f5412-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f5412-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 239

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppCategory",
    "id": "d85d9cee-9cee-d85d-ee9c-5dd8ee9c5dd8",
    "displayName": "Display Name value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
  }
}
```





