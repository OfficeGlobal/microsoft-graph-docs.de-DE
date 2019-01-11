---
title: privacyProfile-Ressourcentyp
description: Stellt das Datenschutzprofil eines Unternehmens dar, das eine URL zu einer Datenschutzerklärung sowie eine Kontaktperson für Fragen im Zusammenhang mit der Datenschutzerklärung umfasst.
localization_priority: Normal
ms.openlocfilehash: 29c4a01cde0e05c42ce74576e769ca005840e854
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884980"
---
# <a name="privacyprofile-resource-type"></a><span data-ttu-id="17b8f-103">privacyProfile-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="17b8f-103">privacyProfile resource type</span></span>

<span data-ttu-id="17b8f-104">Stellt das Datenschutzprofil eines Unternehmens dar, das eine URL zu einer Datenschutzerklärung sowie eine Kontaktperson für Fragen im Zusammenhang mit der Datenschutzerklärung umfasst.</span><span class="sxs-lookup"><span data-stu-id="17b8f-104">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="17b8f-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="17b8f-105">Properties</span></span>
| <span data-ttu-id="17b8f-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="17b8f-106">Property</span></span>   | <span data-ttu-id="17b8f-107">Typ</span><span class="sxs-lookup"><span data-stu-id="17b8f-107">Type</span></span>|<span data-ttu-id="17b8f-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="17b8f-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="17b8f-109">contactEmail</span><span class="sxs-lookup"><span data-stu-id="17b8f-109">contactEmail</span></span>|<span data-ttu-id="17b8f-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="17b8f-110">String</span></span>| <span data-ttu-id="17b8f-111">Eine gültige SMTP-E-Mail-Adresse für den Kontakt für die Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="17b8f-111">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="17b8f-112">Nicht erforderlich.</span><span class="sxs-lookup"><span data-stu-id="17b8f-112">Not required.</span></span>|
|<span data-ttu-id="17b8f-113">statementUrl</span><span class="sxs-lookup"><span data-stu-id="17b8f-113">statementUrl</span></span>|<span data-ttu-id="17b8f-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="17b8f-114">String</span></span>| <span data-ttu-id="17b8f-115">Ein gültiges URL-Format, das mit „http://“ oder „https://“ beginnt.</span><span class="sxs-lookup"><span data-stu-id="17b8f-115">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="17b8f-116">Die maximale Länge beträgt 255 Zeichen.</span><span class="sxs-lookup"><span data-stu-id="17b8f-116">Maximum length is 255 characters.</span></span> <span data-ttu-id="17b8f-117">Die URL, die zur Datenschutzerklärung des Unternehmens weiterleitet.</span><span class="sxs-lookup"><span data-stu-id="17b8f-117">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="17b8f-118">Nicht erforderlich.</span><span class="sxs-lookup"><span data-stu-id="17b8f-118">Not required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="17b8f-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="17b8f-119">JSON representation</span></span>

<span data-ttu-id="17b8f-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="17b8f-120">Here is a JSON representation of the resource</span></span>

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
