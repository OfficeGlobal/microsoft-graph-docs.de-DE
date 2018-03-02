# <a name="educationteacher-resource-type"></a><span data-ttu-id="afae7-101">educationTeacher-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="afae7-101">educationTeacher resource type</span></span>

<span data-ttu-id="afae7-102">Zusätzliche Informationen, die einem vorhandenen [educationUser](educationuser.md) hinzugefügt werden, wenn die primaryRole eines Benutzers `teacher` ist.</span><span class="sxs-lookup"><span data-stu-id="afae7-102">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>


## <a name="properties"></a><span data-ttu-id="afae7-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="afae7-103">Properties</span></span>
| <span data-ttu-id="afae7-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="afae7-104">Property</span></span>     | <span data-ttu-id="afae7-105">Typ</span><span class="sxs-lookup"><span data-stu-id="afae7-105">Type</span></span>   |<span data-ttu-id="afae7-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="afae7-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="afae7-107">externalId</span><span class="sxs-lookup"><span data-stu-id="afae7-107">externalId</span></span>|<span data-ttu-id="afae7-108">String</span><span class="sxs-lookup"><span data-stu-id="afae7-108">String</span></span>| <span data-ttu-id="afae7-109">Die ID der Lehrkraft im Quellsystem.</span><span class="sxs-lookup"><span data-stu-id="afae7-109">ID of the teacher in the source system.</span></span>|
|<span data-ttu-id="afae7-110">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="afae7-110">teacherNumber</span></span>|<span data-ttu-id="afae7-111">String</span><span class="sxs-lookup"><span data-stu-id="afae7-111">String</span></span>|<span data-ttu-id="afae7-112">Lehrernummer</span><span class="sxs-lookup"><span data-stu-id="afae7-112">Teacher number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="afae7-113">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="afae7-113">JSON representation</span></span>

<span data-ttu-id="afae7-114">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="afae7-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationTeacher"
}-->

```json
{
  "externalId": "String",
  "teacherNumber": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationTeacher resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->