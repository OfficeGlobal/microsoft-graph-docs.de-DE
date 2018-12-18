---
title: ChartPoints erstellen
description: Verwenden Sie diese API, um neue ChartPoints zu erstellen.
author: lumine2008
ms.openlocfilehash: bc6d386b7508e98797fbaa79f9b79d066918518a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311578"
---
# <a name="create-chartpoints"></a><span data-ttu-id="3cbcf-103">ChartPoints erstellen</span><span class="sxs-lookup"><span data-stu-id="3cbcf-103">Create ChartPoints</span></span>

> <span data-ttu-id="3cbcf-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3cbcf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3cbcf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3cbcf-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3cbcf-106">Verwenden Sie diese API, um neue ChartPoints zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="3cbcf-106">Use this API to create a new ChartPoints.</span></span>
## <a name="permissions"></a><span data-ttu-id="3cbcf-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3cbcf-107">Permissions</span></span>
<span data-ttu-id="3cbcf-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3cbcf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cbcf-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3cbcf-110">Permission type</span></span>      | <span data-ttu-id="3cbcf-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3cbcf-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3cbcf-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3cbcf-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3cbcf-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3cbcf-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3cbcf-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3cbcf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3cbcf-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3cbcf-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3cbcf-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3cbcf-116">Application</span></span> | <span data-ttu-id="3cbcf-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3cbcf-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3cbcf-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3cbcf-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points

```
## <a name="request-headers"></a><span data-ttu-id="3cbcf-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3cbcf-119">Request headers</span></span>
| <span data-ttu-id="3cbcf-120">Name</span><span class="sxs-lookup"><span data-stu-id="3cbcf-120">Name</span></span>       | <span data-ttu-id="3cbcf-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3cbcf-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3cbcf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3cbcf-122">Authorization</span></span>  | <span data-ttu-id="3cbcf-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3cbcf-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3cbcf-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="3cbcf-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="3cbcf-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="3cbcf-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3cbcf-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3cbcf-128">Request body</span></span>
<span data-ttu-id="3cbcf-129">Geben Sie im Anforderungstext eine JSON-Darstellung des [ChartPoints](../resources/chartpoint.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="3cbcf-129">In the request body, supply a JSON representation of [ChartPoints](../resources/chartpoint.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3cbcf-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="3cbcf-130">Response</span></span>

<span data-ttu-id="3cbcf-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [ChartPoints](../resources/chartpoint.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3cbcf-131">If successful, this method returns `201 Created` response code and [ChartPoints](../resources/chartpoint.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3cbcf-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3cbcf-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3cbcf-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3cbcf-133">Request</span></span>
<span data-ttu-id="3cbcf-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3cbcf-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chartpoints_from_chartseries"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points
Content-type: application/json
Content-length: 3

{
}
```
<span data-ttu-id="3cbcf-135">Geben Sie im Anforderungstext eine JSON-Darstellung des [ChartPoints](../resources/chartpoint.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="3cbcf-135">In the request body, supply a JSON representation of [ChartPoints](../resources/chartpoint.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="3cbcf-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="3cbcf-136">Response</span></span>
<span data-ttu-id="3cbcf-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3cbcf-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartPoint"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 3

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create ChartPoints",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->