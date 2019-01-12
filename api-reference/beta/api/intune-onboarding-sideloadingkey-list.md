---
title: Liste sideLoadingKeies
description: Listeneigenschaften und Beziehungen der SideLoadingKey-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a177e15bd60d4db5a90ab4a931ff950141114b30
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27958320"
---
# <a name="list-sideloadingkeies"></a><span data-ttu-id="b81fe-103">Liste sideLoadingKeies</span><span class="sxs-lookup"><span data-stu-id="b81fe-103">List sideLoadingKeies</span></span>

> <span data-ttu-id="b81fe-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b81fe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b81fe-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b81fe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b81fe-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b81fe-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b81fe-107">Listeneigenschaften und Beziehungen der [SideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="b81fe-107">List properties and relationships of the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b81fe-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b81fe-108">Prerequisites</span></span>
<span data-ttu-id="b81fe-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b81fe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b81fe-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b81fe-111">Permission type</span></span>|<span data-ttu-id="b81fe-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b81fe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b81fe-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b81fe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b81fe-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b81fe-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="b81fe-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b81fe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b81fe-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b81fe-116">Not supported.</span></span>|
|<span data-ttu-id="b81fe-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b81fe-117">Application</span></span>|<span data-ttu-id="b81fe-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b81fe-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b81fe-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b81fe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/sideLoadingKeys
```

## <a name="request-headers"></a><span data-ttu-id="b81fe-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b81fe-120">Request headers</span></span>
|<span data-ttu-id="b81fe-121">Header</span><span class="sxs-lookup"><span data-stu-id="b81fe-121">Header</span></span>|<span data-ttu-id="b81fe-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b81fe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b81fe-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b81fe-123">Authorization</span></span>|<span data-ttu-id="b81fe-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b81fe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b81fe-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b81fe-125">Accept</span></span>|<span data-ttu-id="b81fe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b81fe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b81fe-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b81fe-127">Request body</span></span>
<span data-ttu-id="b81fe-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b81fe-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b81fe-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="b81fe-129">Response</span></span>
<span data-ttu-id="b81fe-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [SideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) .</span><span class="sxs-lookup"><span data-stu-id="b81fe-130">If successful, this method returns a `200 OK` response code and a collection of [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b81fe-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b81fe-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="b81fe-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b81fe-132">Request</span></span>
<span data-ttu-id="b81fe-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b81fe-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/sideLoadingKeys
```

### <a name="response"></a><span data-ttu-id="b81fe-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="b81fe-134">Response</span></span>
<span data-ttu-id="b81fe-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b81fe-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 356

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.sideLoadingKey",
      "id": "21c4a3ff-a3ff-21c4-ffa3-c421ffa3c421",
      "value": "Value value",
      "displayName": "Display Name value",
      "description": "Description value",
      "totalActivation": 15,
      "lastUpdatedDateTime": "Last Updated Date Time value"
    }
  ]
}
```





