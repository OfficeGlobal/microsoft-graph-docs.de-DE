# <a name="internetmessageheader-resource-type"></a><span data-ttu-id="2d806-101">internetMessageHeader-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2d806-101">internetMessageHeader resource type</span></span>


<span data-ttu-id="2d806-102">Ein Schlüssel-Wert-Paar, das eine Internet-Nachrichtenkopfzeile darstellt, wie von [RFC5322](https://www.ietf.org/rfc/rfc5322.txt) definiert, die Informationen zum Netzwerkpfad einer Nachricht vom Absender bis zum Empfänger liefert.</span><span class="sxs-lookup"><span data-stu-id="2d806-102">A key-value pair that represents an Internet message header, as defined by [RFC5322](https://www.ietf.org/rfc/rfc5322.txt), that provides details of the network path taken by a message from the sender to the recipient.</span></span> 

<span data-ttu-id="2d806-103">Beispiele für eine Internet-Nachrichtenkopfzeile finden Sie unter [Anzeigen E-Mail-Kopfzeilen](https://support.office.com/de-DE/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4).</span><span class="sxs-lookup"><span data-stu-id="2d806-103">For examples of an Internet message header, see [View e-mail message headers](https://support.office.com/de-DE/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4).</span></span>


## <a name="properties"></a><span data-ttu-id="2d806-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2d806-104">Properties</span></span>
| <span data-ttu-id="2d806-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2d806-105">Property</span></span>     | <span data-ttu-id="2d806-106">Typ</span><span class="sxs-lookup"><span data-stu-id="2d806-106">Type</span></span>   |<span data-ttu-id="2d806-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2d806-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d806-108">name</span><span class="sxs-lookup"><span data-stu-id="2d806-108">name</span></span>|<span data-ttu-id="2d806-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2d806-109">string</span></span>|<span data-ttu-id="2d806-110">Stellt den Schlüssel in einem Schlüssel-Wert-Paar dar.</span><span class="sxs-lookup"><span data-stu-id="2d806-110">Represents the key in a key-value pair.</span></span>|
|<span data-ttu-id="2d806-111">Wert</span><span class="sxs-lookup"><span data-stu-id="2d806-111">value</span></span>|<span data-ttu-id="2d806-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2d806-112">string</span></span>|<span data-ttu-id="2d806-113">Der Wert in einem Schlüssel-Wert-Paar.</span><span class="sxs-lookup"><span data-stu-id="2d806-113">The value in a key-value pair.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2d806-114">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2d806-114">JSON representation</span></span>

<span data-ttu-id="2d806-115">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2d806-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.internetMessageHeader"
}-->

```json
{
  "name": "string",
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "internetMessageHeader resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->