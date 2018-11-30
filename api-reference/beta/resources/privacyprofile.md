---
title: privacyProfile-Ressourcentyp
description: Stellt das Datenschutzprofil eines Unternehmens dar, das eine URL zu einer Datenschutzerklärung sowie eine Kontaktperson für Fragen im Zusammenhang mit der Datenschutzerklärung umfasst.
ms.openlocfilehash: fb9d5f929f1c9ae28687b80e987dc0909387f5d6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065766"
---
# <a name="privacyprofile-resource-type"></a><span data-ttu-id="f9a2c-103">privacyProfile-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f9a2c-103">privacyProfile resource type</span></span>

> <span data-ttu-id="f9a2c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f9a2c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f9a2c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f9a2c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f9a2c-106">Stellt das Datenschutzprofil eines Unternehmens dar, das eine URL zu einer Datenschutzerklärung sowie eine Kontaktperson für Fragen im Zusammenhang mit der Datenschutzerklärung umfasst.</span><span class="sxs-lookup"><span data-stu-id="f9a2c-106">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="f9a2c-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f9a2c-107">Properties</span></span>
| <span data-ttu-id="f9a2c-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f9a2c-108">Property</span></span>   | <span data-ttu-id="f9a2c-109">Typ</span><span class="sxs-lookup"><span data-stu-id="f9a2c-109">Type</span></span>|<span data-ttu-id="f9a2c-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f9a2c-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f9a2c-111">contactEmail</span><span class="sxs-lookup"><span data-stu-id="f9a2c-111">contactEmail</span></span>|<span data-ttu-id="f9a2c-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f9a2c-112">String</span></span>| <span data-ttu-id="f9a2c-113">Eine gültige SMTP-E-Mail-Adresse für den Kontakt für die Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="f9a2c-113">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="f9a2c-114">Nicht erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f9a2c-114">Not required.</span></span>|
|<span data-ttu-id="f9a2c-115">statementUrl</span><span class="sxs-lookup"><span data-stu-id="f9a2c-115">statementUrl</span></span>|<span data-ttu-id="f9a2c-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f9a2c-116">String</span></span>| <span data-ttu-id="f9a2c-117">Ein gültiges URL-Format, das mit „http://“ oder „https://“ beginnt.</span><span class="sxs-lookup"><span data-stu-id="f9a2c-117">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="f9a2c-118">Die maximale Länge beträgt 255 Zeichen.</span><span class="sxs-lookup"><span data-stu-id="f9a2c-118">Maximum length is 255 characters.</span></span> <span data-ttu-id="f9a2c-119">Die URL, die zur Datenschutzerklärung des Unternehmens weiterleitet.</span><span class="sxs-lookup"><span data-stu-id="f9a2c-119">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="f9a2c-120">Nicht erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f9a2c-120">Not required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f9a2c-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f9a2c-121">JSON representation</span></span>

<span data-ttu-id="f9a2c-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f9a2c-122">Here is a JSON representation of the resource</span></span>

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