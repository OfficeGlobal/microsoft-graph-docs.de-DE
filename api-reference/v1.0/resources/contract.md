---
title: Contract-Ressourcentyp
description: Stellt eine bestehende Partnerschaft zwischen dem Partnermandanten und einem Kundenmandanten dar.
localization_priority: Normal
ms.openlocfilehash: c14f4a51cbab5625c16ef0f0e515fffd35619366
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812299"
---
# <a name="contract-resource-type"></a><span data-ttu-id="cf567-103">Contract-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="cf567-103">Contract resource type</span></span>
<span data-ttu-id="cf567-104">Stellt eine bestehende Partnerschaft zwischen dem Partnermandanten und einem Kundenmandanten dar.</span><span class="sxs-lookup"><span data-stu-id="cf567-104">Represents an existing partnership that the partner tenant has with a customer tenant.</span></span>

> <span data-ttu-id="cf567-p101">**Wichtig:** Ist nur in Partnermandanten vorhanden. Partnermandanten sind Azure AD-Mandanten, die zu Microsoft-Partnern gehören, die Teil der Partnerprogramme [Microsoft Cloud-Lösungsanbieter](https://partnercenter.microsoft.com/en-us/partner/programs), Office 365 Syndication oder Microsoft Advisor sind.</span><span class="sxs-lookup"><span data-stu-id="cf567-p101">**Important:** Exists in partner tenants only. Partner tenants are Azure AD tenants that belong to Microsoft partners who are either part of [Microsoft Cloud Solution Provider](https://partnercenter.microsoft.com/en-us/partner/programs), Office 365 Syndication, or Microsoft Advisor partner programs.</span></span>

## <a name="methods"></a><span data-ttu-id="cf567-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="cf567-107">Methods</span></span>

| <span data-ttu-id="cf567-108">Methode</span><span class="sxs-lookup"><span data-stu-id="cf567-108">Method</span></span>   | <span data-ttu-id="cf567-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="cf567-109">Return Type</span></span> | <span data-ttu-id="cf567-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cf567-110">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="cf567-111">Vertrag abrufen</span><span class="sxs-lookup"><span data-stu-id="cf567-111">Get contract</span></span>](../api/contract-get.md) | <span data-ttu-id="cf567-112">Contract</span><span class="sxs-lookup"><span data-stu-id="cf567-112">Contract</span></span> |<span data-ttu-id="cf567-113">Dient zum Lesen der Eigenschaften eines bestimmten Vertragsobjekts.</span><span class="sxs-lookup"><span data-stu-id="cf567-113">Read properties of a specific contract object.</span></span> |
|[<span data-ttu-id="cf567-114">Verträge auflisten</span><span class="sxs-lookup"><span data-stu-id="cf567-114">List contracts</span></span>](../api/contract-list.md) | <span data-ttu-id="cf567-115">Contract-Sammlung</span><span class="sxs-lookup"><span data-stu-id="cf567-115">Contract collection</span></span> | <span data-ttu-id="cf567-116">Liste der Verträge im Partnermandanten.</span><span class="sxs-lookup"><span data-stu-id="cf567-116">List of contracts in the partner tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="cf567-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="cf567-117">Properties</span></span>
| <span data-ttu-id="cf567-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cf567-118">Property</span></span>   | <span data-ttu-id="cf567-119">Typ</span><span class="sxs-lookup"><span data-stu-id="cf567-119">Type</span></span> | <span data-ttu-id="cf567-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cf567-120">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="cf567-121">contractType</span><span class="sxs-lookup"><span data-stu-id="cf567-121">contractType</span></span>|<span data-ttu-id="cf567-122">String</span><span class="sxs-lookup"><span data-stu-id="cf567-122">String</span></span>|<span data-ttu-id="cf567-123">Typ des Vertrags.</span><span class="sxs-lookup"><span data-stu-id="cf567-123">Type of contract.</span></span><br><br><span data-ttu-id="cf567-124">Die folgenden Werte sind möglich:</span><span class="sxs-lookup"><span data-stu-id="cf567-124">Possible values are:</span></span><br> <span data-ttu-id="cf567-p102">*SyndicationPartner*: Partner, der Office 365 und Intune exklusiv für diesen Kunden verkauft und verwaltet. Die Partner verkaufen und erbringen Supportleistungen für ihre Kunden.</span><span class="sxs-lookup"><span data-stu-id="cf567-p102">*SyndicationPartner* - Partner that exclusively resells and manages O365 and Intune for this customer. They resell and support their customers.</span></span><br> <span data-ttu-id="cf567-p103">*BreadthPartner*: Partner, der administrative Unterstützung für diesen Kunden bereitstellen kann. Der Partner darf jedoch nicht an den Kunden verkaufen.</span><span class="sxs-lookup"><span data-stu-id="cf567-p103">*BreadthPartner* - Partner has the ability to provide administrative support for this customer. However, the partner is not allowed to resell to the customer.</span></span><br><span data-ttu-id="cf567-p104">*ResellerPartner*: Ähnlicher Partner wie Syndication-Partner, mit der Ausnahme, dass der Partner keinen exklusiven Zugriff auf einen Mandanten hat. Im Syndication-Fall kann der Kunde keine zusätzlichen direkten Abonnements von Microsoft oder von anderen Partnern kaufen.</span><span class="sxs-lookup"><span data-stu-id="cf567-p104">*ResellerPartner* - Partner that is similar to a syndication partner, except that the partner doesn’t have exclusive access to a tenant. In the syndication case, the customer cannot buy additional direct subscriptions from Microsoft or from other partners.</span></span>|
|<span data-ttu-id="cf567-131">customerId</span><span class="sxs-lookup"><span data-stu-id="cf567-131">customerId</span></span>|<span data-ttu-id="cf567-132">Guid</span><span class="sxs-lookup"><span data-stu-id="cf567-132">Guid</span></span>|<span data-ttu-id="cf567-p105">Der eindeutige Bezeichner für den Kundenmandanten, auf den in dieser Partnerschaft verwiesen wird. Entspricht der id-Eigenschaft der organization-Ressource des Kundenmandanten.</span><span class="sxs-lookup"><span data-stu-id="cf567-p105">The unique identifier for the customer tenant referenced by this partnership. Corresponds to the id property of the customer tenant's organization resource.</span></span> |
|<span data-ttu-id="cf567-135">defaultDomainName</span><span class="sxs-lookup"><span data-stu-id="cf567-135">defaultDomainName</span></span>|<span data-ttu-id="cf567-136">String</span><span class="sxs-lookup"><span data-stu-id="cf567-136">String</span></span>|<span data-ttu-id="cf567-p106">Eine Kopie des Standarddomänennamens des Kundenmandanten. Die Kopie wird erstellt, wenn die Partnerschaft mit dem Kunden eingerichtet wird. Sie wird nicht automatisch aktualisiert, wenn sich der Standarddomänenname des Kundenmandanten ändert.</span><span class="sxs-lookup"><span data-stu-id="cf567-p106">A copy of the customer tenant's default domain name. The copy is made when the partnership with the customer is established. It is not automatically updated if the customer tenant's default domain name changes.</span></span>|
|<span data-ttu-id="cf567-140">displayName</span><span class="sxs-lookup"><span data-stu-id="cf567-140">displayName</span></span>|<span data-ttu-id="cf567-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cf567-141">String</span></span>|<span data-ttu-id="cf567-p107">Eine Kopie des Anzeigenamens des Kundenmandanten. Die Kopie wird erstellt, wenn die Partnerschaft mit dem Kunden eingerichtet wird. Sie wird nicht automatisch aktualisiert, wenn sich der Anzeigenname des Kundenmandanten ändert.</span><span class="sxs-lookup"><span data-stu-id="cf567-p107">A copy of the customer tenant's display name. The copy is made when the partnership with the customer is established. It is not automatically updated if the customer tenant's display name changes.</span></span>|
|<span data-ttu-id="cf567-145">id</span><span class="sxs-lookup"><span data-stu-id="cf567-145">id</span></span>|<span data-ttu-id="cf567-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cf567-146">String</span></span>| <span data-ttu-id="cf567-p108">Der eindeutige Bezeichner für die Partnerschaft. Schlüssel, schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="cf567-p108">The unique identifier for the partnership. Key, read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="cf567-149">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="cf567-149">Relationships</span></span>
<span data-ttu-id="cf567-150">Keine</span><span class="sxs-lookup"><span data-stu-id="cf567-150">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="cf567-151">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="cf567-151">JSON representation</span></span>
<span data-ttu-id="cf567-152">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="cf567-152">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.contract"
}-->

```json
{
  "contractType": "String",
  "customerId": "Guid",
  "defaultDomainName": "String",
  "displayName": "String",
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Contract resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
