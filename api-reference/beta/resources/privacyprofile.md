---
title: privacyProfile-Ressourcentyp
description: Stellt das Datenschutzprofil eines Unternehmens dar, das eine URL zu einer Datenschutzerklärung sowie eine Kontaktperson für Fragen im Zusammenhang mit der Datenschutzerklärung umfasst.
localization_priority: Normal
ms.openlocfilehash: 9c110cbdb8a456b43936d3b56db5d4563686ed6e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510120"
---
# <a name="privacyprofile-resource-type"></a><span data-ttu-id="6275d-103">privacyProfile-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6275d-103">privacyProfile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6275d-104">Stellt das Datenschutzprofil eines Unternehmens dar, das eine URL zu einer Datenschutzerklärung sowie eine Kontaktperson für Fragen im Zusammenhang mit der Datenschutzerklärung umfasst.</span><span class="sxs-lookup"><span data-stu-id="6275d-104">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="6275d-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6275d-105">Properties</span></span>
| <span data-ttu-id="6275d-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6275d-106">Property</span></span>   | <span data-ttu-id="6275d-107">Typ</span><span class="sxs-lookup"><span data-stu-id="6275d-107">Type</span></span>|<span data-ttu-id="6275d-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6275d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6275d-109">contactEmail</span><span class="sxs-lookup"><span data-stu-id="6275d-109">contactEmail</span></span>|<span data-ttu-id="6275d-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6275d-110">String</span></span>| <span data-ttu-id="6275d-111">Eine gültige SMTP-E-Mail-Adresse für den Kontakt für die Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="6275d-111">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="6275d-112">Nicht erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6275d-112">Not required.</span></span>|
|<span data-ttu-id="6275d-113">statementUrl</span><span class="sxs-lookup"><span data-stu-id="6275d-113">statementUrl</span></span>|<span data-ttu-id="6275d-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6275d-114">String</span></span>| <span data-ttu-id="6275d-115">Ein gültiges URL-Format, das mit „http://“ oder „https://“ beginnt.</span><span class="sxs-lookup"><span data-stu-id="6275d-115">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="6275d-116">Die maximale Länge beträgt 255 Zeichen.</span><span class="sxs-lookup"><span data-stu-id="6275d-116">Maximum length is 255 characters.</span></span> <span data-ttu-id="6275d-117">Die URL, die zur Datenschutzerklärung des Unternehmens weiterleitet.</span><span class="sxs-lookup"><span data-stu-id="6275d-117">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="6275d-118">Nicht erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6275d-118">Not required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6275d-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6275d-119">JSON representation</span></span>

<span data-ttu-id="6275d-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6275d-120">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privacyProfile"
}-->

```json
{
  "contactEmail": "string",
  "statementUrl": "string"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/privacyprofile.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
