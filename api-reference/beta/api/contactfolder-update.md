---
title: contactFolder aktualisieren
description: Mit dieser API können Sie die Eigenschaften von Objekten des Typs „contactfolder“ aktualisieren.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 155a8fb17f0423e2a4718dde8fc9743d8c1f0342
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854761"
---
# <a name="update-contactfolder"></a><span data-ttu-id="306e9-103">contactFolder aktualisieren</span><span class="sxs-lookup"><span data-stu-id="306e9-103">Update contactfolder</span></span>

> <span data-ttu-id="306e9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="306e9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="306e9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="306e9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="306e9-106">Mit dieser API können Sie die Eigenschaften von Objekten des Typs „contactfolder“ aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="306e9-106">Update the properties of contactfolder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="306e9-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="306e9-107">Permissions</span></span>
<span data-ttu-id="306e9-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="306e9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="306e9-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="306e9-110">Permission type</span></span>      | <span data-ttu-id="306e9-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="306e9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="306e9-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="306e9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="306e9-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="306e9-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="306e9-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="306e9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="306e9-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="306e9-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="306e9-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="306e9-116">Application</span></span> | <span data-ttu-id="306e9-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="306e9-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="306e9-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="306e9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/contactFolders/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="306e9-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="306e9-119">Request headers</span></span>
| <span data-ttu-id="306e9-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="306e9-120">Header</span></span>       | <span data-ttu-id="306e9-121">Wert</span><span class="sxs-lookup"><span data-stu-id="306e9-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="306e9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="306e9-122">Authorization</span></span>  | <span data-ttu-id="306e9-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="306e9-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="306e9-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="306e9-125">Content-Type</span></span>  | <span data-ttu-id="306e9-p104">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="306e9-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="306e9-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="306e9-128">Request body</span></span>
<span data-ttu-id="306e9-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="306e9-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="306e9-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="306e9-132">Property</span></span>     | <span data-ttu-id="306e9-133">Typ</span><span class="sxs-lookup"><span data-stu-id="306e9-133">Type</span></span>   |<span data-ttu-id="306e9-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="306e9-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="306e9-135">displayName</span><span class="sxs-lookup"><span data-stu-id="306e9-135">displayName</span></span>|<span data-ttu-id="306e9-136">String</span><span class="sxs-lookup"><span data-stu-id="306e9-136">String</span></span>|<span data-ttu-id="306e9-137">Der Anzeigename des Ordners.</span><span class="sxs-lookup"><span data-stu-id="306e9-137">The folder's display name.</span></span>|
|<span data-ttu-id="306e9-138">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="306e9-138">parentFolderId</span></span>|<span data-ttu-id="306e9-139">String</span><span class="sxs-lookup"><span data-stu-id="306e9-139">String</span></span>|<span data-ttu-id="306e9-140">Die ID des übergeordneten Ordners des Ordners.</span><span class="sxs-lookup"><span data-stu-id="306e9-140">The ID of the folder's parent folder.</span></span>|
|<span data-ttu-id="306e9-141">wellKnownName</span><span class="sxs-lookup"><span data-stu-id="306e9-141">wellKnownName</span></span>|<span data-ttu-id="306e9-142">string</span><span class="sxs-lookup"><span data-stu-id="306e9-142">string</span></span>|<span data-ttu-id="306e9-143">Der Name des Ordners, wenn der Ordner einen erkannten Ordner ist.</span><span class="sxs-lookup"><span data-stu-id="306e9-143">The name of the folder if the folder is a recognized folder.</span></span> <span data-ttu-id="306e9-144">Derzeit `contacts` ist die einzige erkannten Kontakteordner.</span><span class="sxs-lookup"><span data-stu-id="306e9-144">Currently `contacts` is the only recognized contacts folder.</span></span>|

## <a name="response"></a><span data-ttu-id="306e9-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="306e9-145">Response</span></span>

<span data-ttu-id="306e9-146">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [contactFolder](../resources/contactfolder.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="306e9-146">If successful, this method returns a `200 OK` response code and updated [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="306e9-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="306e9-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="306e9-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="306e9-148">Request</span></span>
<span data-ttu-id="306e9-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="306e9-149">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="306e9-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="306e9-150">Response</span></span>
<span data-ttu-id="306e9-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="306e9-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
