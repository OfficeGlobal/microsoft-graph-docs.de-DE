---
title: Ressourcentyp agreementFile
description: Stellt eine anpassbare Begriffe der Vereinbarung-Datei verwenden, die ein Mandanten mit Azure Active Directory (AD Azure) verwaltet. Es enthält Metadaten zu einer Datei Vereinbarung (beispielsweise den Namen, die Sprache und ob sie die Standarddatei ist).
localization_priority: Normal
ms.openlocfilehash: 446173e83d32af96f938cbee15964ea204a62f7e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511429"
---
# <a name="agreementfile-resource-type"></a><span data-ttu-id="84c80-104">Ressourcentyp agreementFile</span><span class="sxs-lookup"><span data-stu-id="84c80-104">agreementFile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84c80-105">Stellt eine anpassbare Begriffe der Vereinbarung-Datei verwenden, die ein Mandanten mit Azure Active Directory (AD Azure) verwaltet.</span><span class="sxs-lookup"><span data-stu-id="84c80-105">Represents a customizable terms of use agreement file that a tenant manages with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="84c80-106">Es enthält Metadaten zu einer Datei Vereinbarung (beispielsweise den Namen, die Sprache und ob sie die Standarddatei ist).</span><span class="sxs-lookup"><span data-stu-id="84c80-106">It contains metadata about the agreement file (for example, the name, the language, and whether it is the default file).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementFile](../api/agreementfile-get.md) | [agreementFile](agreementfile.md) | Read properties and relationships of an **agreementFile** object. |
| [Update](../api/agreementfile-update.md) | [agreementFile](agreementfile.md) | Update an **agreementFile** object. |
| [Delete](../api/agreementfile-delete.md) | None | Delete an **agreementFile** object. |
-->

## <a name="properties"></a><span data-ttu-id="84c80-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="84c80-107">Properties</span></span>
| <span data-ttu-id="84c80-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="84c80-108">Property</span></span>     | <span data-ttu-id="84c80-109">Typ</span><span class="sxs-lookup"><span data-stu-id="84c80-109">Type</span></span>        | <span data-ttu-id="84c80-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="84c80-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="84c80-111">fileData</span><span class="sxs-lookup"><span data-stu-id="84c80-111">fileData</span></span>|[<span data-ttu-id="84c80-112">agreementFileData</span><span class="sxs-lookup"><span data-stu-id="84c80-112">agreementFileData</span></span>](agreementfiledata.md)|<span data-ttu-id="84c80-113">Daten, die die Begriffe verwenden PDF-Dokument darstellt.</span><span class="sxs-lookup"><span data-stu-id="84c80-113">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="84c80-114">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="84c80-114">Read-only.</span></span>|
|<span data-ttu-id="84c80-115">fileName</span><span class="sxs-lookup"><span data-stu-id="84c80-115">fileName</span></span>|<span data-ttu-id="84c80-116">String</span><span class="sxs-lookup"><span data-stu-id="84c80-116">String</span></span>|<span data-ttu-id="84c80-117">Name der Datei Vereinbarung (beispielsweise TOU.pdf).</span><span class="sxs-lookup"><span data-stu-id="84c80-117">Name of the agreement file (for example, TOU.pdf).</span></span> <span data-ttu-id="84c80-118">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="84c80-118">Read-only.</span></span>|
|<span data-ttu-id="84c80-119">id</span><span class="sxs-lookup"><span data-stu-id="84c80-119">id</span></span>|<span data-ttu-id="84c80-120">String</span><span class="sxs-lookup"><span data-stu-id="84c80-120">String</span></span>|<span data-ttu-id="84c80-121">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="84c80-121">Read-only.</span></span>|
|<span data-ttu-id="84c80-122">isDefault</span><span class="sxs-lookup"><span data-stu-id="84c80-122">isDefault</span></span>|<span data-ttu-id="84c80-123">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="84c80-123">Boolean</span></span>|<span data-ttu-id="84c80-124">Gibt an, ob dies Vereinbarung Standarddatei ist, wenn keiner der Kulturen die Client-Vorgabe übereinstimmt.</span><span class="sxs-lookup"><span data-stu-id="84c80-124">Indicates whether this is the default agreement file if none of the cultures matches the client preference.</span></span> <span data-ttu-id="84c80-125">Wenn keine der Dateien als Standard gekennzeichnet sind, wird der ersten als Standard behandelt.</span><span class="sxs-lookup"><span data-stu-id="84c80-125">If none of the files are marked as default, the first one will be treated as the default.</span></span> <span data-ttu-id="84c80-126">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="84c80-126">Read-only.</span></span>|
|<span data-ttu-id="84c80-127">language</span><span class="sxs-lookup"><span data-stu-id="84c80-127">language</span></span>|<span data-ttu-id="84c80-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="84c80-128">String</span></span>|<span data-ttu-id="84c80-129">Kultur der Vereinbarung Datei im Format languagecode2-Land/regioncode2.</span><span class="sxs-lookup"><span data-stu-id="84c80-129">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="84c80-130">languagecode2 ist eine zwei-Code aus Kleinbuchstaben ISO 639-1 abgeleitet.</span><span class="sxs-lookup"><span data-stu-id="84c80-130">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="84c80-131">Land/regioncode2 ISO 3166 abgeleitet ist und in der Regel besteht aus zwei Großbuchstaben oder ein Sprachtag BCP 47 (z. B. En-US).</span><span class="sxs-lookup"><span data-stu-id="84c80-131">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span> <span data-ttu-id="84c80-132">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="84c80-132">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="84c80-133">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="84c80-133">Relationships</span></span>
<span data-ttu-id="84c80-134">Keine.</span><span class="sxs-lookup"><span data-stu-id="84c80-134">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="84c80-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="84c80-135">JSON representation</span></span>

<span data-ttu-id="84c80-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="84c80-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementFile"
}-->

```json
{
  "fileData": {"@odata.type": "microsoft.graph.agreementFileData"},
  "fileName": "String",
  "id": "String (identifier)",
  "isDefault": true,
  "language": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreementFile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/agreementfile.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
