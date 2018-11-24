# <a name="localeinfo-resource-type"></a><span data-ttu-id="7f978-101">localeInfo-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7f978-101">localeInfo resource type</span></span>

<span data-ttu-id="7f978-102">Die Gebietsschemainformationen, einschließlich der bevorzugten Sprache und Land/Region, des angemeldeten Benutzers.</span><span class="sxs-lookup"><span data-stu-id="7f978-102">Information about the locale, including the preferred language and country/region, of the signed-in user.</span></span>


## <a name="properties"></a><span data-ttu-id="7f978-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7f978-103">Properties</span></span>
| <span data-ttu-id="7f978-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7f978-104">Property</span></span>     | <span data-ttu-id="7f978-105">Typ</span><span class="sxs-lookup"><span data-stu-id="7f978-105">Type</span></span>   |<span data-ttu-id="7f978-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7f978-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f978-107">Gebietsschema</span><span class="sxs-lookup"><span data-stu-id="7f978-107">locale</span></span>|<span data-ttu-id="7f978-108">string</span><span class="sxs-lookup"><span data-stu-id="7f978-108">string</span></span>|<span data-ttu-id="7f978-p101">Eine Gebietsschemadarstellung für den Benutzer, die die bevorzugte Sprache des Benutzers sowie Land/Region umfasst. Z. B. „de-de“. Die Sprachkomponente besteht entsprechend der Definitionen in [ISO 639-1](https://www.iso.org/iso/home/standards/language_codes.htm) aus 2 Buchstaben, und die Länderkomponente besteht entsprechend der Definitionen in [ISO 3166-1-Alpha-2](https://www.iso.org/iso/country_codes.htm) aus 2 Buchstaben.</span><span class="sxs-lookup"><span data-stu-id="7f978-p101">A locale representation for the user, which includes the user's preferred language and country/region. For example, "en-us". The language component follows 2-letter codes as defined in [ISO 639-1](https://www.iso.org/iso/home/standards/language_codes.htm), and the country component follows 2-letter codes as defined in [ISO 3166-1 alpha-2](https://www.iso.org/iso/country_codes.htm).</span></span>|
|<span data-ttu-id="7f978-112">displayName</span><span class="sxs-lookup"><span data-stu-id="7f978-112">displayName</span></span>|<span data-ttu-id="7f978-113">string</span><span class="sxs-lookup"><span data-stu-id="7f978-113">string</span></span>|<span data-ttu-id="7f978-114">Ein Name, der das Gebietsschema des Benutzers in natürlicher Sprache darstellt, z. B. „Englisch (USA)“.</span><span class="sxs-lookup"><span data-stu-id="7f978-114">A name representing the user's locale in natural language, for example, "English (United States)".</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7f978-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7f978-115">JSON representation</span></span>

<span data-ttu-id="7f978-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7f978-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.localeInfo"
}-->

```json
{
  "locale": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "localeInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->