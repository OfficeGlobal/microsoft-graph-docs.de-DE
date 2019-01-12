---
title: Typ der Benutzeridentität
description: 'Für die Azure AD zugreifen Reviews (engl.), diesen Typ eine Benutzeridentität Azure AD für Bearbeiter die Überprüfung einer Access darstellt.  '
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 80e8cc68d4fc2f642be6c748b762fe47c7489d59
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932280"
---
# <a name="useridentity-type"></a><span data-ttu-id="ae015-103">Typ der Benutzeridentität</span><span class="sxs-lookup"><span data-stu-id="ae015-103">userIdentity type</span></span>

> <span data-ttu-id="ae015-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ae015-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ae015-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ae015-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ae015-106">Für die Azure AD, [Access überprüft](accessreviews-root.md)ist stellt dieses Typs eine Benutzeridentität Azure AD eines Bearbeiters eines Access-Überprüfung.</span><span class="sxs-lookup"><span data-stu-id="ae015-106">For the Azure AD [access reviews](accessreviews-root.md), this type represents an Azure AD user identity for a reviewer of an access review.</span></span>  
<span data-ttu-id="ae015-107">Im Zusammenhang mit einer Azure AD-Überwachungsprotokoll stellt dies die Benutzerinformationen, die initiiert oder durch eine Aktivität Audit betroffen war.</span><span class="sxs-lookup"><span data-stu-id="ae015-107">In the context of an Azure AD audit log, this represents the user information that initiated or was affected by an audit activity.</span></span>

<span data-ttu-id="ae015-108">Dieser Typ erbt von [Identität](identity.md) und verfügt über eine zusätzliche Eigenschaft, den Benutzerprinzipalnamen des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="ae015-108">This type inherits from [identity](identity.md) and has one additional property, the user principal name of the user.</span></span>

## <a name="methods"></a><span data-ttu-id="ae015-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="ae015-109">Methods</span></span>

<span data-ttu-id="ae015-110">Keine.</span><span class="sxs-lookup"><span data-stu-id="ae015-110">None.</span></span>  <span data-ttu-id="ae015-111">Schließen Sie Objekte dieses Typs im Textkörper einer Anforderung beim [Erstellen einer AccessReview](../api/accessreview-create.md).</span><span class="sxs-lookup"><span data-stu-id="ae015-111">You would include objects of this type in the body of a request when [creating an accessReview](../api/accessreview-create.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ae015-112">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ae015-112">Properties</span></span>
| <span data-ttu-id="ae015-113">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ae015-113">Property</span></span>     | <span data-ttu-id="ae015-114">Typ</span><span class="sxs-lookup"><span data-stu-id="ae015-114">Type</span></span>   |<span data-ttu-id="ae015-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ae015-115">Description</span></span>|
|:---------------|:--------|:----------|
| `displayName` | `String` | <span data-ttu-id="ae015-116">Die Identität der Anzeigename.</span><span class="sxs-lookup"><span data-stu-id="ae015-116">The identity's display name.</span></span> <span data-ttu-id="ae015-117">Beachten Sie, dass dies möglicherweise nicht immer verfügbar oder auf dem neuesten Stand.</span><span class="sxs-lookup"><span data-stu-id="ae015-117">Note that this may not always be available or up-to-date.</span></span>    |
| `id`          | `String` | <span data-ttu-id="ae015-118">Eindeutiger Bezeichner für die Identität.</span><span class="sxs-lookup"><span data-stu-id="ae015-118">Unique identifier for the identity.</span></span>  |
| `ipAddress`| `String`| <span data-ttu-id="ae015-119">Gibt an, die Client-IP-Adresse von Benutzer, die Ausführung der Aktivität (nur Audit Log) verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="ae015-119">Indicates the client IP address used by user performing the activity (audit log only).</span></span>|
| `userPrincipalName`|`String` | <span data-ttu-id="ae015-120">Das UserPrincipalName-Attribut des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="ae015-120">The userPrincipalName attribute of the user.</span></span> |

## <a name="remarks"></a><span data-ttu-id="ae015-121">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="ae015-121">Remarks</span></span>

<span data-ttu-id="ae015-p104">Unter gewissen Umständen steht der eindeutige Bezeichner für den Akteur möglicherweise nicht zur Verfügung. In diesem Fall die wird die Eigenschaft **DisplayName** für die Identität zurückgegeben werden, aber die **Id**-Eigenschaft ist aus der Ressource nicht vorhanden.</span><span class="sxs-lookup"><span data-stu-id="ae015-p104">In some circumstances, the unique identifier for the actor may not be available. In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

## <a name="relationships"></a><span data-ttu-id="ae015-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ae015-124">Relationships</span></span>

<span data-ttu-id="ae015-125">Keine.</span><span class="sxs-lookup"><span data-stu-id="ae015-125">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="ae015-126">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="ae015-126">See also</span></span>

| <span data-ttu-id="ae015-127">Methode</span><span class="sxs-lookup"><span data-stu-id="ae015-127">Method</span></span>           | <span data-ttu-id="ae015-128">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="ae015-128">Return Type</span></span>    |<span data-ttu-id="ae015-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ae015-129">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ae015-130">Abrufen von AccessReview Bearbeiter</span><span class="sxs-lookup"><span data-stu-id="ae015-130">Get accessReview reviewers</span></span>](../api/accessreview-listreviewers.md) |       <span data-ttu-id="ae015-131">[Benutzeridentität](useridentity.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="ae015-131">[userIdentity](useridentity.md) collection</span></span>| <span data-ttu-id="ae015-132">Rufen Sie die Bearbeiter ein AccessReview.</span><span class="sxs-lookup"><span data-stu-id="ae015-132">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="ae015-133">AccessReview Bearbeiter hinzufügen</span><span class="sxs-lookup"><span data-stu-id="ae015-133">Add accessReview reviewer</span></span>](../api/accessreview-addreviewer.md) |      <span data-ttu-id="ae015-134">Keine.</span><span class="sxs-lookup"><span data-stu-id="ae015-134">None.</span></span>   |   <span data-ttu-id="ae015-135">Fügen Sie einem Bearbeiter ein AccessReview hinzu.</span><span class="sxs-lookup"><span data-stu-id="ae015-135">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="ae015-136">AccessReview Reviewer entfernen</span><span class="sxs-lookup"><span data-stu-id="ae015-136">Remove accessReview reviewer</span></span>](../api/accessreview-removereviewer.md) | <span data-ttu-id="ae015-137">Keine.</span><span class="sxs-lookup"><span data-stu-id="ae015-137">None.</span></span>  |   <span data-ttu-id="ae015-138">Entfernen Sie einen Prüfer aus einer AccessReview.</span><span class="sxs-lookup"><span data-stu-id="ae015-138">Remove a reviewer from an accessReview.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ae015-139">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ae015-139">JSON representation</span></span>

<span data-ttu-id="ae015-140">Es folgt eine JSON-Darstellung des Typs.</span><span class="sxs-lookup"><span data-stu-id="ae015-140">Here is a JSON representation of the type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
"displayName", "thumbnails"
  ],
  "@odata.type": "microsoft.graph.userIdentity"
}-->

```json
{
  "displayName": "string",
  "id": "string",
 "userPrincipalName": "String"
}

```

<!-- {
  "type": "#page.annotation",
  "description": "userIdentity type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
