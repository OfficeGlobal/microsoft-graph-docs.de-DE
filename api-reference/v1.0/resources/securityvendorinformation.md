# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="58e34-101">Ressourcentyp securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="58e34-101">securityVendorInformation resource type</span></span>

<span data-ttu-id="58e34-102">Enthält Angaben zum Sicherheitsprodukt/Dienstleister, Anbieter und Unteranbieter (bspw. vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span><span class="sxs-lookup"><span data-stu-id="58e34-102">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="58e34-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="58e34-103">Properties</span></span>

| <span data-ttu-id="58e34-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="58e34-104">Property</span></span>   | <span data-ttu-id="58e34-105">Typ</span><span class="sxs-lookup"><span data-stu-id="58e34-105">Type</span></span>|<span data-ttu-id="58e34-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="58e34-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="58e34-107">provider \*</span><span class="sxs-lookup"><span data-stu-id="58e34-107">provider \*</span></span>|<span data-ttu-id="58e34-108">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="58e34-108">String</span></span>|<span data-ttu-id="58e34-109">Bestimmter Anbieter (Produkt/Dienst - kein Herstellerunternehmen); beispielsweise WindowsDefenderATP.</span><span class="sxs-lookup"><span data-stu-id="58e34-109">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="58e34-110">providerVersion</span><span class="sxs-lookup"><span data-stu-id="58e34-110">providerVersion</span></span>|<span data-ttu-id="58e34-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="58e34-111">String</span></span>|<span data-ttu-id="58e34-112">Version des Anbieters oder Unteranbieters, falls vorhanden, die die Warnung ausgelöst hat.</span><span class="sxs-lookup"><span data-stu-id="58e34-112">Version of the provider or subprovider, if it exists, that generated the alert.</span></span>|
|<span data-ttu-id="58e34-113">subProvider</span><span class="sxs-lookup"><span data-stu-id="58e34-113">subProvider</span></span>|<span data-ttu-id="58e34-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="58e34-114">String</span></span>|<span data-ttu-id="58e34-115">Bestimmter Unteranbieter (unter einem aggregierten Anbieter); beispielsweise WindowsDefenderATP.SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="58e34-115">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="58e34-116">vendor \*</span><span class="sxs-lookup"><span data-stu-id="58e34-116">vendor \*</span></span>|<span data-ttu-id="58e34-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="58e34-117">String</span></span>|<span data-ttu-id="58e34-118">Name des Warnungs-Software-Herstellers (beispielsweise Microsoft, Dell, FireEye).</span><span class="sxs-lookup"><span data-stu-id="58e34-118">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span>|
<span data-ttu-id="58e34-119">(\* Kennzeichnet ein Pflichtfeld.)</span><span class="sxs-lookup"><span data-stu-id="58e34-119">(\* Indicates a mandatory field.)</span></span>

## <a name="json-representation"></a><span data-ttu-id="58e34-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="58e34-120">JSON representation</span></span>

<span data-ttu-id="58e34-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="58e34-121">The following is a JSON representation of the resource.</span></span>
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
