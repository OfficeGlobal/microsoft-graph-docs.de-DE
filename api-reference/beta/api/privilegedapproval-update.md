---
title: Privilegedapproval aktualisieren
description: Aktualisieren Sie die Eigenschaften des Privilegedapproval-Objekts.
localization_priority: Normal
ms.openlocfilehash: cb108ca35b07138f84a9fd969bfe7c7241e9672e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524898"
---
# <a name="update-privilegedapproval"></a><span data-ttu-id="e86c1-103">Privilegedapproval aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e86c1-103">Update privilegedapproval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e86c1-104">Aktualisieren Sie die Eigenschaften des Privilegedapproval-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e86c1-104">Update the properties of privilegedapproval object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e86c1-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e86c1-105">Permissions</span></span>
<span data-ttu-id="e86c1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e86c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e86c1-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e86c1-108">Permission type</span></span>      | <span data-ttu-id="e86c1-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e86c1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e86c1-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e86c1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e86c1-111">PrivilegedAccess.ReadWrite.AzureAD Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e86c1-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e86c1-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e86c1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e86c1-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e86c1-113">Not supported.</span></span>    |
|<span data-ttu-id="e86c1-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e86c1-114">Application</span></span> | <span data-ttu-id="e86c1-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e86c1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e86c1-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e86c1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedApproval/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="e86c1-117">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e86c1-117">Optional request headers</span></span>
| <span data-ttu-id="e86c1-118">Name</span><span class="sxs-lookup"><span data-stu-id="e86c1-118">Name</span></span>       | <span data-ttu-id="e86c1-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e86c1-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e86c1-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e86c1-120">Authorization</span></span>  | <span data-ttu-id="e86c1-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e86c1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e86c1-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e86c1-123">Request body</span></span>
<span data-ttu-id="e86c1-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="e86c1-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e86c1-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e86c1-127">Property</span></span>     | <span data-ttu-id="e86c1-128">Typ</span><span class="sxs-lookup"><span data-stu-id="e86c1-128">Type</span></span>   |<span data-ttu-id="e86c1-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e86c1-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e86c1-130">approvalDuration</span><span class="sxs-lookup"><span data-stu-id="e86c1-130">approvalDuration</span></span>|<span data-ttu-id="e86c1-131">Dauer</span><span class="sxs-lookup"><span data-stu-id="e86c1-131">Duration</span></span>||
|<span data-ttu-id="e86c1-132">approvalState</span><span class="sxs-lookup"><span data-stu-id="e86c1-132">approvalState</span></span>|<span data-ttu-id="e86c1-133">string</span><span class="sxs-lookup"><span data-stu-id="e86c1-133">string</span></span>| <span data-ttu-id="e86c1-134">Mögliche Werte sind: `pending`, `approved`, `denied`, `aborted` und `canceled`.</span><span class="sxs-lookup"><span data-stu-id="e86c1-134">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="e86c1-135">approvalType</span><span class="sxs-lookup"><span data-stu-id="e86c1-135">approvalType</span></span>|<span data-ttu-id="e86c1-136">String</span><span class="sxs-lookup"><span data-stu-id="e86c1-136">String</span></span>||
|<span data-ttu-id="e86c1-137">approverReason</span><span class="sxs-lookup"><span data-stu-id="e86c1-137">approverReason</span></span>|<span data-ttu-id="e86c1-138">String</span><span class="sxs-lookup"><span data-stu-id="e86c1-138">String</span></span>||
|<span data-ttu-id="e86c1-139">endDateTime</span><span class="sxs-lookup"><span data-stu-id="e86c1-139">endDateTime</span></span>|<span data-ttu-id="e86c1-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e86c1-140">DateTimeOffset</span></span>||
|<span data-ttu-id="e86c1-141">requestorReason</span><span class="sxs-lookup"><span data-stu-id="e86c1-141">requestorReason</span></span>|<span data-ttu-id="e86c1-142">String</span><span class="sxs-lookup"><span data-stu-id="e86c1-142">String</span></span>||
|<span data-ttu-id="e86c1-143">roleId</span><span class="sxs-lookup"><span data-stu-id="e86c1-143">roleId</span></span>|<span data-ttu-id="e86c1-144">String</span><span class="sxs-lookup"><span data-stu-id="e86c1-144">String</span></span>||
|<span data-ttu-id="e86c1-145">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e86c1-145">startDateTime</span></span>|<span data-ttu-id="e86c1-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e86c1-146">DateTimeOffset</span></span>||
|<span data-ttu-id="e86c1-147">userId</span><span class="sxs-lookup"><span data-stu-id="e86c1-147">userId</span></span>|<span data-ttu-id="e86c1-148">String</span><span class="sxs-lookup"><span data-stu-id="e86c1-148">String</span></span>||

## <a name="response"></a><span data-ttu-id="e86c1-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="e86c1-149">Response</span></span>

<span data-ttu-id="e86c1-150">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e86c1-150">If successful, this method returns a `204 No Content` response code</span></span>

<span data-ttu-id="e86c1-151">Beachten Sie, dass der Mandant muss auf den PIM registriert werden.</span><span class="sxs-lookup"><span data-stu-id="e86c1-151">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="e86c1-152">Andernfalls wird der Statuscode HTTP 403 Verboten zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="e86c1-152">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="e86c1-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e86c1-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e86c1-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e86c1-154">Request</span></span>
<span data-ttu-id="e86c1-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e86c1-155">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_privilegedapproval"
}-->
```http
PATCH https://graph.microsoft.com/beta/privilegedApproval{request-id}
Content-type: application/json
Content-length: 180

{
  "approvalState": "approvalState-value",
  "approverReason": "approverReason-value"
}
```
##### <a name="response"></a><span data-ttu-id="e86c1-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="e86c1-156">Response</span></span>
<span data-ttu-id="e86c1-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e86c1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update privilegedapproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedapproval-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
