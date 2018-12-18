---
title: Liste embeddedSIMActivationCodePoolAssignments
description: Listeneigenschaften und Beziehungen der EmbeddedSIMActivationCodePoolAssignment-Objekte.
author: tfitzmac
ms.openlocfilehash: 798701e538d1eabe7d49350efdb16777deee3dea
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352927"
---
# <a name="list-embeddedsimactivationcodepoolassignments"></a><span data-ttu-id="824b6-103">Liste embeddedSIMActivationCodePoolAssignments</span><span class="sxs-lookup"><span data-stu-id="824b6-103">List embeddedSIMActivationCodePoolAssignments</span></span>

> <span data-ttu-id="824b6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="824b6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="824b6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="824b6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="824b6-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="824b6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="824b6-107">Listeneigenschaften und Beziehungen der [EmbeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="824b6-107">List properties and relationships of the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="824b6-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="824b6-108">Prerequisites</span></span>
<span data-ttu-id="824b6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="824b6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="824b6-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="824b6-111">Permission type</span></span>|<span data-ttu-id="824b6-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="824b6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="824b6-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="824b6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="824b6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="824b6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="824b6-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="824b6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="824b6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="824b6-116">Not supported.</span></span>|
|<span data-ttu-id="824b6-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="824b6-117">Application</span></span>|<span data-ttu-id="824b6-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="824b6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="824b6-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="824b6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="824b6-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="824b6-120">Request headers</span></span>
|<span data-ttu-id="824b6-121">Header</span><span class="sxs-lookup"><span data-stu-id="824b6-121">Header</span></span>|<span data-ttu-id="824b6-122">Wert</span><span class="sxs-lookup"><span data-stu-id="824b6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="824b6-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="824b6-123">Authorization</span></span>|<span data-ttu-id="824b6-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="824b6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="824b6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="824b6-125">Accept</span></span>|<span data-ttu-id="824b6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="824b6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="824b6-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="824b6-127">Request body</span></span>
<span data-ttu-id="824b6-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="824b6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="824b6-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="824b6-129">Response</span></span>
<span data-ttu-id="824b6-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [EmbeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="824b6-130">If successful, this method returns a `200 OK` response code and a collection of [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="824b6-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="824b6-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="824b6-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="824b6-132">Request</span></span>
<span data-ttu-id="824b6-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="824b6-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments
```

### <a name="response"></a><span data-ttu-id="824b6-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="824b6-134">Response</span></span>
<span data-ttu-id="824b6-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="824b6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 281

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
      "id": "e7304dcc-4dcc-e730-cc4d-30e7cc4d30e7",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```





