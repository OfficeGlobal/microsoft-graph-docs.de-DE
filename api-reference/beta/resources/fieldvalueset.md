---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: FieldValueSet
localization_priority: Normal
ms.openlocfilehash: ed10b586ee55ccd32e81b03bdc6359ee13605877
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480166"
---
# <a name="fieldvalueset-resource"></a><span data-ttu-id="3f606-102">FieldValueSet-Ressource</span><span class="sxs-lookup"><span data-stu-id="3f606-102">FieldValueSet resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f606-103">Stellt die Spaltenwerte in einer [ListItem](listitem.md)-Ressource dar.</span><span class="sxs-lookup"><span data-stu-id="3f606-103">Represents the column values in a [listItem](listitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f606-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3f606-104">JSON representation</span></span>

<span data-ttu-id="3f606-105">Es folgt eine JSON-Darstellung einer **fieldValueSet**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="3f606-105">Here is a JSON representation of a **fieldValueSet** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.fieldValueSet",
       "keyProperty": "id", "openType": true } -->

```json
{
    "Author": "Brad Cleaver",
    "AuthorLookupId": "13",
    "Name": "Kangaroos and Wallabies: A Deep Dive",
    "Color": "Red",
    "Quantity": 350,
}
```

## <a name="properties"></a><span data-ttu-id="3f606-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3f606-106">Properties</span></span>

<span data-ttu-id="3f606-107">Jedes für den Benutzer sichtbare Feld im **ListItem** wird als Name-Wert-Paar im **FieldValueSet** wiedergegeben.</span><span class="sxs-lookup"><span data-stu-id="3f606-107">Each user-visible field in the **listItem** is returned as a name-value pair in the **fieldValueSet**.</span></span>
<span data-ttu-id="3f606-108">Das Beispiel oben bezieht sich auf eine Liste mit den vier Spalten **Autor**, **Namen**, **Farbe** und **Menge**.</span><span class="sxs-lookup"><span data-stu-id="3f606-108">The example above is for a list that contains four columns, **Author**, **Name**, **Color**, and **Quantity**.</span></span>

<span data-ttu-id="3f606-109">Nachschlage-Feldern (wie `Author` oben) werden standardmäßig nicht zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3f606-109">Lookup fields (like `Author` above) are not returned by default.</span></span>
<span data-ttu-id="3f606-110">In diesem Fall gibt der Server ein Feld 'LookupId' (wie `AuthorLookupId` oben) zurück, das sich auf das in der Suche angegebene ListItem bezieht.</span><span class="sxs-lookup"><span data-stu-id="3f606-110">Instead, the server returns a 'LookupId' field (like `AuthorLookupId` above) referencing the listItem targeted in the lookup.</span></span>
<span data-ttu-id="3f606-111">Der Name des Felds 'LookupId' besteht aus dem ursprünglichen Feldnamen gefolgt von `LookupId`.</span><span class="sxs-lookup"><span data-stu-id="3f606-111">The name of the 'LookupId' field is the original field name followed by `LookupId`.</span></span>

<span data-ttu-id="3f606-112">Bis zu 12 Nachschlagetabellen in einer einzigen Abfrage angefordert werden.</span><span class="sxs-lookup"><span data-stu-id="3f606-112">Up to 12 lookup fields may be requested in a single query.</span></span>
<span data-ttu-id="3f606-113">Der Server gibt Nachschlagewerte zurück, wenn Ihre Anforderung eine `select`-Anweisung mit den von Ihnen benötigten Feldern enthält.</span><span class="sxs-lookup"><span data-stu-id="3f606-113">The server will return lookup values if your request includes a `select` statement with the fields you need.</span></span>
<span data-ttu-id="3f606-114">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="3f606-114">Example:</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Author,BookTitle,PageCount)
```

<span data-ttu-id="3f606-115">Sie können bis zu 12 Nachschlage-Felder in einer Abfrage sowie eine beliebige Anzahl regulärer Felder anfordern.</span><span class="sxs-lookup"><span data-stu-id="3f606-115">You may request up to 12 lookup fields in a single query, plus any number of regular fields.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/FieldValueSet",
  "suppressions": [
    "Error: /api-reference/beta/resources/fieldvalueset.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
