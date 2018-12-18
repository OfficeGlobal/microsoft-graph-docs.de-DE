---
title: 'Benutzer: ExportPersonalData'
description: Fordert die Daten Richtlinie Vorgang, versucht ein Unternehmensadministrator, eine Organisationseinheit Benutzerdaten exportieren.
ms.openlocfilehash: 27a299a4cfa6ccc3016a1f706b452840aa5dc396
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329125"
---
# <a name="user-exportpersonaldata"></a><span data-ttu-id="78287-103">Benutzer: ExportPersonalData</span><span class="sxs-lookup"><span data-stu-id="78287-103">user: exportPersonalData</span></span>

<span data-ttu-id="78287-104">Fordert die Daten Richtlinie Vorgang, versucht ein Unternehmensadministrator, eine Organisationseinheit Benutzerdaten exportieren.</span><span class="sxs-lookup"><span data-stu-id="78287-104">Submits a data policy operation request, made by a Company Administrator to export an organizational user's data.</span></span>

## <a name="permissions"></a><span data-ttu-id="78287-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="78287-105">Permissions</span></span>
<span data-ttu-id="78287-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78287-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78287-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="78287-108">Permission type</span></span>      | <span data-ttu-id="78287-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="78287-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="78287-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="78287-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="78287-111">User.Export.All und User.Read.All</span><span class="sxs-lookup"><span data-stu-id="78287-111">User.Export.All and User.Read.All</span></span>  |
|<span data-ttu-id="78287-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="78287-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="78287-113">Nicht zutreffend</span><span class="sxs-lookup"><span data-stu-id="78287-113">Not applicable</span></span>  |
|<span data-ttu-id="78287-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="78287-114">Application</span></span> | <span data-ttu-id="78287-115">User.Export.All und User.Read.All</span><span class="sxs-lookup"><span data-stu-id="78287-115">User.Export.All and User.Read.All</span></span> |

><span data-ttu-id="78287-116">Hinweis: Export kann nur ein Unternehmensadministrator erfolgen bei Verwendung die delegierte Berechtigung.</span><span class="sxs-lookup"><span data-stu-id="78287-116">Note: Export can only be performed by a Company Administrator when using the delegated permission.</span></span>

## <a name="http-request"></a><span data-ttu-id="78287-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="78287-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/<id>/exportPersonalData

```
## <a name="request-headers"></a><span data-ttu-id="78287-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="78287-118">Request headers</span></span>
| <span data-ttu-id="78287-119">Name</span><span class="sxs-lookup"><span data-stu-id="78287-119">Name</span></span>       | <span data-ttu-id="78287-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="78287-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="78287-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="78287-121">Authorization</span></span>  | <span data-ttu-id="78287-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="78287-122">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="78287-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="78287-123">Request body</span></span>
<span data-ttu-id="78287-124">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="78287-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="78287-125">Parameter</span><span class="sxs-lookup"><span data-stu-id="78287-125">Parameter</span></span>    | <span data-ttu-id="78287-126">Typ</span><span class="sxs-lookup"><span data-stu-id="78287-126">Type</span></span>   |<span data-ttu-id="78287-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="78287-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="78287-128">storageLocation</span><span class="sxs-lookup"><span data-stu-id="78287-128">storageLocation</span></span>|<span data-ttu-id="78287-129">String</span><span class="sxs-lookup"><span data-stu-id="78287-129">String</span></span>|<span data-ttu-id="78287-130">Dies ist die URL einer gemeinsamen Zugriff Signatur (SAS) ein Konto Azure-Speicher an, in dem Daten exportiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="78287-130">This is a shared access signature (SAS) URL to an Azure Storage account, to where data should be exported.</span></span>|

## <a name="response"></a><span data-ttu-id="78287-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="78287-131">Response</span></span>
<span data-ttu-id="78287-p102">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200, OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="78287-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78287-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="78287-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="78287-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="78287-135">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "user_exportpersonaldata"
}-->
```http
POST https://graph.microsoft.com/beta/users/{id}/exportPersonalData
Content-type: application/json
Content-length: 48

{
  "storageLocation": "storageLocation-value"
}
```

##### <a name="response"></a><span data-ttu-id="78287-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="78287-136">Response</span></span>
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
  "description": "user: exportPersonalData",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
