---
title: Ressourcentyp parentalControlSettings
description: Gibt die Altersfreigabe Einstellungen für eine Anwendung. Diese Einstellungen Steuern der Zustimmung wünschen.
localization_priority: Normal
ms.openlocfilehash: 8a3a768cc9264b6d1a25532455da20d87a5bc4e8
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573872"
---
# <a name="parentalcontrolsettings-resource-type"></a><span data-ttu-id="79885-104">Ressourcentyp parentalControlSettings</span><span class="sxs-lookup"><span data-stu-id="79885-104">parentalControlSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79885-105">Gibt die Altersfreigabe Einstellungen für eine Anwendung.</span><span class="sxs-lookup"><span data-stu-id="79885-105">Specifies parental control settings for an application.</span></span> <span data-ttu-id="79885-106">Diese Einstellungen Steuern der Zustimmung wünschen.</span><span class="sxs-lookup"><span data-stu-id="79885-106">These settings control the consent experience.</span></span>

## <a name="properties"></a><span data-ttu-id="79885-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="79885-107">Properties</span></span>

| <span data-ttu-id="79885-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="79885-108">Property</span></span> | <span data-ttu-id="79885-109">Typ</span><span class="sxs-lookup"><span data-stu-id="79885-109">Type</span></span> | <span data-ttu-id="79885-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="79885-110">Description</span></span> |
:---------------|:--------|:----------|
|<span data-ttu-id="79885-111">countriesBlockedForMinors</span><span class="sxs-lookup"><span data-stu-id="79885-111">countriesBlockedForMinors</span></span>|<span data-ttu-id="79885-112">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="79885-112">String collection</span></span>| <span data-ttu-id="79885-113">Gibt die [zwei Buchstaben ISO-Ländercodes](https://www.iso.org/iso-3166-country-codes.html).</span><span class="sxs-lookup"><span data-stu-id="79885-113">Specifies the [two-letter ISO country codes](https://www.iso.org/iso-3166-country-codes.html).</span></span> <span data-ttu-id="79885-114">Zugriff auf die Anwendung werden für Minderjährige aus den in dieser Liste angegebenen Ländern blockiert.</span><span class="sxs-lookup"><span data-stu-id="79885-114">Access to the application will be blocked for minors from the countries specified in this list.</span></span>|
|<span data-ttu-id="79885-115">legalAgeGroupRule</span><span class="sxs-lookup"><span data-stu-id="79885-115">legalAgeGroupRule</span></span>| <span data-ttu-id="79885-116">String</span><span class="sxs-lookup"><span data-stu-id="79885-116">String</span></span> | <span data-ttu-id="79885-117">Gibt die ALTER Legal Gruppenregel, die für Benutzer der app gilt.</span><span class="sxs-lookup"><span data-stu-id="79885-117">Specifies the legal age group rule that applies to users of the app.</span></span> <span data-ttu-id="79885-118">Kann auf einen der folgenden Werte festgelegt werden:</span><span class="sxs-lookup"><span data-stu-id="79885-118">Can be set to one of the following values:</span></span> <table><tr><th><span data-ttu-id="79885-119">Wert</span><span class="sxs-lookup"><span data-stu-id="79885-119">Value</span></span></th><th><span data-ttu-id="79885-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="79885-120">Description</span></span></th></tr><tr><td><span data-ttu-id="79885-121">Allow</span><span class="sxs-lookup"><span data-stu-id="79885-121">Allow</span></span></td><td><span data-ttu-id="79885-122">Standard.</span><span class="sxs-lookup"><span data-stu-id="79885-122">Default.</span></span> <span data-ttu-id="79885-123">Erzwingt die rechtliche minimale.</span><span class="sxs-lookup"><span data-stu-id="79885-123">Enforces the legal minimum.</span></span> <span data-ttu-id="79885-124">Dies bedeutet, dass die Zustimmung der Eltern für Minderjährige in der Europäischen Union und Korea erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="79885-124">This means parental consent is required for minors in the European Union and Korea.</span></span></td></tr><tr><td><span data-ttu-id="79885-125">RequireConsentForPrivacyServices</span><span class="sxs-lookup"><span data-stu-id="79885-125">RequireConsentForPrivacyServices</span></span></td><td><span data-ttu-id="79885-126">Erzwingt den Benutzer zum Angeben von Geburtsdatum COPPA-Regeln einhalten.</span><span class="sxs-lookup"><span data-stu-id="79885-126">Enforces the user to specify date of birth to comply with COPPA rules.</span></span> </td></tr><tr><td><span data-ttu-id="79885-127">RequireConsentForMinors</span><span class="sxs-lookup"><span data-stu-id="79885-127">RequireConsentForMinors</span></span></td><td><span data-ttu-id="79885-128">Erfordert Zustimmung der Eltern für Jahren unter 18, unabhängig davon Land minor Regeln.</span><span class="sxs-lookup"><span data-stu-id="79885-128">Requires parental consent for ages below 18, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="79885-129">RequireConsentForKids</span><span class="sxs-lookup"><span data-stu-id="79885-129">RequireConsentForKids</span></span></td><td><span data-ttu-id="79885-130">Erfordert Zustimmung der Eltern für Jahren unter 14, unabhängig davon Land minor Regeln.</span><span class="sxs-lookup"><span data-stu-id="79885-130">Requires parental consent for ages below 14, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="79885-131">BlockMinors</span><span class="sxs-lookup"><span data-stu-id="79885-131">BlockMinors</span></span></td><td><span data-ttu-id="79885-132">Blöcke Minderjährige aus mithilfe der app.</span><span class="sxs-lookup"><span data-stu-id="79885-132">Blocks minors from using the app.</span></span></td></tr></table> |

## <a name="json-representation"></a><span data-ttu-id="79885-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="79885-133">JSON representation</span></span>
<span data-ttu-id="79885-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="79885-134">Here is a JSON representation of the resource.</span></span>
<!-- 
{
    "blockType": "resource",
    "@odata.type":"microsoft.graph.parentalControlSettings"
}
-->
```json
{
  "countriesBlockedForMinors": [ "String" ],
  "legalAgeGroupRule": "String"
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/parentalcontrolsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
