---
title: Ressourcentyp mfaDetail
description: 'Gibt Details für eine bestimmte Anmeldung mehrstufiger Authentifizierung das an. Sie enthält die Authentifizierungsmethode für die Anmeldung sowie Details Auth (zum Beispiel: Telefon, SMS oder Voicemail) '
localization_priority: Normal
ms.openlocfilehash: 5069045fd202d443a94a80f7333f12ab5e707ada
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883741"
---
# <a name="mfadetail-resource-type"></a><span data-ttu-id="72e9e-104">Ressourcentyp mfaDetail</span><span class="sxs-lookup"><span data-stu-id="72e9e-104">mfaDetail resource type</span></span>
<span data-ttu-id="72e9e-105">Gibt Details für eine bestimmte Anmeldung mehrstufiger Authentifizierung das an.</span><span class="sxs-lookup"><span data-stu-id="72e9e-105">Indicates MFA details for a specific sign-in.</span></span> <span data-ttu-id="72e9e-106">Sie enthält die Authentifizierungsmethode für die Anmeldung sowie Details Auth (zum Beispiel: Telefon, SMS oder Voicemail)</span><span class="sxs-lookup"><span data-stu-id="72e9e-106">It includes the authentication method used for signing in as well as auth details (for example: Phone, SMS or voicemail)</span></span> 



## <a name="properties"></a><span data-ttu-id="72e9e-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="72e9e-107">Properties</span></span>
| <span data-ttu-id="72e9e-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="72e9e-108">Property</span></span>     | <span data-ttu-id="72e9e-109">Typ</span><span class="sxs-lookup"><span data-stu-id="72e9e-109">Type</span></span>   |<span data-ttu-id="72e9e-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="72e9e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="72e9e-111">authDetail</span><span class="sxs-lookup"><span data-stu-id="72e9e-111">authDetail</span></span>|<span data-ttu-id="72e9e-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="72e9e-112">String</span></span>|<span data-ttu-id="72e9e-113">Gibt an, für die entsprechende Aktivität-in den Details der mehrstufiger Authentifizierung das Auth der mehrstufiger Authentifizierung das erforderlich ist, "Yes".</span><span class="sxs-lookup"><span data-stu-id="72e9e-113">Indicates the MFA auth detail for the corresponding Sign-in activity when the MFA Required is "Yes".</span></span>|
|<span data-ttu-id="72e9e-114">Authentifizierungsmethode</span><span class="sxs-lookup"><span data-stu-id="72e9e-114">authMethod</span></span>|<span data-ttu-id="72e9e-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="72e9e-115">String</span></span>|<span data-ttu-id="72e9e-116">Gibt die mehrstufiger Authentifizierung das Auth-Methoden (SMS, Telefon- und Authentifizierungsserver App sind einige der Wert) für die entsprechende Aktivität-Anmeldung bei das mehrstufiger Authentifizierung das erforderliche Feld ist "Yes" an.</span><span class="sxs-lookup"><span data-stu-id="72e9e-116">Indicates the MFA Auth methods (SMS, Phone, Authenticator App are some of the value) for the corresponding sign-in activity when the MFA Required field is "Yes".</span></span>|

## <a name="json-representation"></a><span data-ttu-id="72e9e-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="72e9e-117">JSON representation</span></span>

<span data-ttu-id="72e9e-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="72e9e-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mfaDetail"
}-->

```json
{
  "authDetail": "String",
  "authMethod": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mfaDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
