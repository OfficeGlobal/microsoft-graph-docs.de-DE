---
author: rahmit
ms.author: rahmit
ms.date: 05/07/2018
title: Erstellen einer neuen Seite in einer SharePoint-Website
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: be3f24f3d4795c473562ddc01d75d54117dcedd3
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572787"
---
# <a name="create-a-page-in-the-site-pages-list-of-a-site"></a><span data-ttu-id="ba259-102">Erstellen Sie eine Seite in der Liste der Website-Seiten einer Website</span><span class="sxs-lookup"><span data-stu-id="ba259-102">Create a page in the site pages list of a site</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba259-103">Erstellen Sie eine neue [SitePage][] in der Website-Seiten- [Liste][] in einer [Website][].</span><span class="sxs-lookup"><span data-stu-id="ba259-103">Create a new [sitePage][] in the site pages [list][] in a [site][].</span></span>

## <a name="permissions"></a><span data-ttu-id="ba259-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ba259-104">Permissions</span></span>

<span data-ttu-id="ba259-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba259-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba259-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ba259-107">Permission type</span></span>      | <span data-ttu-id="ba259-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ba259-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba259-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ba259-109">Delegated (work or school account)</span></span> | <span data-ttu-id="ba259-110">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba259-110">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ba259-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ba259-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba259-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ba259-112">Not supported.</span></span>    |
|<span data-ttu-id="ba259-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ba259-113">Application</span></span> | <span data-ttu-id="ba259-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba259-114">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba259-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ba259-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/pages
```

## <a name="request-body"></a><span data-ttu-id="ba259-116">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ba259-116">Request body</span></span>

<span data-ttu-id="ba259-117">Geben Sie im Textkörper Anforderung eine JSON-Darstellung der [SitePage][] Ressource zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="ba259-117">In the request body, supply a JSON representation of the [sitePage][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="ba259-118">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ba259-118">Example</span></span>

<span data-ttu-id="ba259-119">Im folgenden Beispiel wird gezeigt, wie eine neue Seite zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="ba259-119">The following example shows how to create a new page.</span></span>

<!-- { "blockType": "request", "name": "create-page", "scopes": "sites.readwrite.all" } -->

```json
POST /sites/{site-id}/page
Content-Type: application/json

{
    "name": "Events.aspx",
    "title": "Team Events",
    "publishingState": {
        "level": "checkedOut",
        "versionId": "0.1"
    },
    "webParts": [
        {
            "type": "rte",
            "innerHTML": "<p>Here are the team's upcoming events:</p>"
        },
        {
            "type": "d1d91016-032f-456d-98a4-721247c305e8",
            "data": {
                "title": "Events",
                "description": "Display upcoming events",
                "serverProcessedContent": {
                    "htmlStrings": {},
                    "searchablePlainTexts": {
                        "title": ""
                    },
                    "imageSources": {},
                    "links": {
                        "baseUrl": "https://www.contoso.com/sites/Engineering"
                    },
                    "componentDependencies": {
                        "layoutComponentId": "8ac0c53c-e8d0-4e3e-87d0-7449eb0d4027"
                    }
                },
                "dataVersion": "1.0",
                "properties": {
                    "selectedListId": "032e08ab-89b0-4d8f-bc10-73094233615c",
                    "selectedCategory": "",
                    "dateRangeOption": 0,
                    "startDate": "",
                    "endDate": "",
                    "isOnSeeAllPage": false,
                    "layoutId": "FilmStrip",
                    "dataProviderId": "Event",
                    "webId": "0764c419-1ecc-4126-ba32-0c25ae0fffe8",
                    "siteId": "6b4ffc7a-cfc2-4a76-903a-1cc3686dee23"
                }
            }
        }
    ]
}
```

## <a name="response"></a><span data-ttu-id="ba259-120">Antwort</span><span class="sxs-lookup"><span data-stu-id="ba259-120">Response</span></span>

<span data-ttu-id="ba259-121">Wenn erfolgreich, gibt diese Methode eine [SitePage][] im Antworttext für die Seite erstellt.</span><span class="sxs-lookup"><span data-stu-id="ba259-121">If successful, this method returns a [sitePage][] in the response body for the created page.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.sitePage", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "2",
    "eTag": "75bc70e2-6587-45be-8493-c99a956b2e05,7",
    "createdDateTime": "2016-12-06T20:04:40Z",
    "lastModifiedDateTime": "2016-12-06T20:05:09Z",
    "webUrl": "https://www.contoso.com/sites/Engineering/SitePages/Events.aspx",
    "createdBy": {
        "user": {
            "email": "rahmit",
            "id": "1b37d2e1-5000-4648-b431-7dfa509b5660",
            "displayName": "Rahul Mittal"
        }
    },
    "lastModifiedBy": {
        "user": {
            "email": "rahmit",
            "id": "1b37d2e1-5000-4648-b431-7dfa509b5660",
            "displayName": "Rahul Mittal"
        }
    },
    "parentReference": {
        "id": "eb3bfd48-56f8-4c1e-8312-e58588b22e7c"
    },
    "contentType": {
        "id": "0x0101009D1CB255DA76424F860D91F20E6C411800C9E7033636784C4B88A284B1823C45FD",
        "name": "Site Page"
    },
    "description": "",
    "title": "Team Events",
    "webParts": [
        {
            "type": "rte",
            "data": {
                "innerHTML": "<p>Here are the team's upcoming events:</p>"
            }
        },
        {
            "type": "d1d91016-032f-456d-98a4-721247c305e8",
            "data": {
                "title": "Events",
                "description": "Display upcoming events",
                "serverProcessedContent": {
                    "htmlStrings": {},
                    "searchablePlainTexts": {
                        "title": ""
                    },
                    "imageSources": {},
                    "links": {
                        "baseUrl": "https://www.contoso.com/teams/Engineering"
                    },
                    "componentDependencies": {
                        "layoutComponentId": "8ac0c53c-e8d0-4e3e-87d0-7449eb0d4027"
                    }
                },
                "dataVersion": "1.0",
                "properties": {
                    "selectedListId": "032e08ab-89b0-4d8f-bc10-73094233615c",
                    "selectedCategory": "",
                    "dateRangeOption": 0,
                    "startDate": "",
                    "endDate": "",
                    "isOnSeeAllPage": false,
                    "layoutId": "FilmStrip",
                    "dataProviderId": "Event",
                    "webId": "0764c419-1ecc-4126-ba32-0c25ae0fffe8",
                    "siteId": "6b4ffc7a-cfc2-4a76-903a-1cc3686dee23"
                }
            }
        }
    ]
}
```

<span data-ttu-id="ba259-122">**Hinweis:** Das „Response“-Objekt wurde zwecks besserer Übersichtlichkeit gekürzt.</span><span class="sxs-lookup"><span data-stu-id="ba259-122">**Note:** The response object is truncated for clarity.</span></span> <span data-ttu-id="ba259-123">Der tatsächliche Aufruf gibt die Standardeigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="ba259-123">Default properties will be returned from the actual call.</span></span>

[list]: ../resources/list.md
[listItem]: ../resources/listitem.md
[site]: ../resources/site.md
[sitePage]: ../resources/sitepage.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a sitePage in the SitePages list in a site.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Pages/Create",
  "suppressions": [
    "Error: /api-reference/beta/api/sitepage-create.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
