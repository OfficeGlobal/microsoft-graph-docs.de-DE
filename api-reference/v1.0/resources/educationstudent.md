# <a name="educationstudent-resource-type"></a><span data-ttu-id="3fa71-101">educationStudent-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3fa71-101">educationStudent resource type</span></span>

<span data-ttu-id="3fa71-102">Zusätzliche Informationen, die einem vorhandenen [educationUser](educationuser.md) hinzugefügt werden, wenn die primaryRole eines Benutzers `student` ist.</span><span class="sxs-lookup"><span data-stu-id="3fa71-102">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="3fa71-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3fa71-103">Properties</span></span>
| <span data-ttu-id="3fa71-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3fa71-104">Property</span></span>     | <span data-ttu-id="3fa71-105">Typ</span><span class="sxs-lookup"><span data-stu-id="3fa71-105">Type</span></span>   |<span data-ttu-id="3fa71-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3fa71-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3fa71-107">birthDate</span><span class="sxs-lookup"><span data-stu-id="3fa71-107">birthDate</span></span>|<span data-ttu-id="3fa71-108">Date</span><span class="sxs-lookup"><span data-stu-id="3fa71-108">Date</span></span>| <span data-ttu-id="3fa71-109">Geburtsdatum des Kursteilnehmers.</span><span class="sxs-lookup"><span data-stu-id="3fa71-109">Birth date of the student.</span></span>|
|<span data-ttu-id="3fa71-110">externalId</span><span class="sxs-lookup"><span data-stu-id="3fa71-110">externalId</span></span>|<span data-ttu-id="3fa71-111">String</span><span class="sxs-lookup"><span data-stu-id="3fa71-111">String</span></span>| <span data-ttu-id="3fa71-112">ID des Kursteilnehmers im Quellsystem.</span><span class="sxs-lookup"><span data-stu-id="3fa71-112">ID of the student in the source system.</span></span>|
|<span data-ttu-id="3fa71-113">gender</span><span class="sxs-lookup"><span data-stu-id="3fa71-113">Gender</span></span>|`educationGender enumeration`| <span data-ttu-id="3fa71-114">Mögliche Werte: `female`, `male`, `other`, `unkownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="3fa71-114">Possible values are: `female`, `male`, `other`, `unkownFutureValue`.</span></span>|
|<span data-ttu-id="3fa71-115">grade</span><span class="sxs-lookup"><span data-stu-id="3fa71-115">QuizInfoPage: grade</span></span>|<span data-ttu-id="3fa71-116">String</span><span class="sxs-lookup"><span data-stu-id="3fa71-116">String</span></span>|<span data-ttu-id="3fa71-117">Aktuelle Klassenstufe des Kursteilnehmers.</span><span class="sxs-lookup"><span data-stu-id="3fa71-117">Current grade level of the student.</span></span>|
|<span data-ttu-id="3fa71-118">graduationYear</span><span class="sxs-lookup"><span data-stu-id="3fa71-118">graduationYear</span></span>|<span data-ttu-id="3fa71-119">String</span><span class="sxs-lookup"><span data-stu-id="3fa71-119">String</span></span>| <span data-ttu-id="3fa71-120">Jahr, in dem der Kursteilnehmer die Schule abschließt.</span><span class="sxs-lookup"><span data-stu-id="3fa71-120">Year the student is graduating from the school.</span></span>|
|<span data-ttu-id="3fa71-121">studentNumber</span><span class="sxs-lookup"><span data-stu-id="3fa71-121">studentNumber</span></span>|<span data-ttu-id="3fa71-122">String</span><span class="sxs-lookup"><span data-stu-id="3fa71-122">String</span></span>| <span data-ttu-id="3fa71-123">Kursteilnehmernummer</span><span class="sxs-lookup"><span data-stu-id="3fa71-123">Student Number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3fa71-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3fa71-124">JSON representation</span></span>

<span data-ttu-id="3fa71-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3fa71-125">The following is a JSON representation of the resource.</span></span>

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