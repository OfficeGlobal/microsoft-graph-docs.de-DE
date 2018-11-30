---
title: Tabelle aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des Tabellenobjekts.
ms.openlocfilehash: a929329ed9a88b7dda6206193292f1ca1e63ced1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061319"
---
# <a name="update-table"></a><span data-ttu-id="163d2-103">Tabelle aktualisieren</span><span class="sxs-lookup"><span data-stu-id="163d2-103">Update table</span></span>

> <span data-ttu-id="163d2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="163d2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="163d2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="163d2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="163d2-106">Dient zum Aktualisieren der Eigenschaften des Tabellenobjekts.</span><span class="sxs-lookup"><span data-stu-id="163d2-106">Update the properties of table object.</span></span>
## <a name="permissions"></a><span data-ttu-id="163d2-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="163d2-107">Permissions</span></span>
<span data-ttu-id="163d2-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="163d2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="163d2-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="163d2-110">Permission type</span></span>      | <span data-ttu-id="163d2-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="163d2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="163d2-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="163d2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="163d2-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="163d2-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="163d2-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="163d2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="163d2-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="163d2-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="163d2-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="163d2-116">Application</span></span> | <span data-ttu-id="163d2-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="163d2-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="163d2-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="163d2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}
PATCH /workbook/worksheets/{id|name}/tables/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="163d2-119">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="163d2-119">Optional request headers</span></span>
| <span data-ttu-id="163d2-120">Name</span><span class="sxs-lookup"><span data-stu-id="163d2-120">Name</span></span>       | <span data-ttu-id="163d2-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="163d2-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="163d2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="163d2-122">Authorization</span></span>  | <span data-ttu-id="163d2-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="163d2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="163d2-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="163d2-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="163d2-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="163d2-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="163d2-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="163d2-128">Request body</span></span>
<span data-ttu-id="163d2-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="163d2-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="163d2-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="163d2-132">Property</span></span>     | <span data-ttu-id="163d2-133">Typ</span><span class="sxs-lookup"><span data-stu-id="163d2-133">Type</span></span>   |<span data-ttu-id="163d2-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="163d2-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="163d2-135">name</span><span class="sxs-lookup"><span data-stu-id="163d2-135">name</span></span>|<span data-ttu-id="163d2-136">string</span><span class="sxs-lookup"><span data-stu-id="163d2-136">string</span></span>|<span data-ttu-id="163d2-137">Der Name der Tabelle.</span><span class="sxs-lookup"><span data-stu-id="163d2-137">Name of the table.</span></span>|
|<span data-ttu-id="163d2-138">showHeaders</span><span class="sxs-lookup"><span data-stu-id="163d2-138">showHeaders</span></span>|<span data-ttu-id="163d2-139">boolean</span><span class="sxs-lookup"><span data-stu-id="163d2-139">boolean</span></span>|<span data-ttu-id="163d2-p106">Gibt an, ob die Kopfzeile sichtbar oder nicht sichtbar ist. Dieser Wert kann festgelegt werden, um die Kopfzeile anzuzeigen, oder sie zu entfernen.</span><span class="sxs-lookup"><span data-stu-id="163d2-p106">Indicates whether the header row is visible or not. This value can be set to show or remove the header row.</span></span>|
|<span data-ttu-id="163d2-142">showTotals</span><span class="sxs-lookup"><span data-stu-id="163d2-142">showTotals</span></span>|<span data-ttu-id="163d2-143">boolean</span><span class="sxs-lookup"><span data-stu-id="163d2-143">boolean</span></span>|<span data-ttu-id="163d2-p107">Gibt an, ob die Ergebniszeile sichtbar ist oder nicht. Dieser Wert kann so festgelegt werden, dass die Ergebniszeile angezeigt oder ausgeblendet wird.</span><span class="sxs-lookup"><span data-stu-id="163d2-p107">Indicates whether the total row is visible or not. This value can be set to show or remove the total row.</span></span>|
|<span data-ttu-id="163d2-146">style</span><span class="sxs-lookup"><span data-stu-id="163d2-146">style</span></span>|<span data-ttu-id="163d2-147">string</span><span class="sxs-lookup"><span data-stu-id="163d2-147">string</span></span>|<span data-ttu-id="163d2-p108">Konstanter Wert, der das Tabellenformat darstellt. Die folgenden Werte sind möglich: TableStyleLight1 thru TableStyleLight21, TableStyleMedium1 thru TableStyleMedium28, TableStyleStyleDark1 thru TableStyleStyleDark11. Es kann ebenfalls eine in der Arbeitsmappe vorhandene benutzerdefinierte Formatierung angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="163d2-p108">Constant value that represents the Table style. Possible values are: TableStyleLight1 thru TableStyleLight21, TableStyleMedium1 thru TableStyleMedium28, TableStyleStyleDark1 thru TableStyleStyleDark11. A custom user-defined style present in the workbook can also be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="163d2-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="163d2-151">Response</span></span>

<span data-ttu-id="163d2-152">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [Table](../resources/table.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="163d2-152">If successful, this method returns a `200 OK` response code and updated [Table](../resources/table.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="163d2-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="163d2-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="163d2-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="163d2-154">Request</span></span>
<span data-ttu-id="163d2-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="163d2-155">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_table"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}
Content-type: application/json
Content-length: 109

{
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```
##### <a name="response"></a><span data-ttu-id="163d2-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="163d2-156">Response</span></span>
<span data-ttu-id="163d2-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="163d2-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.table"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 109

{
  "id": "99",
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update table",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->