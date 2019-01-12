---
title: Liste officeClientConfigurationAssignments
description: Listeneigenschaften und Beziehungen der OfficeClientConfigurationAssignment-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1e0398e5fe9773171ce8ba5d12c456a287185cdf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954421"
---
# <a name="list-officeclientconfigurationassignments"></a><span data-ttu-id="8238b-103">Liste officeClientConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="8238b-103">List officeClientConfigurationAssignments</span></span>

> <span data-ttu-id="8238b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8238b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8238b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8238b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8238b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8238b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8238b-107">Listeneigenschaften und Beziehungen der [OfficeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="8238b-107">List properties and relationships of the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8238b-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8238b-108">Prerequisites</span></span>
<span data-ttu-id="8238b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8238b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8238b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8238b-111">Permission type</span></span>|<span data-ttu-id="8238b-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8238b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8238b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8238b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8238b-114">\*\* Zu erledigen: Bestimmen der Bereiche \*\*</span><span class="sxs-lookup"><span data-stu-id="8238b-114">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="8238b-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8238b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8238b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8238b-116">Not supported.</span></span>|
|<span data-ttu-id="8238b-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8238b-117">Application</span></span>|<span data-ttu-id="8238b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8238b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8238b-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8238b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="8238b-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8238b-120">Request headers</span></span>
|<span data-ttu-id="8238b-121">Header</span><span class="sxs-lookup"><span data-stu-id="8238b-121">Header</span></span>|<span data-ttu-id="8238b-122">Wert</span><span class="sxs-lookup"><span data-stu-id="8238b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8238b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8238b-123">Authorization</span></span>|<span data-ttu-id="8238b-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8238b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8238b-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8238b-125">Accept</span></span>|<span data-ttu-id="8238b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8238b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8238b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8238b-127">Request body</span></span>
<span data-ttu-id="8238b-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8238b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8238b-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="8238b-129">Response</span></span>
<span data-ttu-id="8238b-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [OfficeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="8238b-130">If successful, this method returns a `200 OK` response code and a collection of [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8238b-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8238b-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="8238b-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8238b-132">Request</span></span>
<span data-ttu-id="8238b-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8238b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="8238b-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="8238b-134">Response</span></span>
<span data-ttu-id="8238b-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8238b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



