---
title: Liste officeClientConfigurationAssignments
description: Listeneigenschaften und Beziehungen der OfficeClientConfigurationAssignment-Objekte.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e0a9a0c759bfc73ed5eeb998952f9634d1eb99ca
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886807"
---
# <a name="list-officeclientconfigurationassignments"></a><span data-ttu-id="ed963-103">Liste officeClientConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="ed963-103">List officeClientConfigurationAssignments</span></span>

> <span data-ttu-id="ed963-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ed963-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ed963-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ed963-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ed963-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ed963-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ed963-107">Listeneigenschaften und Beziehungen der [OfficeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="ed963-107">List properties and relationships of the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ed963-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ed963-108">Prerequisites</span></span>
<span data-ttu-id="ed963-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed963-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed963-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ed963-111">Permission type</span></span>|<span data-ttu-id="ed963-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ed963-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed963-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ed963-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ed963-114">\*\* Zu erledigen: Bestimmen der Bereiche \*\*</span><span class="sxs-lookup"><span data-stu-id="ed963-114">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="ed963-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ed963-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed963-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ed963-116">Not supported.</span></span>|
|<span data-ttu-id="ed963-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ed963-117">Application</span></span>|<span data-ttu-id="ed963-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ed963-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed963-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ed963-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="ed963-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ed963-120">Request headers</span></span>
|<span data-ttu-id="ed963-121">Header</span><span class="sxs-lookup"><span data-stu-id="ed963-121">Header</span></span>|<span data-ttu-id="ed963-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ed963-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed963-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed963-123">Authorization</span></span>|<span data-ttu-id="ed963-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ed963-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed963-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ed963-125">Accept</span></span>|<span data-ttu-id="ed963-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ed963-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed963-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ed963-127">Request body</span></span>
<span data-ttu-id="ed963-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ed963-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed963-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="ed963-129">Response</span></span>
<span data-ttu-id="ed963-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [OfficeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="ed963-130">If successful, this method returns a `200 OK` response code and a collection of [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed963-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ed963-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="ed963-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ed963-132">Request</span></span>
<span data-ttu-id="ed963-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ed963-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="ed963-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="ed963-134">Response</span></span>
<span data-ttu-id="ed963-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ed963-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 274

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
      "id": "804730f3-30f3-8047-f330-4780f3304780",
      "target": {
        "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
      }
    }
  ]
}
```



