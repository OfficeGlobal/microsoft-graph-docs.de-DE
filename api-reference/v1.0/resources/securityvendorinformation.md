# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="babc2-101">Ressourcentyp securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="babc2-101">securityVendorInformation resource type</span></span>

<span data-ttu-id="babc2-102">Enthält Details über die Produkt-Dienst Sicherheitsanbieter, Anbieter und Subprovider (beispielsweise Hersteller = Microsoft; Provider = Windows Defender ATP; SubProvider = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="babc2-102">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="babc2-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="babc2-103">Properties</span></span>

| <span data-ttu-id="babc2-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="babc2-104">Property</span></span>   | <span data-ttu-id="babc2-105">Typ</span><span class="sxs-lookup"><span data-stu-id="babc2-105">Type</span></span>|<span data-ttu-id="babc2-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="babc2-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="babc2-107">Anbieter</span><span class="sxs-lookup"><span data-stu-id="babc2-107">provider</span></span> |<span data-ttu-id="babc2-108">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="babc2-108">String</span></span>|<span data-ttu-id="babc2-109">Bestimmte Anbieter (Product/Service - nicht Hersteller Unternehmen); beispielsweise WindowsDefenderATP.</span><span class="sxs-lookup"><span data-stu-id="babc2-109">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="babc2-110">providerVersion</span><span class="sxs-lookup"><span data-stu-id="babc2-110">providerVersion</span></span>|<span data-ttu-id="babc2-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="babc2-111">String</span></span>|<span data-ttu-id="babc2-112">Version des Anbieters oder Subprovider, falls vorhanden, die Warnung ausgelöst wurde.</span><span class="sxs-lookup"><span data-stu-id="babc2-112">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="babc2-113">*Required*</span><span class="sxs-lookup"><span data-stu-id="babc2-113">*Required*</span></span>|
|<span data-ttu-id="babc2-114">subProvider</span><span class="sxs-lookup"><span data-stu-id="babc2-114">subProvider</span></span>|<span data-ttu-id="babc2-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="babc2-115">String</span></span>|<span data-ttu-id="babc2-116">Bestimmte Subprovider (unter aggregieren Anbieter); beispielsweise WindowsDefenderATP.SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="babc2-116">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="babc2-117">Hersteller</span><span class="sxs-lookup"><span data-stu-id="babc2-117">vendor</span></span> |<span data-ttu-id="babc2-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="babc2-118">String</span></span>|<span data-ttu-id="babc2-119">Name des Herstellers alert (beispielsweise Microsoft, Dell, FireEye).</span><span class="sxs-lookup"><span data-stu-id="babc2-119">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="babc2-120">*Required*</span><span class="sxs-lookup"><span data-stu-id="babc2-120">*Required*</span></span>|


## <a name="json-representation"></a><span data-ttu-id="babc2-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="babc2-121">JSON representation</span></span>

<span data-ttu-id="babc2-122">Die folgenden ist eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="babc2-122">The folllowing is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityVendorInformation"
}-->

```json
{
  "provider": "String",
  "providerVersion": "String",
  "subProvider": "String",
  "vendor": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityVendorInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
