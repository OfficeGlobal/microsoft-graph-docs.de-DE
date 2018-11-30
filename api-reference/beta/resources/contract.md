---
title: Contract-Ressourcentyp
description: Stellt eine bestehende Partnerschaft zwischen dem Partnermandanten und einem Kundenmandanten dar.
ms.openlocfilehash: 7465a54c735b7c1e6f9d5ecb8bf79420b8de45c3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065340"
---
# <a name="contract-resource-type"></a><span data-ttu-id="9c7b2-103">Contract-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9c7b2-103">Contract resource type</span></span>

> <span data-ttu-id="9c7b2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9c7b2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9c7b2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9c7b2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9c7b2-106">Stellt eine bestehende Partnerschaft zwischen dem Partnermandanten und einem Kundenmandanten dar.</span><span class="sxs-lookup"><span data-stu-id="9c7b2-106">Represents an existing partnership that the partner tenant has with a customer tenant.</span></span>

> <span data-ttu-id="9c7b2-p102">**Wichtig:** Ist nur in Partnermandanten vorhanden. Partnermandanten sind Azure AD-Mandanten, die zu Microsoft-Partnern gehören, die Teil der Partnerprogramme [Microsoft Cloud-Lösungsanbieter](https://partnercenter.microsoft.com/en-us/partner/programs), Office 365 Syndication oder Microsoft Advisor sind.</span><span class="sxs-lookup"><span data-stu-id="9c7b2-p102">**Important:** Exists in partner tenants only. Partner tenants are Azure AD tenants that belong to Microsoft partners who are either part of [Microsoft Cloud Solution Provider](https://partnercenter.microsoft.com/en-us/partner/programs), Office 365 Syndication, or Microsoft Advisor partner programs.</span></span>

## <a name="methods"></a><span data-ttu-id="9c7b2-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="9c7b2-109">Methods</span></span>

| <span data-ttu-id="9c7b2-110">Methode</span><span class="sxs-lookup"><span data-stu-id="9c7b2-110">Method</span></span>   | <span data-ttu-id="9c7b2-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="9c7b2-111">Return Type</span></span> | <span data-ttu-id="9c7b2-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9c7b2-112">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="9c7b2-113">Vertrag abrufen</span><span class="sxs-lookup"><span data-stu-id="9c7b2-113">Get contract</span></span>](../api/contract-get.md) | <span data-ttu-id="9c7b2-114">Contract</span><span class="sxs-lookup"><span data-stu-id="9c7b2-114">Contract</span></span> |<span data-ttu-id="9c7b2-115">Dient zum Lesen der Eigenschaften eines bestimmten Vertragsobjekts.</span><span class="sxs-lookup"><span data-stu-id="9c7b2-115">Read properties of a specific contract object.</span></span> |
|[<span data-ttu-id="9c7b2-116">Verträge auflisten</span><span class="sxs-lookup"><span data-stu-id="9c7b2-116">List contracts</span></span>](../api/contract-list.md) | <span data-ttu-id="9c7b2-117">Contract-Sammlung</span><span class="sxs-lookup"><span data-stu-id="9c7b2-117">Contract collection</span></span> | <span data-ttu-id="9c7b2-118">Liste der Verträge im Partnermandanten.</span><span class="sxs-lookup"><span data-stu-id="9c7b2-118">List of contracts in the partner tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="9c7b2-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9c7b2-119">Properties</span></span>
| <span data-ttu-id="9c7b2-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9c7b2-120">Property</span></span>   | <span data-ttu-id="9c7b2-121">Typ</span><span class="sxs-lookup"><span data-stu-id="9c7b2-121">Type</span></span> | <span data-ttu-id="9c7b2-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9c7b2-122">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="9c7b2-123">contractType</span><span class="sxs-lookup"><span data-stu-id="9c7b2-123">contractType</span></span>|<span data-ttu-id="9c7b2-124">String</span><span class="sxs-lookup"><span data-stu-id="9c7b2-124">String</span></span>|<span data-ttu-id="9c7b2-125">Typ des Vertrags.</span><span class="sxs-lookup"><span data-stu-id="9c7b2-125">Type of contract.</span></span><br><br><span data-ttu-id="9c7b2-126">Die folgenden Werte sind möglich:</span><span class="sxs-lookup"><span data-stu-id="9c7b2-126">Possible values are:</span></span><br> <span data-ttu-id="9c7b2-p103">*SyndicationPartner*: Partner, der Office 365 und Intune exklusiv für diesen Kunden verkauft und verwaltet. Die Partner verkaufen und erbringen Supportleistungen für ihre Kunden.</span><span class="sxs-lookup"><span data-stu-id="9c7b2-p103">*SyndicationPartner* - Partner that exclusively resells and manages O365 and Intune for this customer. They resell and support their customers.</span></span><br> <span data-ttu-id="9c7b2-p104">*BreadthPartner*: Partner, der administrative Unterstützung für diesen Kunden bereitstellen kann. Der Partner darf jedoch nicht an den Kunden verkaufen.</span><span class="sxs-lookup"><span data-stu-id="9c7b2-p104">*BreadthPartner* - Partner has the ability to provide administrative support for this customer. However, the partner is not allowed to resell to the customer.</span></span><br><span data-ttu-id="9c7b2-p105">*ResellerPartner*: Ähnlicher Partner wie Syndication-Partner, mit der Ausnahme, dass der Partner keinen exklusiven Zugriff auf einen Mandanten hat. Im Syndication-Fall kann der Kunde keine zusätzlichen direkten Abonnements von Microsoft oder von anderen Partnern kaufen.</span><span class="sxs-lookup"><span data-stu-id="9c7b2-p105">*ResellerPartner* - Partner that is similar to a syndication partner, except that the partner doesn’t have exclusive access to a tenant. In the syndication case, the customer cannot buy additional direct subscriptions from Microsoft or from other partners.</span></span>|
|<span data-ttu-id="9c7b2-133">customerId</span><span class="sxs-lookup"><span data-stu-id="9c7b2-133">customerId</span></span>|<span data-ttu-id="9c7b2-134">Guid</span><span class="sxs-lookup"><span data-stu-id="9c7b2-134">Guid</span></span>|<span data-ttu-id="9c7b2-p106">Der eindeutige Bezeichner für den Kundenmandanten, auf den in dieser Partnerschaft verwiesen wird. Entspricht der id-Eigenschaft der organization-Ressource des Kundenmandanten.</span><span class="sxs-lookup"><span data-stu-id="9c7b2-p106">The unique identifier for the customer tenant referenced by this partnership. Corresponds to the id property of the customer tenant's organization resource.</span></span> |
|<span data-ttu-id="9c7b2-137">defaultDomainName</span><span class="sxs-lookup"><span data-stu-id="9c7b2-137">defaultDomainName</span></span>|<span data-ttu-id="9c7b2-138">String</span><span class="sxs-lookup"><span data-stu-id="9c7b2-138">String</span></span>|<span data-ttu-id="9c7b2-p107">Eine Kopie des Standarddomänennamens des Kundenmandanten. Die Kopie wird erstellt, wenn die Partnerschaft mit dem Kunden eingerichtet wird. Sie wird nicht automatisch aktualisiert, wenn sich der Standarddomänenname des Kundenmandanten ändert.</span><span class="sxs-lookup"><span data-stu-id="9c7b2-p107">A copy of the customer tenant's default domain name. The copy is made when the partnership with the customer is established. It is not automatically updated if the customer tenant's default domain name changes.</span></span>|
|<span data-ttu-id="9c7b2-142">displayName</span><span class="sxs-lookup"><span data-stu-id="9c7b2-142">displayName</span></span>|<span data-ttu-id="9c7b2-143">String</span><span class="sxs-lookup"><span data-stu-id="9c7b2-143">String</span></span>|<span data-ttu-id="9c7b2-p108">Eine Kopie des Anzeigenamens des Kundenmandanten. Die Kopie wird erstellt, wenn die Partnerschaft mit dem Kunden eingerichtet wird. Sie wird nicht automatisch aktualisiert, wenn sich der Anzeigenname des Kundenmandanten ändert.</span><span class="sxs-lookup"><span data-stu-id="9c7b2-p108">A copy of the customer tenant's display name. The copy is made when the partnership with the customer is established. It is not automatically updated if the customer tenant's display name changes.</span></span>|
|<span data-ttu-id="9c7b2-147">id</span><span class="sxs-lookup"><span data-stu-id="9c7b2-147">id</span></span>|<span data-ttu-id="9c7b2-148">String</span><span class="sxs-lookup"><span data-stu-id="9c7b2-148">String</span></span>| <span data-ttu-id="9c7b2-p109">Der eindeutige Bezeichner für die Partnerschaft. Schlüssel, schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9c7b2-p109">The unique identifier for the partnership. Key, read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="9c7b2-151">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9c7b2-151">Relationships</span></span>
<span data-ttu-id="9c7b2-152">Keine</span><span class="sxs-lookup"><span data-stu-id="9c7b2-152">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9c7b2-153">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9c7b2-153">JSON representation</span></span>
<span data-ttu-id="9c7b2-154">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9c7b2-154">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.Contract"
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