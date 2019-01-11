---
title: Ressourcentyp office365ActivationsUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: f87a5b32b08466428f0f6f0246a4b8d4c20e97be
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877336"
---
# <a name="office365activationsuserdetail-resource-type"></a><span data-ttu-id="ac3ed-103">Ressourcentyp office365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="ac3ed-103">office365ActivationsUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="ac3ed-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ac3ed-104">Properties</span></span>

| <span data-ttu-id="ac3ed-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ac3ed-105">Property</span></span>             | <span data-ttu-id="ac3ed-106">Typ</span><span class="sxs-lookup"><span data-stu-id="ac3ed-106">Type</span></span>                                     | <span data-ttu-id="ac3ed-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ac3ed-107">Description</span></span>                              |
| :------------------- | :--------------------------------------- | ---------------------------------------- |
| <span data-ttu-id="ac3ed-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="ac3ed-108">reportRefreshDate</span></span>    | <span data-ttu-id="ac3ed-109">Datum</span><span class="sxs-lookup"><span data-stu-id="ac3ed-109">Date</span></span>                                     | <span data-ttu-id="ac3ed-110">Das aktuelle Datum des Inhalts.</span><span class="sxs-lookup"><span data-stu-id="ac3ed-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="ac3ed-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ac3ed-111">userPrincipalName</span></span>    | <span data-ttu-id="ac3ed-112">String</span><span class="sxs-lookup"><span data-stu-id="ac3ed-112">String</span></span>                                   | <span data-ttu-id="ac3ed-113">Der Benutzerprinzipalname (UPN) des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="ac3ed-113">The user principal name (UPN) of the user.</span></span> <span data-ttu-id="ac3ed-114">Der Benutzerprinzipalname ist ein Internet-Schreibweise Anmeldenamen für den Benutzer anhand der Internetstandard RFC 822.</span><span class="sxs-lookup"><span data-stu-id="ac3ed-114">The UPN is an Internet-style login name for the user based on the Internet standard RFC 822.</span></span> <span data-ttu-id="ac3ed-115">Standardmäßig sollte dies der Name des Benutzers e-Mail zuordnen.</span><span class="sxs-lookup"><span data-stu-id="ac3ed-115">By convention, this should map to the user's email name.</span></span> <span data-ttu-id="ac3ed-116">Das Standardformat ist alias@domain, wobei muss Domäne in den Mandanten-Auflistung der überprüften Domänen vorhanden sein.</span><span class="sxs-lookup"><span data-stu-id="ac3ed-116">The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains.</span></span> <span data-ttu-id="ac3ed-117">Diese Eigenschaft ist erforderlich, wenn ein Benutzer erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="ac3ed-117">This property is required when a user is created.</span></span> |
| <span data-ttu-id="ac3ed-118">displayName</span><span class="sxs-lookup"><span data-stu-id="ac3ed-118">displayName</span></span>          | <span data-ttu-id="ac3ed-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ac3ed-119">String</span></span>                                   | <span data-ttu-id="ac3ed-120">Der Name des Benutzers, der im Adressbuch angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="ac3ed-120">The name displayed in the address book for the user.</span></span> <span data-ttu-id="ac3ed-121">Dies ist normalerweise eine Kombination aus dem Vornamen, der Initiale des weiteren Vornamens und des Nachnamens.</span><span class="sxs-lookup"><span data-stu-id="ac3ed-121">This is usually the combination of the user's first name, middle initial, and last name.</span></span> <span data-ttu-id="ac3ed-122">Diese Eigenschaft ist beim Erstellen eines Benutzers erforderlich und kann nicht bei Updates deaktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="ac3ed-122">This property is required when a user is created and it cannot be cleared during updates.</span></span> |
| <span data-ttu-id="ac3ed-123">userActivationCounts</span><span class="sxs-lookup"><span data-stu-id="ac3ed-123">userActivationCounts</span></span> | <span data-ttu-id="ac3ed-124">[UserActivationCounts](../resources/useractivationcounts.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="ac3ed-124">[userActivationCounts](../resources/useractivationcounts.md) collection</span></span> | <span data-ttu-id="ac3ed-125">Neueste produktaktivierung des Benutzers wird auf allen Plattformen für alle zugewiesenen Produkttypen gezählt.</span><span class="sxs-lookup"><span data-stu-id="ac3ed-125">The user's latest product activation counts on all the platforms for all the assigned product types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ac3ed-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ac3ed-126">JSON representation</span></span>

<span data-ttu-id="ac3ed-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ac3ed-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActivationsUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "userActivationCounts": [{"@odata.type":"microsoft.graph.userActivationCounts"}]
}
```
