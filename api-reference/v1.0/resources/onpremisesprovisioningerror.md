# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="3b42a-101">Ressourcentyp onPremisesProvisioningError</span><span class="sxs-lookup"><span data-stu-id="3b42a-101">onPremisesProvisioningError resource type</span></span>

<span data-ttu-id="3b42a-102">Repräsentiert Verzeichnissynchronisierungsfehler bei der Synchronisierung lokaler Verzeichnisse zum Azure Active Directory für die [Benutzer-](user.md) und [Gruppe](group.md)-Entitäten.</span><span class="sxs-lookup"><span data-stu-id="3b42a-102">Represents directory synchronization errors for the [user](user.md) and [group](group.md) entities when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="3b42a-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3b42a-103">Properties</span></span>

| <span data-ttu-id="3b42a-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3b42a-104">Property</span></span> | <span data-ttu-id="3b42a-105">Typ</span><span class="sxs-lookup"><span data-stu-id="3b42a-105">Type</span></span> | <span data-ttu-id="3b42a-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3b42a-106">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="3b42a-107">Kategorie</span><span class="sxs-lookup"><span data-stu-id="3b42a-107">category</span></span>|<span data-ttu-id="3b42a-108">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3b42a-108">String</span></span>| <span data-ttu-id="3b42a-109">Die Kategorie des Provisioning-Fehler.</span><span class="sxs-lookup"><span data-stu-id="3b42a-109">Category of the provisioning error.</span></span> <span data-ttu-id="3b42a-110">Hinweis: Zurzeit besteht nur ein möglicher Wert.</span><span class="sxs-lookup"><span data-stu-id="3b42a-110">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="3b42a-111">Möglicher Wert: *PropertyConflict* - gibt an, dass ein Eigenschaftswert nicht eindeutig ist.</span><span class="sxs-lookup"><span data-stu-id="3b42a-111">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="3b42a-112">Andere Objekte enthalten den gleichen Wert für die Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="3b42a-112">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="3b42a-113">occurredDateTime</span><span class="sxs-lookup"><span data-stu-id="3b42a-113">occurredDateTime</span></span>|<span data-ttu-id="3b42a-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b42a-114">DateTimeOffset</span></span>| <span data-ttu-id="3b42a-115">Das Datum und die Uhrzeit, an denen der Fehler aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="3b42a-115">The time at which the error occurred.</span></span> |
|<span data-ttu-id="3b42a-116">propertyCausingError</span><span class="sxs-lookup"><span data-stu-id="3b42a-116">propertyCausingError</span></span>|<span data-ttu-id="3b42a-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3b42a-117">String</span></span>| <span data-ttu-id="3b42a-118">Name der Verzeichniseigenschaft, die den Fehler verursacht.</span><span class="sxs-lookup"><span data-stu-id="3b42a-118">Name of the directory property causing the error.</span></span> <span data-ttu-id="3b42a-119">Aktuelle mögliche Werte: *UserPrincipalName* oder *ProxyAddress*</span><span class="sxs-lookup"><span data-stu-id="3b42a-119">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="3b42a-120">Wert</span><span class="sxs-lookup"><span data-stu-id="3b42a-120">value</span></span>|<span data-ttu-id="3b42a-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3b42a-121">String</span></span>| <span data-ttu-id="3b42a-122">Der Wert der Eigenschaft, die den Fehler verursacht.</span><span class="sxs-lookup"><span data-stu-id="3b42a-122">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3b42a-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3b42a-123">JSON representation</span></span>
<span data-ttu-id="3b42a-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3b42a-124">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesProvisioningError"
}-->

```json
{
  "category": "String",
  "occurredDateTime": "String (timestamp)",
  "propertyCausingError": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesProvisioningError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->