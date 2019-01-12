---
title: Auflisten von „mobileAppCategory“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs mobileAppCategory auf.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b5b59f3020030c1aa1cf761af6edc52b0abef39e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919599"
---
# <a name="list-mobileappcategories"></a><span data-ttu-id="b4911-103">Auflisten von „mobileAppCategory“</span><span class="sxs-lookup"><span data-stu-id="b4911-103">List mobileAppCategories</span></span>

> <span data-ttu-id="b4911-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b4911-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b4911-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b4911-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b4911-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b4911-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b4911-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) auf.</span><span class="sxs-lookup"><span data-stu-id="b4911-107">List properties and relationships of the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b4911-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b4911-108">Prerequisites</span></span>
<span data-ttu-id="b4911-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4911-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4911-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b4911-111">Permission type</span></span>|<span data-ttu-id="b4911-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b4911-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4911-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b4911-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b4911-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b4911-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b4911-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b4911-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4911-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b4911-116">Not supported.</span></span>|
|<span data-ttu-id="b4911-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b4911-117">Application</span></span>|<span data-ttu-id="b4911-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b4911-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4911-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b4911-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppCategories
GET /deviceAppManagement/mobileApps/{mobileAppId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="b4911-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b4911-120">Request headers</span></span>
|<span data-ttu-id="b4911-121">Header</span><span class="sxs-lookup"><span data-stu-id="b4911-121">Header</span></span>|<span data-ttu-id="b4911-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b4911-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4911-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4911-123">Authorization</span></span>|<span data-ttu-id="b4911-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b4911-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4911-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b4911-125">Accept</span></span>|<span data-ttu-id="b4911-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b4911-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4911-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b4911-127">Request body</span></span>
<span data-ttu-id="b4911-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b4911-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4911-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="b4911-129">Response</span></span>
<span data-ttu-id="b4911-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b4911-130">If successful, this method returns a `200 OK` response code and a collection of [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4911-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b4911-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="b4911-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b4911-132">Request</span></span>
<span data-ttu-id="b4911-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b4911-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppCategories
```

### <a name="response"></a><span data-ttu-id="b4911-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="b4911-134">Response</span></span>
<span data-ttu-id="b4911-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b4911-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 261

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppCategory",
      "id": "d85d9cee-9cee-d85d-ee9c-5dd8ee9c5dd8",
      "displayName": "Display Name value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```





