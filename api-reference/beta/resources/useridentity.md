---
title: Typ der Benutzeridentität
description: 'Für die Azure AD zugreifen Reviews (engl.), diesen Typ eine Benutzeridentität Azure AD für Bearbeiter die Überprüfung einer Access darstellt.  '
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ab8076c5ff24e20006b5a5569dacf4c45d987512
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529467"
---
# <a name="useridentity-type"></a><span data-ttu-id="7caf4-103">Typ der Benutzeridentität</span><span class="sxs-lookup"><span data-stu-id="7caf4-103">userIdentity type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7caf4-104">Für die Azure AD, [Access überprüft](accessreviews-root.md)ist stellt dieses Typs eine Benutzeridentität Azure AD eines Bearbeiters eines Access-Überprüfung.</span><span class="sxs-lookup"><span data-stu-id="7caf4-104">For the Azure AD [access reviews](accessreviews-root.md), this type represents an Azure AD user identity for a reviewer of an access review.</span></span>  
<span data-ttu-id="7caf4-105">Im Zusammenhang mit einer Azure AD-Überwachungsprotokoll stellt dies die Benutzerinformationen, die initiiert oder durch eine Aktivität Audit betroffen war.</span><span class="sxs-lookup"><span data-stu-id="7caf4-105">In the context of an Azure AD audit log, this represents the user information that initiated or was affected by an audit activity.</span></span>

<span data-ttu-id="7caf4-106">Dieser Typ erbt von [Identität](identity.md) und verfügt über eine zusätzliche Eigenschaft, den Benutzerprinzipalnamen des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="7caf4-106">This type inherits from [identity](identity.md) and has one additional property, the user principal name of the user.</span></span>

## <a name="methods"></a><span data-ttu-id="7caf4-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="7caf4-107">Methods</span></span>

<span data-ttu-id="7caf4-108">Keine.</span><span class="sxs-lookup"><span data-stu-id="7caf4-108">None.</span></span>  <span data-ttu-id="7caf4-109">Schließen Sie Objekte dieses Typs im Textkörper einer Anforderung beim [Erstellen einer AccessReview](../api/accessreview-create.md).</span><span class="sxs-lookup"><span data-stu-id="7caf4-109">You would include objects of this type in the body of a request when [creating an accessReview](../api/accessreview-create.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7caf4-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7caf4-110">Properties</span></span>
| <span data-ttu-id="7caf4-111">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7caf4-111">Property</span></span>     | <span data-ttu-id="7caf4-112">Typ</span><span class="sxs-lookup"><span data-stu-id="7caf4-112">Type</span></span>   |<span data-ttu-id="7caf4-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7caf4-113">Description</span></span>|
|:---------------|:--------|:----------|
| `displayName` | `String` | <span data-ttu-id="7caf4-114">Die Identität der Anzeigename.</span><span class="sxs-lookup"><span data-stu-id="7caf4-114">The identity's display name.</span></span> <span data-ttu-id="7caf4-115">Beachten Sie, dass dies möglicherweise nicht immer verfügbar oder auf dem neuesten Stand.</span><span class="sxs-lookup"><span data-stu-id="7caf4-115">Note that this may not always be available or up-to-date.</span></span>    |
| `id`          | `String` | <span data-ttu-id="7caf4-116">Eindeutiger Bezeichner für die Identität.</span><span class="sxs-lookup"><span data-stu-id="7caf4-116">Unique identifier for the identity.</span></span>  |
| `ipAddress`| `String`| <span data-ttu-id="7caf4-117">Gibt an, die Client-IP-Adresse von Benutzer, die Ausführung der Aktivität (nur Audit Log) verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="7caf4-117">Indicates the client IP address used by user performing the activity (audit log only).</span></span>|
| `userPrincipalName`|`String` | <span data-ttu-id="7caf4-118">Das UserPrincipalName-Attribut des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="7caf4-118">The userPrincipalName attribute of the user.</span></span> |

## <a name="remarks"></a><span data-ttu-id="7caf4-119">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="7caf4-119">Remarks</span></span>

<span data-ttu-id="7caf4-p103">Unter gewissen Umständen steht der eindeutige Bezeichner für den Akteur möglicherweise nicht zur Verfügung. In diesem Fall die wird die Eigenschaft **DisplayName** für die Identität zurückgegeben werden, aber die **Id**-Eigenschaft ist aus der Ressource nicht vorhanden.</span><span class="sxs-lookup"><span data-stu-id="7caf4-p103">In some circumstances, the unique identifier for the actor may not be available. In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

## <a name="relationships"></a><span data-ttu-id="7caf4-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7caf4-122">Relationships</span></span>

<span data-ttu-id="7caf4-123">None.</span><span class="sxs-lookup"><span data-stu-id="7caf4-123">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="7caf4-124">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="7caf4-124">See also</span></span>

| <span data-ttu-id="7caf4-125">Methode</span><span class="sxs-lookup"><span data-stu-id="7caf4-125">Method</span></span>           | <span data-ttu-id="7caf4-126">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="7caf4-126">Return Type</span></span>    |<span data-ttu-id="7caf4-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7caf4-127">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7caf4-128">Abrufen von AccessReview Bearbeiter</span><span class="sxs-lookup"><span data-stu-id="7caf4-128">Get accessReview reviewers</span></span>](../api/accessreview-listreviewers.md) |       <span data-ttu-id="7caf4-129">[Benutzeridentität](useridentity.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="7caf4-129">[userIdentity](useridentity.md) collection</span></span>| <span data-ttu-id="7caf4-130">Rufen Sie die Bearbeiter ein AccessReview.</span><span class="sxs-lookup"><span data-stu-id="7caf4-130">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="7caf4-131">AccessReview Bearbeiter hinzufügen</span><span class="sxs-lookup"><span data-stu-id="7caf4-131">Add accessReview reviewer</span></span>](../api/accessreview-addreviewer.md) |      <span data-ttu-id="7caf4-132">Keine.</span><span class="sxs-lookup"><span data-stu-id="7caf4-132">None.</span></span>   |   <span data-ttu-id="7caf4-133">Fügen Sie einem Bearbeiter ein AccessReview hinzu.</span><span class="sxs-lookup"><span data-stu-id="7caf4-133">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="7caf4-134">AccessReview Reviewer entfernen</span><span class="sxs-lookup"><span data-stu-id="7caf4-134">Remove accessReview reviewer</span></span>](../api/accessreview-removereviewer.md) | <span data-ttu-id="7caf4-135">Keine.</span><span class="sxs-lookup"><span data-stu-id="7caf4-135">None.</span></span>  |   <span data-ttu-id="7caf4-136">Entfernen Sie einen Prüfer aus einer AccessReview.</span><span class="sxs-lookup"><span data-stu-id="7caf4-136">Remove a reviewer from an accessReview.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7caf4-137">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7caf4-137">JSON representation</span></span>

<span data-ttu-id="7caf4-138">Es folgt eine JSON-Darstellung des Typs.</span><span class="sxs-lookup"><span data-stu-id="7caf4-138">Here is a JSON representation of the type.</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "userIdentity type",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/useridentity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
