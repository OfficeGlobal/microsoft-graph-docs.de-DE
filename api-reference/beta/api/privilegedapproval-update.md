---
title: Privilegedapproval aktualisieren
description: Aktualisieren Sie die Eigenschaften des Privilegedapproval-Objekts.
localization_priority: Normal
ms.openlocfilehash: 0ddab7d7a628be8513c27114e1e4ec3d13477784
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866885"
---
# <a name="update-privilegedapproval"></a><span data-ttu-id="162f3-103">Privilegedapproval aktualisieren</span><span class="sxs-lookup"><span data-stu-id="162f3-103">Update privilegedapproval</span></span>

> <span data-ttu-id="162f3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="162f3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="162f3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="162f3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="162f3-106">Aktualisieren Sie die Eigenschaften des Privilegedapproval-Objekts.</span><span class="sxs-lookup"><span data-stu-id="162f3-106">Update the properties of privilegedapproval object.</span></span>
## <a name="permissions"></a><span data-ttu-id="162f3-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="162f3-107">Permissions</span></span>
<span data-ttu-id="162f3-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="162f3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="162f3-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="162f3-110">Permission type</span></span>      | <span data-ttu-id="162f3-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="162f3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="162f3-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="162f3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="162f3-113">PrivilegedAccess.ReadWrite.AzureAD Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="162f3-113">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="162f3-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="162f3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="162f3-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="162f3-115">Not supported.</span></span>    |
|<span data-ttu-id="162f3-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="162f3-116">Application</span></span> | <span data-ttu-id="162f3-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="162f3-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="162f3-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="162f3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedApproval/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="162f3-119">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="162f3-119">Optional request headers</span></span>
| <span data-ttu-id="162f3-120">Name</span><span class="sxs-lookup"><span data-stu-id="162f3-120">Name</span></span>       | <span data-ttu-id="162f3-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="162f3-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="162f3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="162f3-122">Authorization</span></span>  | <span data-ttu-id="162f3-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="162f3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="162f3-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="162f3-125">Request body</span></span>
<span data-ttu-id="162f3-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="162f3-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="162f3-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="162f3-129">Property</span></span>     | <span data-ttu-id="162f3-130">Typ</span><span class="sxs-lookup"><span data-stu-id="162f3-130">Type</span></span>   |<span data-ttu-id="162f3-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="162f3-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="162f3-132">approvalDuration</span><span class="sxs-lookup"><span data-stu-id="162f3-132">approvalDuration</span></span>|<span data-ttu-id="162f3-133">Duration</span><span class="sxs-lookup"><span data-stu-id="162f3-133">Duration</span></span>||
|<span data-ttu-id="162f3-134">approvalState</span><span class="sxs-lookup"><span data-stu-id="162f3-134">approvalState</span></span>|<span data-ttu-id="162f3-135">string</span><span class="sxs-lookup"><span data-stu-id="162f3-135">string</span></span>| <span data-ttu-id="162f3-136">Mögliche Werte sind: `pending`, `approved`, `denied`, `aborted` und `canceled`.</span><span class="sxs-lookup"><span data-stu-id="162f3-136">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="162f3-137">approvalType</span><span class="sxs-lookup"><span data-stu-id="162f3-137">approvalType</span></span>|<span data-ttu-id="162f3-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="162f3-138">String</span></span>||
|<span data-ttu-id="162f3-139">approverReason</span><span class="sxs-lookup"><span data-stu-id="162f3-139">approverReason</span></span>|<span data-ttu-id="162f3-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="162f3-140">String</span></span>||
|<span data-ttu-id="162f3-141">endDateTime</span><span class="sxs-lookup"><span data-stu-id="162f3-141">endDateTime</span></span>|<span data-ttu-id="162f3-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="162f3-142">DateTimeOffset</span></span>||
|<span data-ttu-id="162f3-143">requestorReason</span><span class="sxs-lookup"><span data-stu-id="162f3-143">requestorReason</span></span>|<span data-ttu-id="162f3-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="162f3-144">String</span></span>||
|<span data-ttu-id="162f3-145">roleId</span><span class="sxs-lookup"><span data-stu-id="162f3-145">roleId</span></span>|<span data-ttu-id="162f3-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="162f3-146">String</span></span>||
|<span data-ttu-id="162f3-147">startDateTime</span><span class="sxs-lookup"><span data-stu-id="162f3-147">startDateTime</span></span>|<span data-ttu-id="162f3-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="162f3-148">DateTimeOffset</span></span>||
|<span data-ttu-id="162f3-149">userId</span><span class="sxs-lookup"><span data-stu-id="162f3-149">userId</span></span>|<span data-ttu-id="162f3-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="162f3-150">String</span></span>||

## <a name="response"></a><span data-ttu-id="162f3-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="162f3-151">Response</span></span>

<span data-ttu-id="162f3-152">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `204 No Content` Antwortcode</span><span class="sxs-lookup"><span data-stu-id="162f3-152">If successful, this method returns a `204 No Content` response code</span></span>

<span data-ttu-id="162f3-153">Beachten Sie, dass der Mandant muss auf den PIM registriert werden.</span><span class="sxs-lookup"><span data-stu-id="162f3-153">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="162f3-154">Andernfalls wird der Statuscode HTTP 403 Verboten zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="162f3-154">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="162f3-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="162f3-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="162f3-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="162f3-156">Request</span></span>
<span data-ttu-id="162f3-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="162f3-157">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="162f3-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="162f3-158">Response</span></span>
<span data-ttu-id="162f3-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="162f3-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update privilegedapproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
