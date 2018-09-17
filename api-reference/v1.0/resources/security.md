# <a name="security-resource-type"></a><span data-ttu-id="41b3f-101">Ressourcentyp security</span><span class="sxs-lookup"><span data-stu-id="41b3f-101">security resource type</span></span>

<span data-ttu-id="41b3f-102">Die Sicherheitsressource ist der Einstiegspunkt für das Objektmodell Sicherheit.</span><span class="sxs-lookup"><span data-stu-id="41b3f-102">The security resource is the entry point for the Security object model.</span></span> <span data-ttu-id="41b3f-103">Es gibt eine Singleton Sicherheitsressource zurück.</span><span class="sxs-lookup"><span data-stu-id="41b3f-103">It returns a singleton security resource.</span></span> <span data-ttu-id="41b3f-104">Es enthält keine verwendbaren Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="41b3f-104">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="41b3f-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="41b3f-105">Methods</span></span>

| <span data-ttu-id="41b3f-106">Methode</span><span class="sxs-lookup"><span data-stu-id="41b3f-106">Method</span></span>       | <span data-ttu-id="41b3f-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="41b3f-107">Return Type</span></span> | <span data-ttu-id="41b3f-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="41b3f-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="41b3f-109">Warnungen auflisten</span><span class="sxs-lookup"><span data-stu-id="41b3f-109">List alerts</span></span>](../api/alert_list.md) | <span data-ttu-id="41b3f-110">[alert](alert.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="41b3f-110">[alert](alert.md) collection</span></span> | <span data-ttu-id="41b3f-111">Abruf einer Warnungs-Objekt-Sammlung.</span><span class="sxs-lookup"><span data-stu-id="41b3f-111">Get a licenseDetails object collection.</span></span> |
| [<span data-ttu-id="41b3f-112">get alerts</span><span class="sxs-lookup"><span data-stu-id="41b3f-112">get alerts</span></span>](../api/alert_get.md) | <span data-ttu-id="41b3f-113">[alert](alert.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="41b3f-113">[alert](alert.md) collection</span></span> | <span data-ttu-id="41b3f-114">Abruf eines Warnungs-Objekts.</span><span class="sxs-lookup"><span data-stu-id="41b3f-114">Get a alert object.</span></span> |
| [<span data-ttu-id="41b3f-115">Aktualisieren von Benachrichtigungen</span><span class="sxs-lookup"><span data-stu-id="41b3f-115">Update alerts</span></span>](../api/alert_update.md) | <span data-ttu-id="41b3f-116">[alert](alert.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="41b3f-116">[alert](alert.md) collection</span></span> | <span data-ttu-id="41b3f-117">Abruf eines Warnungs-Objekts.</span><span class="sxs-lookup"><span data-stu-id="41b3f-117">Get a alert object.</span></span> |

## <a name="properties"></a><span data-ttu-id="41b3f-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="41b3f-118">Properties</span></span>
<span data-ttu-id="41b3f-119">Keine</span><span class="sxs-lookup"><span data-stu-id="41b3f-119">None</span></span>

## <a name="relationships"></a><span data-ttu-id="41b3f-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="41b3f-120">Relationships</span></span>
| <span data-ttu-id="41b3f-121">Beziehung</span><span class="sxs-lookup"><span data-stu-id="41b3f-121">Relationship</span></span> | <span data-ttu-id="41b3f-122">Typ</span><span class="sxs-lookup"><span data-stu-id="41b3f-122">Type</span></span>        | <span data-ttu-id="41b3f-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="41b3f-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="41b3f-124">alerts</span><span class="sxs-lookup"><span data-stu-id="41b3f-124">alerts</span></span>|<span data-ttu-id="41b3f-125">[alert](alert.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="41b3f-125">[alert](alert.md) collection</span></span>| <span data-ttu-id="41b3f-p102">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="41b3f-p102">Read-only. Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="41b3f-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="41b3f-128">JSON representation</span></span>
<span data-ttu-id="41b3f-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="41b3f-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.security"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="41b3f-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="41b3f-130">Example</span></span>

<span data-ttu-id="41b3f-131">Die **security**-Ressource ist im Stamm des Diagramms verfügbar.</span><span class="sxs-lookup"><span data-stu-id="41b3f-131">The **security** resource is available at the root of the graph.</span></span>

<!--{
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/security
```

<!--{
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security"
}-->
```json
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "security resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->