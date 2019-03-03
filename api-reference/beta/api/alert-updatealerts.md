---
title: 'Warnung: updateAlerts'
description: Aktualisieren Sie mehrere Warnungen in einer Anforderung anstelle mehrerer Anforderungen.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 5be6374d70baaf4205d5fc1e431111844ce34313
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366994"
---
# <a name="alert-updatealerts"></a><span data-ttu-id="018cd-103">Warnung: updateAlerts</span><span class="sxs-lookup"><span data-stu-id="018cd-103">alert: updateAlerts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="018cd-104">Aktualisieren Sie mehrere Warnungen in einer Anforderung anstelle mehrerer Anforderungen.</span><span class="sxs-lookup"><span data-stu-id="018cd-104">Update multiple alerts in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="018cd-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="018cd-105">Permissions</span></span>

<span data-ttu-id="018cd-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="018cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="018cd-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="018cd-108">Permission type</span></span>                        | <span data-ttu-id="018cd-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="018cd-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="018cd-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="018cd-110">Delegated (work or school account)</span></span> |   <span data-ttu-id="018cd-111">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="018cd-111">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="018cd-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="018cd-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="018cd-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="018cd-113">Not supported.</span></span>  |
|<span data-ttu-id="018cd-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="018cd-114">Application</span></span> | <span data-ttu-id="018cd-115">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="018cd-115">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="018cd-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="018cd-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/alerts/updateAlerts
```

## <a name="request-headers"></a><span data-ttu-id="018cd-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="018cd-117">Request headers</span></span>

| <span data-ttu-id="018cd-118">Name</span><span class="sxs-lookup"><span data-stu-id="018cd-118">Name</span></span>          | <span data-ttu-id="018cd-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="018cd-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="018cd-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="018cd-120">Authorization</span></span> | <span data-ttu-id="018cd-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="018cd-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="018cd-122">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="018cd-122">Request body</span></span>

<span data-ttu-id="018cd-123">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="018cd-123">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="018cd-124">Jede Entität muss über **ID** -und **vendorInformation** -Eigenschaften verfügen.</span><span class="sxs-lookup"><span data-stu-id="018cd-124">Each entity must have **id** and **vendorInformation** properties.</span></span> <span data-ttu-id="018cd-125">Ausführliche Informationen zu Eigenschaften, die aktualisiert werden können, finden Sie unter [updatealert](alert-update.md).</span><span class="sxs-lookup"><span data-stu-id="018cd-125">For details about properties that can be updated, see [update alert](alert-update.md).</span></span>

| <span data-ttu-id="018cd-126">Parameter</span><span class="sxs-lookup"><span data-stu-id="018cd-126">Parameter</span></span>    | <span data-ttu-id="018cd-127">Typ</span><span class="sxs-lookup"><span data-stu-id="018cd-127">Type</span></span>        | <span data-ttu-id="018cd-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="018cd-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="018cd-129">Wert</span><span class="sxs-lookup"><span data-stu-id="018cd-129">value</span></span>|<span data-ttu-id="018cd-130">[Warnungs](../resources/alert.md) Sammlung</span><span class="sxs-lookup"><span data-stu-id="018cd-130">[alert](../resources/alert.md) collection</span></span>| <span data-ttu-id="018cd-131">Sammlung von zu aktualisierende Warnungen.</span><span class="sxs-lookup"><span data-stu-id="018cd-131">Collection of alerts to update.</span></span> <span data-ttu-id="018cd-132">Jede Entität muss **ID**, **vendorInformation**und andere bearbeitbare Eigenschaften haben, die aktualisiert werden müssen.</span><span class="sxs-lookup"><span data-stu-id="018cd-132">Each entity must have **id**, **vendorInformation**, and other editable properties to be updated.</span></span>|

## <a name="response"></a><span data-ttu-id="018cd-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="018cd-133">Response</span></span>

<span data-ttu-id="018cd-134">Bei erfolgreicher Ausführung gibt diese Methode `200, OK` den Antwortcode und das [Alert](../resources/alert.md) -Auflistungsobjekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="018cd-134">If successful, this method returns `200, OK` response code and [alert](../resources/alert.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="018cd-135">Beispiele</span><span class="sxs-lookup"><span data-stu-id="018cd-135">Examples</span></span>

<span data-ttu-id="018cd-136">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="018cd-136">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="018cd-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="018cd-137">Request</span></span>

<span data-ttu-id="018cd-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="018cd-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "alert_updatealerts"
}-->

```http
POST https://graph.microsoft.com/beta/security/alerts/updateAlerts
Content-type: application/json

{
  "value": [
    {
      "assignedTo": "String",
      "closedDateTime": "String (timestamp)",
      "comments": ["String"],
      "feedback": "@odata.type: microsoft.graph.alertFeedback",
      "id": "String (identifier)",
      "status": "@odata.type: microsoft.graph.alertStatus",
      "tags": ["String"],
      "vendorInformation":
        {
          "provider": "String",
          "vendor": "String"
        }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="018cd-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="018cd-139">Response</span></span>

<span data-ttu-id="018cd-140">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="018cd-140">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="018cd-141">Das hier gezeigte Antwortobjekt kann zur Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="018cd-141">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="018cd-142">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="018cd-142">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
{
  "value": [
    {
      "activityGroupName": "activityGroupName-value",
      "assignedTo": "assignedTo-value",
      "azureSubscriptionId": "azureSubscriptionId-value",
      "azureTenantId": "azureTenantId-value",
      "category": "category-value",
      "closedDateTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alert: updateAlerts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
