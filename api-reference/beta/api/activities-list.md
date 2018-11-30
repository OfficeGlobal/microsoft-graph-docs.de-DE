---
author: daspek
ms.author: dspektor
ms.date: 09/10/2017
title: Datei Aktivitäten
ms.openlocfilehash: f228f96083d899c4d9a43f6a4d41f2b90ce2eaf7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059344"
---
# <a name="enumerate-activities-preview"></a><span data-ttu-id="efa7c-102">Auflisten von Aktivitäten (Vorschau)</span><span class="sxs-lookup"><span data-stu-id="efa7c-102">Enumerate activities (preview)</span></span>

> <span data-ttu-id="efa7c-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="efa7c-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="efa7c-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="efa7c-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="efa7c-105">Listen Sie die letzten [Aktivitäten][] auf, die für ein Element oder unter einer Hierarchie stattgefunden haben.</span><span class="sxs-lookup"><span data-stu-id="efa7c-105">List the recent [activities][] that took place on an item or under a hierarchy.</span></span>

<span data-ttu-id="efa7c-106">**Hinweis:** Die Aktivitäten werden  in einer eingeschränkten Vorschau angezeigt und sind noch nicht für alle Mandanten verfügbar.</span><span class="sxs-lookup"><span data-stu-id="efa7c-106">**Note:** Activities is in a limited Preview and not yet available to all tenants.</span></span>

[activities]: ../resources/itemactivity.md

## <a name="permissions"></a><span data-ttu-id="efa7c-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="efa7c-108">Permissions</span></span>

<span data-ttu-id="efa7c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efa7c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efa7c-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="efa7c-111">Permission type</span></span>                        | <span data-ttu-id="efa7c-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="efa7c-112">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="efa7c-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="efa7c-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="efa7c-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efa7c-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="efa7c-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="efa7c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="efa7c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="efa7c-116">Not supported.</span></span>
|<span data-ttu-id="efa7c-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="efa7c-117">Application</span></span>                            | <span data-ttu-id="efa7c-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efa7c-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="efa7c-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="efa7c-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/activities
GET /drives/{drive-id}/items/{item-id}/activities
GET /sites/{site-id}/lists/{list-id}/activities
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/activities
```

## <a name="example"></a><span data-ttu-id="efa7c-120">Beispiel</span><span class="sxs-lookup"><span data-stu-id="efa7c-120">Example</span></span>

#### <a name="request"></a><span data-ttu-id="efa7c-121">Anforderung</span><span class="sxs-lookup"><span data-stu-id="efa7c-121">Request</span></span>

<!-- { "blockType": "request", "name": "list-activities" } -->

```http
GET https://graph.microsoft.com/beta/me/drive/activities
```

#### <a name="response"></a><span data-ttu-id="efa7c-122">Antwort</span><span class="sxs-lookup"><span data-stu-id="efa7c-122">Response</span></span>

<!-- { "blockType": "response", "@type": "Collection(microsoft.graph.itemActivity)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "action": {
                "comment": {}
            },
            "actor": {
                "user": {
                    "displayName": "Xavier Wilke"
                }
            },
            "id": "EJalEvjV1EgIYFQAAAAAAA==",
            "times": {
                "recordedTime": "2017-07-29T18:34:40Z"
            }
        },
        {
            "action": {
                "edit": {},
                "version": {
                    "newVersion": "2.0"
                }
            },
            "actor": {
                "user": {
                    "displayName": "Judith Clemons"
                }
            },
            "id": "cInT6/fV1EgFYFQAAAAAAA==",
            "times": {
                "recordedTime": "2017-07-29T16:23:35Z"
            }
        },
        {
            "action": {
                "mention": {
                    "mentionees": [
                        {
                            "user": {
                                "displayName": "Judith Clemons"
                            }
                        }
                    ]
                }
            },
            "actor": {
                "user": {
                    "displayName": "Misty Suarez"
                }
            },
            "id": "EBJa0vPV1EjFX1QAAAAAAA==",
            "times": {
                "recordedTime": "2017-07-28T20:14:14Z"
            }
        },
        {
            "action": {
                "rename": {
                    "oldName": "Document2.docx"
                }
            },
            "actor": {
                "user": {
                    "displayName": "Misty Suarez"
                }
            },
            "id": "QFJFlfPV1Ei/X1QAAAAAAA==",
            "times": {
                "recordedTime": "2017-07-28T20:12:32Z"
            }
        },
        {
            "action": {
                "create": {}
            },
            "actor": {
                "user": {
                    "displayName": "Misty Suarez"
                }
            },
            "id": "IJydkPPV1Ei9X1QAAAAAAA==",
            "times": {
                "recordedTime": "2017-07-28T20:02:24Z"
            }
        }
    ]
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Site/List sites"
} -->
