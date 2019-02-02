---
title: Ressourcentyp relatedContact
description: Wenden Sie sich an Datensatz im Zusammenhang mit einer EducationUser, die Informationen für Aufsichtspersonen, Datenblätter, Ärzten und So weiter bereitstellt.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: d29cf93154e2c032ac7010372e3f116f2a1dd46c
ms.sourcegitcommit: d6209114cbbe8072e3ecf7eba23819ae5ace7db5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/01/2019
ms.locfileid: "29694475"
---
# <a name="relatedcontact-resource-type"></a><span data-ttu-id="044d7-103">Ressourcentyp relatedContact</span><span class="sxs-lookup"><span data-stu-id="044d7-103">relatedContact resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="044d7-104">Wenden Sie sich an Datensatz im Zusammenhang mit einer [EducationUser](../resources/educationuser.md) , die Informationen für Aufsichtspersonen, Datenblätter, Ärzten und So weiter bereitstellt.</span><span class="sxs-lookup"><span data-stu-id="044d7-104">Contact record related to an [educationUser](../resources/educationuser.md) that provides inforation for guardians, aides, doctors, and so on.</span></span>

## <a name="properties"></a><span data-ttu-id="044d7-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="044d7-105">Properties</span></span>
| <span data-ttu-id="044d7-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="044d7-106">Property</span></span>     | <span data-ttu-id="044d7-107">Typ</span><span class="sxs-lookup"><span data-stu-id="044d7-107">Type</span></span>   |<span data-ttu-id="044d7-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="044d7-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="044d7-109">id</span><span class="sxs-lookup"><span data-stu-id="044d7-109">id</span></span>|<span data-ttu-id="044d7-110">string</span><span class="sxs-lookup"><span data-stu-id="044d7-110">String</span></span>|<span data-ttu-id="044d7-111">Die Identität des Kontakts in Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="044d7-111">Identity of the contact within Azure Active Directory.</span></span>|
|<span data-ttu-id="044d7-112">displayName</span><span class="sxs-lookup"><span data-stu-id="044d7-112">displayName</span></span>|<span data-ttu-id="044d7-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="044d7-113">String</span></span>|<span data-ttu-id="044d7-114">Name des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="044d7-114">Name of the contact.</span></span> <span data-ttu-id="044d7-115">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="044d7-115">Required.</span></span>|
|<span data-ttu-id="044d7-116">emailAddress</span><span class="sxs-lookup"><span data-stu-id="044d7-116">emailAddress</span></span>|<span data-ttu-id="044d7-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="044d7-117">String</span></span>|<span data-ttu-id="044d7-118">Primäre e-Mail-Adresse des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="044d7-118">Primary email address of the contact.</span></span>|
|<span data-ttu-id="044d7-119">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="044d7-119">mobilePhone</span></span>|<span data-ttu-id="044d7-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="044d7-120">String</span></span>|<span data-ttu-id="044d7-121">Die Mobiltelefonnummer des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="044d7-121">Mobile phone number of the contact.</span></span>|
|<span data-ttu-id="044d7-122">Beziehung</span><span class="sxs-lookup"><span data-stu-id="044d7-122">relationship</span></span>|`contactRelationship`|<span data-ttu-id="044d7-123">Beziehung für den Benutzer.</span><span class="sxs-lookup"><span data-stu-id="044d7-123">Relationship to the user.</span></span> <span data-ttu-id="044d7-124">Mögliche Werte sind `parent`, `relative`, `aide`, `doctor`, `guardian`, `child`, `other`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="044d7-124">Possible values are `parent`, `relative`, `aide`, `doctor`, `guardian`, `child`, `other`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="044d7-125">accessConsent</span><span class="sxs-lookup"><span data-stu-id="044d7-125">accessConsent</span></span>|<span data-ttu-id="044d7-126">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="044d7-126">Boolean</span></span>|<span data-ttu-id="044d7-127">Gibt an, ob der Benutzer Zugriff auf Daten Student zugestimmt wurde hat.</span><span class="sxs-lookup"><span data-stu-id="044d7-127">Indicates whether the user has been consented to access student data.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="044d7-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="044d7-128">JSON representation</span></span>

<span data-ttu-id="044d7-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="044d7-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.relatedContact"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "emailAddress": "String",
  "mobilePhone": "String",
  "relationship": "contactRelationship",
  "accessConsent": true
}
```

<!-- uuid: 720F9AB6-6E7A-4A66-8B0A-37A556FF99C5
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "relatedContact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
