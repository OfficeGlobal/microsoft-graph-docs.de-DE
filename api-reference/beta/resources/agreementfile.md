---
title: Ressourcentyp agreementFile
description: Stellt eine anpassbare Begriffe der Vereinbarung-Datei verwenden, die ein Mandanten mit Azure Active Directory (AD Azure) verwaltet. Es enthält Metadaten zu einer Datei Vereinbarung (beispielsweise den Namen, die Sprache und ob sie die Standarddatei ist).
ms.openlocfilehash: f099715fd25fbae9d7b2a94d6de841b8766c30e2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061945"
---
# <a name="agreementfile-resource-type"></a><span data-ttu-id="b4a67-104">Ressourcentyp agreementFile</span><span class="sxs-lookup"><span data-stu-id="b4a67-104">agreementFile resource type</span></span>

> <span data-ttu-id="b4a67-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b4a67-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b4a67-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b4a67-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b4a67-107">Stellt eine anpassbare Begriffe der Vereinbarung-Datei verwenden, die ein Mandanten mit Azure Active Directory (AD Azure) verwaltet.</span><span class="sxs-lookup"><span data-stu-id="b4a67-107">Represents a customizable terms of use agreement file that a tenant manages with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="b4a67-108">Es enthält Metadaten zu einer Datei Vereinbarung (beispielsweise den Namen, die Sprache und ob sie die Standarddatei ist).</span><span class="sxs-lookup"><span data-stu-id="b4a67-108">It contains metadata about the agreement file (for example, the name, the language, and whether it is the default file).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementFile](../api/agreementfile-get.md) | [agreementFile](agreementfile.md) | Read properties and relationships of an **agreementFile** object. |
| [Update](../api/agreementfile-update.md) | [agreementFile](agreementfile.md) | Update an **agreementFile** object. |
| [Delete](../api/agreementfile-delete.md) | None | Delete an **agreementFile** object. |
-->

## <a name="properties"></a><span data-ttu-id="b4a67-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b4a67-109">Properties</span></span>
| <span data-ttu-id="b4a67-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b4a67-110">Property</span></span>     | <span data-ttu-id="b4a67-111">Typ</span><span class="sxs-lookup"><span data-stu-id="b4a67-111">Type</span></span>        | <span data-ttu-id="b4a67-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b4a67-112">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b4a67-113">fileData</span><span class="sxs-lookup"><span data-stu-id="b4a67-113">fileData</span></span>|[<span data-ttu-id="b4a67-114">agreementFileData</span><span class="sxs-lookup"><span data-stu-id="b4a67-114">agreementFileData</span></span>](agreementfiledata.md)|<span data-ttu-id="b4a67-115">Daten, die die Begriffe verwenden PDF-Dokument darstellt.</span><span class="sxs-lookup"><span data-stu-id="b4a67-115">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="b4a67-116">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b4a67-116">Read-only.</span></span>|
|<span data-ttu-id="b4a67-117">fileName</span><span class="sxs-lookup"><span data-stu-id="b4a67-117">fileName</span></span>|<span data-ttu-id="b4a67-118">String</span><span class="sxs-lookup"><span data-stu-id="b4a67-118">String</span></span>|<span data-ttu-id="b4a67-119">Name der Datei Vereinbarung (beispielsweise TOU.pdf).</span><span class="sxs-lookup"><span data-stu-id="b4a67-119">Name of the agreement file (for example, TOU.pdf).</span></span> <span data-ttu-id="b4a67-120">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b4a67-120">Read-only.</span></span>|
|<span data-ttu-id="b4a67-121">id</span><span class="sxs-lookup"><span data-stu-id="b4a67-121">id</span></span>|<span data-ttu-id="b4a67-122">String</span><span class="sxs-lookup"><span data-stu-id="b4a67-122">String</span></span>|<span data-ttu-id="b4a67-123">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b4a67-123">Read-only.</span></span>|
|<span data-ttu-id="b4a67-124">isDefault</span><span class="sxs-lookup"><span data-stu-id="b4a67-124">isDefault</span></span>|<span data-ttu-id="b4a67-125">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4a67-125">Boolean</span></span>|<span data-ttu-id="b4a67-126">Gibt an, ob dies Vereinbarung Standarddatei ist, wenn keiner der Kulturen die Client-Vorgabe übereinstimmt.</span><span class="sxs-lookup"><span data-stu-id="b4a67-126">Indicates whether this is the default agreement file if none of the cultures matches the client preference.</span></span> <span data-ttu-id="b4a67-127">Wenn keine der Dateien als Standard gekennzeichnet sind, wird der ersten als Standard behandelt.</span><span class="sxs-lookup"><span data-stu-id="b4a67-127">If none of the files are marked as default, the first one will be treated as the default.</span></span> <span data-ttu-id="b4a67-128">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b4a67-128">Read-only.</span></span>|
|<span data-ttu-id="b4a67-129">language</span><span class="sxs-lookup"><span data-stu-id="b4a67-129">language</span></span>|<span data-ttu-id="b4a67-130">String</span><span class="sxs-lookup"><span data-stu-id="b4a67-130">String</span></span>|<span data-ttu-id="b4a67-131">Kultur der Vereinbarung Datei im Format languagecode2-Land/regioncode2.</span><span class="sxs-lookup"><span data-stu-id="b4a67-131">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="b4a67-132">languagecode2 ist eine zwei-Code aus Kleinbuchstaben ISO 639-1 abgeleitet.</span><span class="sxs-lookup"><span data-stu-id="b4a67-132">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="b4a67-133">Land/regioncode2 ISO 3166 abgeleitet ist und in der Regel besteht aus zwei Großbuchstaben oder ein Sprachtag BCP 47 (z. B. En-US).</span><span class="sxs-lookup"><span data-stu-id="b4a67-133">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span> <span data-ttu-id="b4a67-134">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b4a67-134">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b4a67-135">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b4a67-135">Relationships</span></span>
<span data-ttu-id="b4a67-136">Keine.</span><span class="sxs-lookup"><span data-stu-id="b4a67-136">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="b4a67-137">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b4a67-137">JSON representation</span></span>

<span data-ttu-id="b4a67-138">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b4a67-138">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "agreementFile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
