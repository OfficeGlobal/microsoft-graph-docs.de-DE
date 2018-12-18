---
title: Abrufen von „mobileAppCategory“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs mobileAppCategory.
author: tfitzmac
ms.openlocfilehash: 99ed0bb0159bd39efe417aa66950a13a5d2dbcfe
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349903"
---
# <a name="get-mobileappcategory"></a><span data-ttu-id="35d05-103">Abrufen von „mobileAppCategory“</span><span class="sxs-lookup"><span data-stu-id="35d05-103">Get mobileAppCategory</span></span>

> <span data-ttu-id="35d05-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="35d05-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="35d05-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="35d05-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="35d05-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="35d05-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="35d05-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="35d05-107">Read properties and relationships of the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="35d05-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="35d05-108">Prerequisites</span></span>
<span data-ttu-id="35d05-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35d05-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35d05-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="35d05-111">Permission type</span></span>|<span data-ttu-id="35d05-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="35d05-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35d05-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="35d05-113">Delegated (work or school account)</span></span>|<span data-ttu-id="35d05-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="35d05-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="35d05-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="35d05-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35d05-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="35d05-116">Not supported.</span></span>|
|<span data-ttu-id="35d05-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="35d05-117">Application</span></span>|<span data-ttu-id="35d05-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="35d05-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="35d05-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="35d05-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/categories/{mobileAppCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="35d05-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="35d05-120">Optional query parameters</span></span>
<span data-ttu-id="35d05-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="35d05-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="35d05-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="35d05-122">Request headers</span></span>
|<span data-ttu-id="35d05-123">Header</span><span class="sxs-lookup"><span data-stu-id="35d05-123">Header</span></span>|<span data-ttu-id="35d05-124">Wert</span><span class="sxs-lookup"><span data-stu-id="35d05-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35d05-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="35d05-125">Authorization</span></span>|<span data-ttu-id="35d05-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="35d05-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35d05-127">Accept</span><span class="sxs-lookup"><span data-stu-id="35d05-127">Accept</span></span>|<span data-ttu-id="35d05-128">application/json</span><span class="sxs-lookup"><span data-stu-id="35d05-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35d05-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="35d05-129">Request body</span></span>
<span data-ttu-id="35d05-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="35d05-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="35d05-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="35d05-131">Response</span></span>
<span data-ttu-id="35d05-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="35d05-132">If successful, this method returns a `200 OK` response code and [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35d05-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="35d05-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="35d05-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="35d05-134">Request</span></span>
<span data-ttu-id="35d05-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="35d05-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
```

### <a name="response"></a><span data-ttu-id="35d05-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="35d05-136">Response</span></span>
<span data-ttu-id="35d05-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="35d05-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





