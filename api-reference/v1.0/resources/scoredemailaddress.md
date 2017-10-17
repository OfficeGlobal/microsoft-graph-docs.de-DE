# <a name="scoredemailaddress-resource-type"></a><span data-ttu-id="61fc7-101">scoredEmailAddress-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="61fc7-101">scoredEmailAddress resource type</span></span>

<span data-ttu-id="61fc7-102">Gibt eine bewertete E-Mail-Adresse an.</span><span class="sxs-lookup"><span data-stu-id="61fc7-102">Represents a scored email address.</span></span>


## <a name="properties"></a><span data-ttu-id="61fc7-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="61fc7-103">Properties</span></span>
| <span data-ttu-id="61fc7-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="61fc7-104">Property</span></span>     | <span data-ttu-id="61fc7-105">Typ</span><span class="sxs-lookup"><span data-stu-id="61fc7-105">Type</span></span>   |<span data-ttu-id="61fc7-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="61fc7-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="61fc7-107">address</span><span class="sxs-lookup"><span data-stu-id="61fc7-107">address</span></span>|<span data-ttu-id="61fc7-108">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="61fc7-108">string</span></span>|<span data-ttu-id="61fc7-109">Die E-Mail-Adresse</span><span class="sxs-lookup"><span data-stu-id="61fc7-109">The email address.</span></span>|
|<span data-ttu-id="61fc7-110">relevanceScore</span><span class="sxs-lookup"><span data-stu-id="61fc7-110">relevanceScore</span></span>|<span data-ttu-id="61fc7-111">double</span><span class="sxs-lookup"><span data-stu-id="61fc7-111">double</span></span>|<span data-ttu-id="61fc7-p101">Die Relevanzbewertung der E-Mail-Adresse. Eine Relevanzbewertung dient als Sortierschlüssel, in Bezug auf andere zurückgegebene Ergebnisse. Ein höherer Relevanzwert entspricht einem relevanteren Ergebnis. Relevanz wird durch die Kommunikations- und Zusammenarbeitsmuster und Geschäftsbeziehungen des Benutzers bestimmt.</span><span class="sxs-lookup"><span data-stu-id="61fc7-p101">The relevance score of the email address. A relevance score is used as a sort key, in relation to the other returned results. A higher relevance score value corresponds to a more relevant result. Relevance is determined by the user’s communication and collaboration patterns and business relationships.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="61fc7-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="61fc7-116">JSON representation</span></span>

<span data-ttu-id="61fc7-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="61fc7-117">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scoredEmailAddress"
}-->

```json
{
  "address": "string",
  "relevanceScore": 1024.0
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "scoredEmailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
