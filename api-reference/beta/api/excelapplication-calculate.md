---
title: 'Anwendung: berechnen'
description: Alle in Excel geöffnete Arbeitsmappen werden neu berechnet.
ms.openlocfilehash: 5d2d0d5603f70691d2c73548bd7a20acc03c340e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062718"
---
# <a name="application-calculate"></a><span data-ttu-id="6f4db-103">Anwendung: berechnen</span><span class="sxs-lookup"><span data-stu-id="6f4db-103">Application: calculate</span></span>

> <span data-ttu-id="6f4db-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6f4db-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6f4db-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6f4db-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6f4db-106">Alle in Excel geöffnete Arbeitsmappen werden neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="6f4db-106">Recalculate all currently opened workbooks in Excel.</span></span>
## <a name="permissions"></a><span data-ttu-id="6f4db-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6f4db-107">Permissions</span></span>
<span data-ttu-id="6f4db-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f4db-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f4db-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6f4db-110">Permission type</span></span>      | <span data-ttu-id="6f4db-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6f4db-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f4db-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6f4db-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6f4db-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6f4db-113">Not supported.</span></span>    |
|<span data-ttu-id="6f4db-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6f4db-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f4db-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6f4db-115">Not supported.</span></span>    |
|<span data-ttu-id="6f4db-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6f4db-116">Application</span></span> | <span data-ttu-id="6f4db-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6f4db-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f4db-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6f4db-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/application/calculate

```
## <a name="request-headers"></a><span data-ttu-id="6f4db-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6f4db-119">Request headers</span></span>
| <span data-ttu-id="6f4db-120">Name</span><span class="sxs-lookup"><span data-stu-id="6f4db-120">Name</span></span>       | <span data-ttu-id="6f4db-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6f4db-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6f4db-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f4db-122">Authorization</span></span>  | <span data-ttu-id="6f4db-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6f4db-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6f4db-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6f4db-125">Request body</span></span>
<span data-ttu-id="6f4db-126">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="6f4db-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6f4db-127">Parameter</span><span class="sxs-lookup"><span data-stu-id="6f4db-127">Parameter</span></span>    | <span data-ttu-id="6f4db-128">Typ</span><span class="sxs-lookup"><span data-stu-id="6f4db-128">Type</span></span>   |<span data-ttu-id="6f4db-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6f4db-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6f4db-130">calculationType</span><span class="sxs-lookup"><span data-stu-id="6f4db-130">calculationType</span></span>|<span data-ttu-id="6f4db-131">string</span><span class="sxs-lookup"><span data-stu-id="6f4db-131">string</span></span>|<span data-ttu-id="6f4db-132">Gibt den Berechnungstyp verwendet.</span><span class="sxs-lookup"><span data-stu-id="6f4db-132">Specifies the calculation type to use.</span></span>  <span data-ttu-id="6f4db-133">Mögliche Werte sind: `Recalculate`, `Full` und `FullRebuild`.</span><span class="sxs-lookup"><span data-stu-id="6f4db-133">Possible values are: `Recalculate`, `Full`, `FullRebuild`.</span></span>|

## <a name="response"></a><span data-ttu-id="6f4db-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="6f4db-134">Response</span></span>

<span data-ttu-id="6f4db-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6f4db-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f4db-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6f4db-137">Example</span></span>
<span data-ttu-id="6f4db-138">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="6f4db-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6f4db-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6f4db-139">Request</span></span>
<span data-ttu-id="6f4db-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6f4db-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "application_calculate"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/application/calculate
Content-type: application/json
Content-length: 48

{
  "calculationType": "calculationType-value"
}
```

##### <a name="response"></a><span data-ttu-id="6f4db-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="6f4db-141">Response</span></span>
<span data-ttu-id="6f4db-142">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6f4db-142">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Application: calculate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->