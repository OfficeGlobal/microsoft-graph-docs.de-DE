# <a name="cloudappsecuritystate-resource-type"></a><span data-ttu-id="20ae0-101">Ressourcentyp cloudAppSecurityState</span><span class="sxs-lookup"><span data-stu-id="20ae0-101">cloudAppSecurityState resource type</span></span>

<span data-ttu-id="20ae0-102">Enthält Zustandsinformationen über die Cloud-Anwendung (destinationServiceName, destinationServiceIp).</span><span class="sxs-lookup"><span data-stu-id="20ae0-102">Contains stateful information about the cloud application (destinationServiceName, destinationServiceIp).</span></span>

## <a name="properties"></a><span data-ttu-id="20ae0-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="20ae0-103">Properties</span></span>

| <span data-ttu-id="20ae0-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="20ae0-104">Property</span></span>     | <span data-ttu-id="20ae0-105">Typ</span><span class="sxs-lookup"><span data-stu-id="20ae0-105">Type</span></span>        | <span data-ttu-id="20ae0-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="20ae0-106">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="20ae0-107">destinationServiceIp</span><span class="sxs-lookup"><span data-stu-id="20ae0-107">destinationServiceIp</span></span>|<span data-ttu-id="20ae0-108">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="20ae0-108">String</span></span>|<span data-ttu-id="20ae0-109">Ziel-IP-Adresse der Verbindung mit der Cloud-Anwendung/dem Dienst.</span><span class="sxs-lookup"><span data-stu-id="20ae0-109">Destination IP Address of the connection to the cloud application/service.</span></span>|
|<span data-ttu-id="20ae0-110">destinationServiceName</span><span class="sxs-lookup"><span data-stu-id="20ae0-110">destinationServiceName</span></span>|<span data-ttu-id="20ae0-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="20ae0-111">String</span></span>|<span data-ttu-id="20ae0-112">Name der Cloud-Anwendung/des Dienstes (zum Beispiel "Salesforce", "DropBox" usw.).</span><span class="sxs-lookup"><span data-stu-id="20ae0-112">Cloud application/service name (for example "Salesforce", "DropBox", etc.).</span></span>|
|<span data-ttu-id="20ae0-113">riskScore</span><span class="sxs-lookup"><span data-stu-id="20ae0-113">riskScore</span></span>|<span data-ttu-id="20ae0-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="20ae0-114">String</span></span>|<span data-ttu-id="20ae0-115">Vom Anbieter generierte/berechnete Risikobewertung der Cloud-Anwendung/des Dienstes.</span><span class="sxs-lookup"><span data-stu-id="20ae0-115">Provider-generated/calculated risk score of the Cloud Application/Service.</span></span> <span data-ttu-id="20ae0-116">Empfohlener Wertebereich von 0-1, was einem Prozentsatz entspricht.</span><span class="sxs-lookup"><span data-stu-id="20ae0-116">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="20ae0-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="20ae0-117">JSON representation</span></span>

<span data-ttu-id="20ae0-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="20ae0-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.cloudAppSecurityState"
}-->

```json
{
  "destinationServiceIp": "String",
  "destinationServiceName": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "cloudAppSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->