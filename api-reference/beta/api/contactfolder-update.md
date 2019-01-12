---
title: contactFolder aktualisieren
description: Mit dieser API können Sie die Eigenschaften von Objekten des Typs „contactfolder“ aktualisieren.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 9b2244f17bf877c1f52ae5de812f65ba1eae3b98
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956150"
---
# <a name="update-contactfolder"></a><span data-ttu-id="92c12-103">contactFolder aktualisieren</span><span class="sxs-lookup"><span data-stu-id="92c12-103">Update contactfolder</span></span>

> <span data-ttu-id="92c12-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="92c12-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="92c12-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="92c12-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="92c12-106">Mit dieser API können Sie die Eigenschaften von Objekten des Typs „contactfolder“ aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="92c12-106">Update the properties of contactfolder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="92c12-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="92c12-107">Permissions</span></span>
<span data-ttu-id="92c12-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92c12-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92c12-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="92c12-110">Permission type</span></span>      | <span data-ttu-id="92c12-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="92c12-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="92c12-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="92c12-112">Delegated (work or school account)</span></span> | <span data-ttu-id="92c12-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="92c12-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="92c12-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="92c12-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92c12-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="92c12-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="92c12-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="92c12-116">Application</span></span> | <span data-ttu-id="92c12-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="92c12-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="92c12-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="92c12-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/contactFolders/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="92c12-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="92c12-119">Request headers</span></span>
| <span data-ttu-id="92c12-120">Header</span><span class="sxs-lookup"><span data-stu-id="92c12-120">Header</span></span>       | <span data-ttu-id="92c12-121">Wert</span><span class="sxs-lookup"><span data-stu-id="92c12-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="92c12-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="92c12-122">Authorization</span></span>  | <span data-ttu-id="92c12-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="92c12-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="92c12-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="92c12-125">Content-Type</span></span>  | <span data-ttu-id="92c12-p104">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="92c12-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="92c12-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="92c12-128">Request body</span></span>
<span data-ttu-id="92c12-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="92c12-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="92c12-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="92c12-132">Property</span></span>     | <span data-ttu-id="92c12-133">Typ</span><span class="sxs-lookup"><span data-stu-id="92c12-133">Type</span></span>   |<span data-ttu-id="92c12-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="92c12-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="92c12-135">displayName</span><span class="sxs-lookup"><span data-stu-id="92c12-135">displayName</span></span>|<span data-ttu-id="92c12-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="92c12-136">String</span></span>|<span data-ttu-id="92c12-137">Der Anzeigename des Ordners.</span><span class="sxs-lookup"><span data-stu-id="92c12-137">The folder's display name.</span></span>|
|<span data-ttu-id="92c12-138">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="92c12-138">parentFolderId</span></span>|<span data-ttu-id="92c12-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="92c12-139">String</span></span>|<span data-ttu-id="92c12-140">Die ID des übergeordneten Ordners des Ordners.</span><span class="sxs-lookup"><span data-stu-id="92c12-140">The ID of the folder's parent folder.</span></span>|
|<span data-ttu-id="92c12-141">wellKnownName</span><span class="sxs-lookup"><span data-stu-id="92c12-141">wellKnownName</span></span>|<span data-ttu-id="92c12-142">string</span><span class="sxs-lookup"><span data-stu-id="92c12-142">string</span></span>|<span data-ttu-id="92c12-143">Der Name des Ordners, wenn der Ordner einen erkannten Ordner ist.</span><span class="sxs-lookup"><span data-stu-id="92c12-143">The name of the folder if the folder is a recognized folder.</span></span> <span data-ttu-id="92c12-144">Derzeit `contacts` ist die einzige erkannten Kontakteordner.</span><span class="sxs-lookup"><span data-stu-id="92c12-144">Currently `contacts` is the only recognized contacts folder.</span></span>|

## <a name="response"></a><span data-ttu-id="92c12-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="92c12-145">Response</span></span>

<span data-ttu-id="92c12-146">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [contactFolder](../resources/contactfolder.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="92c12-146">If successful, this method returns a `200 OK` response code and updated [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="92c12-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="92c12-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="92c12-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="92c12-148">Request</span></span>
<span data-ttu-id="92c12-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="92c12-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_contactfolder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/contactFolders/{id}
Content-type: application/json
Content-length: 84

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value"
}
```
##### <a name="response"></a><span data-ttu-id="92c12-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="92c12-150">Response</span></span>
<span data-ttu-id="92c12-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="92c12-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "wellKnownName": "wellKnownName-value",
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
