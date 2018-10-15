# <a name="educationstudent-resource-type"></a><span data-ttu-id="81049-101">educationStudent-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="81049-101">educationStudent resource type</span></span>

<span data-ttu-id="81049-102">Zusätzliche Informationen, die einem vorhandenen [educationUser](educationuser.md) hinzugefügt werden, wenn die primaryRole eines Benutzers `student` ist.</span><span class="sxs-lookup"><span data-stu-id="81049-102">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="81049-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="81049-103">Properties</span></span>
| <span data-ttu-id="81049-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="81049-104">Property</span></span>     | <span data-ttu-id="81049-105">Typ</span><span class="sxs-lookup"><span data-stu-id="81049-105">Type</span></span>   |<span data-ttu-id="81049-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="81049-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81049-107">birthDate</span><span class="sxs-lookup"><span data-stu-id="81049-107">birthDate</span></span>|<span data-ttu-id="81049-108">Datum</span><span class="sxs-lookup"><span data-stu-id="81049-108">Date</span></span>| <span data-ttu-id="81049-109">Geburtsdatum des Kursteilnehmers.</span><span class="sxs-lookup"><span data-stu-id="81049-109">Birth date of the student.</span></span>|
|<span data-ttu-id="81049-110">externalId</span><span class="sxs-lookup"><span data-stu-id="81049-110">externalId</span></span>|<span data-ttu-id="81049-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="81049-111">String</span></span>| <span data-ttu-id="81049-112">ID des Kursteilnehmers im Quellsystem.</span><span class="sxs-lookup"><span data-stu-id="81049-112">ID of the student in the source system.</span></span>|
|<span data-ttu-id="81049-113">gender</span><span class="sxs-lookup"><span data-stu-id="81049-113">gender</span></span>|<span data-ttu-id="81049-114">educationGender</span><span class="sxs-lookup"><span data-stu-id="81049-114">educationGender values</span></span>| <span data-ttu-id="81049-115">Die möglichen Werte sind: `female`, `male`, `other`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="81049-115">The possible values are `female`, `male`, `other`, `unknownFutureValue`, , , , , , , , or .</span></span>|
|<span data-ttu-id="81049-116">Ergebnis</span><span class="sxs-lookup"><span data-stu-id="81049-116">grade</span></span>|<span data-ttu-id="81049-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="81049-117">String</span></span>|<span data-ttu-id="81049-118">Aktuelle Klassenstufe des Kursteilnehmers.</span><span class="sxs-lookup"><span data-stu-id="81049-118">Current grade level of the student.</span></span>|
|<span data-ttu-id="81049-119">graduationYear</span><span class="sxs-lookup"><span data-stu-id="81049-119">graduationYear</span></span>|<span data-ttu-id="81049-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="81049-120">String</span></span>| <span data-ttu-id="81049-121">Jahr, in dem der Kursteilnehmer die Schule abschließt.</span><span class="sxs-lookup"><span data-stu-id="81049-121">Year the student is graduating from the school.</span></span>|
|<span data-ttu-id="81049-122">studentNumber</span><span class="sxs-lookup"><span data-stu-id="81049-122">studentNumber</span></span>|<span data-ttu-id="81049-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="81049-123">String</span></span>| <span data-ttu-id="81049-124">Kursteilnehmernummer</span><span class="sxs-lookup"><span data-stu-id="81049-124">Student Number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="81049-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="81049-125">JSON representation</span></span>

<span data-ttu-id="81049-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="81049-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationStudent"
}-->

```json
{
  "birthDate": "String (timestamp)",
  "externalId": "String",
  "gender": "educationGender",
  "grade": "String",
  "graduationYear": "String",
  "studentNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationStudent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
