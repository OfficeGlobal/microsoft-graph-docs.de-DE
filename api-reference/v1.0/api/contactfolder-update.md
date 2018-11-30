---
title: contactFolder aktualisieren
description: Mit dieser API können Sie die Eigenschaften von Objekten des Typs „contactfolder“ aktualisieren.
ms.openlocfilehash: 410dc0962278b63650637efb2ed67f7cf038b677
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018347"
---
# <a name="update-contactfolder"></a><span data-ttu-id="8b296-103">contactFolder aktualisieren</span><span class="sxs-lookup"><span data-stu-id="8b296-103">Update contactfolder</span></span>

<span data-ttu-id="8b296-104">Mit dieser API können Sie die Eigenschaften von Objekten des Typs „contactfolder“ aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="8b296-104">Update the properties of contactfolder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8b296-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8b296-105">Permissions</span></span>
<span data-ttu-id="8b296-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b296-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b296-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8b296-108">Permission type</span></span>      | <span data-ttu-id="8b296-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8b296-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b296-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8b296-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8b296-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b296-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="8b296-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8b296-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b296-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b296-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="8b296-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8b296-114">Application</span></span> | <span data-ttu-id="8b296-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b296-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b296-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8b296-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/contactFolders/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8b296-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8b296-117">Request headers</span></span>
| <span data-ttu-id="8b296-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8b296-118">Header</span></span>       | <span data-ttu-id="8b296-119">Wert</span><span class="sxs-lookup"><span data-stu-id="8b296-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8b296-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b296-120">Authorization</span></span>  | <span data-ttu-id="8b296-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8b296-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8b296-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8b296-123">Content-Type</span></span>  | <span data-ttu-id="8b296-p103">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="8b296-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8b296-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8b296-126">Request body</span></span>
<span data-ttu-id="8b296-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="8b296-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8b296-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8b296-130">Property</span></span>     | <span data-ttu-id="8b296-131">Typ</span><span class="sxs-lookup"><span data-stu-id="8b296-131">Type</span></span>   |<span data-ttu-id="8b296-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8b296-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8b296-133">displayName</span><span class="sxs-lookup"><span data-stu-id="8b296-133">displayName</span></span>|<span data-ttu-id="8b296-134">String</span><span class="sxs-lookup"><span data-stu-id="8b296-134">String</span></span>|<span data-ttu-id="8b296-135">Der Anzeigename des Ordners.</span><span class="sxs-lookup"><span data-stu-id="8b296-135">The folder's display name.</span></span>|
|<span data-ttu-id="8b296-136">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="8b296-136">parentFolderId</span></span>|<span data-ttu-id="8b296-137">String</span><span class="sxs-lookup"><span data-stu-id="8b296-137">String</span></span>|<span data-ttu-id="8b296-138">Die ID des übergeordneten Ordners des Ordners.</span><span class="sxs-lookup"><span data-stu-id="8b296-138">The ID of the folder's parent folder.</span></span>|

## <a name="response"></a><span data-ttu-id="8b296-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="8b296-139">Response</span></span>

<span data-ttu-id="8b296-140">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [contactFolder](../resources/contactfolder.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8b296-140">If successful, this method returns a `200 OK` response code and updated [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8b296-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8b296-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8b296-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8b296-142">Request</span></span>
<span data-ttu-id="8b296-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8b296-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_contactfolder"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/contactFolders/{id}
Content-type: application/json
Content-length: 84

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value"
}
```
##### <a name="response"></a><span data-ttu-id="8b296-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="8b296-144">Response</span></span>
<span data-ttu-id="8b296-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8b296-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 104

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update contactfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->