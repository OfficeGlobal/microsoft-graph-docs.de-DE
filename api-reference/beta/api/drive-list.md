---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Laufwerke auflisten
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5c85533a2c335158d953749ae329cc6cd2b7ec37
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966230"
---
# <a name="list-available-drives"></a><span data-ttu-id="9ef40-102">Verfügbare Laufwerke auflisten</span><span class="sxs-lookup"><span data-stu-id="9ef40-102">List available drives</span></span>

> <span data-ttu-id="9ef40-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9ef40-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9ef40-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9ef40-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9ef40-105">Rufen Sie die Liste der [Laufwerk](../resources/drive.md)-Ressourcen ab, die für einen Ziel-Benutzer, eine Ziel-Gruppe oder eine Ziel-[Seite](../resources/site.md) verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="9ef40-105">Retrieve the list of [Drive](../resources/drive.md) resources available for a target User, Group, or [Site](../resources/site.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9ef40-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9ef40-106">Permissions</span></span>

<span data-ttu-id="9ef40-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ef40-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ef40-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9ef40-109">Permission type</span></span>      | <span data-ttu-id="9ef40-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9ef40-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ef40-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9ef40-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9ef40-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef40-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="9ef40-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9ef40-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ef40-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef40-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="9ef40-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9ef40-115">Application</span></span> | <span data-ttu-id="9ef40-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef40-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="list-a-groups-drives"></a><span data-ttu-id="9ef40-117">Auflisten des Laufwerks einer Gruppe</span><span class="sxs-lookup"><span data-stu-id="9ef40-117">List a group's drives</span></span>

<span data-ttu-id="9ef40-118">Für die Auflistung der Dokumentbibliotheken einer Gruppe fordert Ihre App die **drives**-Beziehung bei der Gruppe an.</span><span class="sxs-lookup"><span data-stu-id="9ef40-118">To list the document libraries for a group, your app requests the **drives** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="9ef40-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9ef40-119">HTTP request</span></span>

<!-- {"blockType": "request", "name": "group-list-drives", "scopes": "groups.read.all" } -->

```http
GET /groups/{groupId}/drives
```

## <a name="list-a-sites-drives"></a><span data-ttu-id="9ef40-120">Auflisten der Laufwerke einer Website</span><span class="sxs-lookup"><span data-stu-id="9ef40-120">List a site's drives</span></span>

<span data-ttu-id="9ef40-121">Für die Auflistung der Dokumentbibliotheken einer Website fordert Ihre App die **drives**-Beziehung bei der Website an.</span><span class="sxs-lookup"><span data-stu-id="9ef40-121">To list the document libraries for a site, your app requests the **drives** relationship on the Site.</span></span>

<!-- {"blockType": "request", "name": "site-list-drives", "scopes": "sites.read.all" } -->

```http
GET /sites/{siteId}/drives
```

## <a name="list-a-users-drives"></a><span data-ttu-id="9ef40-122">Auflisten der Laufwerke eines Benutzers</span><span class="sxs-lookup"><span data-stu-id="9ef40-122">List a user's drives</span></span>

<!-- {"blockType": "request", "name": "user-list-drives", "scopes": "files.read.all" } -->

```http
GET /users/{userId}/drives
```

## <a name="list-the-current-users-drives"></a><span data-ttu-id="9ef40-123">Die Laufwerke des aktuellen Benutzers auflisten</span><span class="sxs-lookup"><span data-stu-id="9ef40-123">List the current user's drives</span></span>

<!-- {"blockType": "request", "name": "enum-drives", "scopes": "files.read" } -->

```http
GET /me/drives
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9ef40-124">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9ef40-124">Optional query parameters</span></span>

<span data-ttu-id="9ef40-125">Diese Methode unterstützt die `$expand`, `$select`, `$skipToken`, `$top` und `$orderby` [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9ef40-125">This method supports the `$expand`, `$select`, `$skipToken`, `$top`, and `$orderby` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="9ef40-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="9ef40-126">Response</span></span>

<span data-ttu-id="9ef40-127">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Drive](../resources/drive.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9ef40-127">If successful, this method returns a `200 OK` response code and collection of [Drive](../resources/drive.md) objects in the response body.</span></span>

<!-- { "blockType": "response", 
       "@odata.type": "Collection(microsoft.graph.drive)",
       "name": ["group-list-drives", "site-list-drives", "user-list-drives", "enum-drives"],
       "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "942CAEB0-13AE-491B-85E4-7557CDC0F25F",
      "driveType": "documentLibrary",
      "name": "Shared Documents",
      "owner": {
        "user": {
          "id": "AE2A1EE9-81A7-423C-ABE4-B945F47509BB",
          "displayName": "Ryan Gregg"
        }
      }
    },
    {
      "id": "C1CD3ED9-0E98-4B0B-82D3-C8FB784B9DCC",
      "driveType": "documentLibrary",
      "name": "Contoso Project Files",
      "owner": {
        "user": {
          "id": "406B2281-18E8-4416-9857-38C531B904F1",
          "displayName": "Daron Spektor"
        }
      }
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="9ef40-128">Hinweise</span><span class="sxs-lookup"><span data-stu-id="9ef40-128">Remarks</span></span>

<span data-ttu-id="9ef40-129">Die meisten Benutzer verfügen nur über eine einzige Laufwerkressource.</span><span class="sxs-lookup"><span data-stu-id="9ef40-129">Most users will only have a single Drive resource.</span></span>

<span data-ttu-id="9ef40-130">Gruppen und Webseiten verfügen möglicherweise über mehrere Laufwerksressourcen.</span><span class="sxs-lookup"><span data-stu-id="9ef40-130">Groups and Sites may have multiple Drive resources available.</span></span>

<span data-ttu-id="9ef40-131">Laufwerke mit dem [System][]-Facet sind standardmäßig ausgeblendet.</span><span class="sxs-lookup"><span data-stu-id="9ef40-131">Drives with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="9ef40-132">Fügen Sie `system` in Ihre `$select`-Anweisung ein, um sie aufzulisten.</span><span class="sxs-lookup"><span data-stu-id="9ef40-132">To list them, include `system` in your `$select` statement.</span></span>

[System]: ../resources/systemfacet.md
[system]: ../resources/systemfacet.md

<!-- {
  "type": "#page.annotation",
  "description": "List the available drives for a user, group, or site.",
  "keywords": "drive,onedrive.drive,list drives",
  "section": "documentation",
  "tocPath": "Drives/List drives"
} -->
