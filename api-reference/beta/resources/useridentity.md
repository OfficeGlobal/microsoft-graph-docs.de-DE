---
title: Typ der Benutzeridentität
description: 'Für die Azure AD zugreifen Reviews (engl.), diesen Typ eine Benutzeridentität Azure AD für Bearbeiter die Überprüfung einer Access darstellt.  '
localization_priority: Normal
ms.openlocfilehash: 5b629fff4c5cecd513777cc5004646aac5f1c85b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839641"
---
# <a name="useridentity-type"></a><span data-ttu-id="cff23-103">Typ der Benutzeridentität</span><span class="sxs-lookup"><span data-stu-id="cff23-103">userIdentity type</span></span>

> <span data-ttu-id="cff23-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="cff23-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cff23-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cff23-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cff23-106">Für die Azure AD, [Access überprüft](accessreviews-root.md)ist stellt dieses Typs eine Benutzeridentität Azure AD eines Bearbeiters eines Access-Überprüfung.</span><span class="sxs-lookup"><span data-stu-id="cff23-106">For the Azure AD [access reviews](accessreviews-root.md), this type represents an Azure AD user identity for a reviewer of an access review.</span></span>  
<span data-ttu-id="cff23-107">Im Zusammenhang mit einer Azure AD-Überwachungsprotokoll stellt dies die Benutzerinformationen, die initiiert oder durch eine Aktivität Audit betroffen war.</span><span class="sxs-lookup"><span data-stu-id="cff23-107">In the context of an Azure AD audit log, this represents the user information that initiated or was affected by an audit activity.</span></span>

<span data-ttu-id="cff23-108">Dieser Typ erbt von [Identität](identity.md) und verfügt über eine zusätzliche Eigenschaft, den Benutzerprinzipalnamen des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="cff23-108">This type inherits from [identity](identity.md) and has one additional property, the user principal name of the user.</span></span>

## <a name="methods"></a><span data-ttu-id="cff23-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="cff23-109">Methods</span></span>

<span data-ttu-id="cff23-110">Keine.</span><span class="sxs-lookup"><span data-stu-id="cff23-110">None.</span></span>  <span data-ttu-id="cff23-111">Schließen Sie Objekte dieses Typs im Textkörper einer Anforderung beim [Erstellen einer AccessReview](../api/accessreview-create.md).</span><span class="sxs-lookup"><span data-stu-id="cff23-111">You would include objects of this type in the body of a request when [creating an accessReview](../api/accessreview-create.md).</span></span>

## <a name="properties"></a><span data-ttu-id="cff23-112">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="cff23-112">Properties</span></span>
| <span data-ttu-id="cff23-113">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cff23-113">Property</span></span>     | <span data-ttu-id="cff23-114">Typ</span><span class="sxs-lookup"><span data-stu-id="cff23-114">Type</span></span>   |<span data-ttu-id="cff23-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cff23-115">Description</span></span>|
|:---------------|:--------|:----------|
| `displayName` | `String` | <span data-ttu-id="cff23-116">Die Identität der Anzeigename.</span><span class="sxs-lookup"><span data-stu-id="cff23-116">The identity's display name.</span></span> <span data-ttu-id="cff23-117">Beachten Sie, dass dies möglicherweise nicht immer verfügbar oder auf dem neuesten Stand.</span><span class="sxs-lookup"><span data-stu-id="cff23-117">Note that this may not always be available or up-to-date.</span></span>    |
| `id`          | `String` | <span data-ttu-id="cff23-118">Eindeutiger Bezeichner für die Identität.</span><span class="sxs-lookup"><span data-stu-id="cff23-118">Unique identifier for the identity.</span></span>  |
| `ipAddress`| `String`| <span data-ttu-id="cff23-119">Gibt an, die Client-IP-Adresse von Benutzer, die Ausführung der Aktivität (nur Audit Log) verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="cff23-119">Indicates the client IP address used by user performing the activity (audit log only).</span></span>|
| `userPrincipalName`|`String` | <span data-ttu-id="cff23-120">Das UserPrincipalName-Attribut des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="cff23-120">The userPrincipalName attribute of the user.</span></span> |

## <a name="remarks"></a><span data-ttu-id="cff23-121">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="cff23-121">Remarks</span></span>

<span data-ttu-id="cff23-p104">Unter gewissen Umständen steht der eindeutige Bezeichner für den Akteur möglicherweise nicht zur Verfügung. In diesem Fall die wird die Eigenschaft **DisplayName** für die Identität zurückgegeben werden, aber die **Id**-Eigenschaft ist aus der Ressource nicht vorhanden.</span><span class="sxs-lookup"><span data-stu-id="cff23-p104">In some circumstances, the unique identifier for the actor may not be available. In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

## <a name="relationships"></a><span data-ttu-id="cff23-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="cff23-124">Relationships</span></span>

<span data-ttu-id="cff23-125">Keine.</span><span class="sxs-lookup"><span data-stu-id="cff23-125">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="cff23-126">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="cff23-126">See also</span></span>

| <span data-ttu-id="cff23-127">Methode</span><span class="sxs-lookup"><span data-stu-id="cff23-127">Method</span></span>           | <span data-ttu-id="cff23-128">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="cff23-128">Return Type</span></span>    |<span data-ttu-id="cff23-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cff23-129">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cff23-130">Abrufen von AccessReview Bearbeiter</span><span class="sxs-lookup"><span data-stu-id="cff23-130">Get accessReview reviewers</span></span>](../api/accessreview-listreviewers.md) |       <span data-ttu-id="cff23-131">[Benutzeridentität](useridentity.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="cff23-131">[userIdentity](useridentity.md) collection</span></span>| <span data-ttu-id="cff23-132">Rufen Sie die Bearbeiter ein AccessReview.</span><span class="sxs-lookup"><span data-stu-id="cff23-132">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="cff23-133">AccessReview Bearbeiter hinzufügen</span><span class="sxs-lookup"><span data-stu-id="cff23-133">Add accessReview reviewer</span></span>](../api/accessreview-addreviewer.md) |      <span data-ttu-id="cff23-134">Keine.</span><span class="sxs-lookup"><span data-stu-id="cff23-134">None.</span></span>   |   <span data-ttu-id="cff23-135">Fügen Sie einem Bearbeiter ein AccessReview hinzu.</span><span class="sxs-lookup"><span data-stu-id="cff23-135">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="cff23-136">AccessReview Reviewer entfernen</span><span class="sxs-lookup"><span data-stu-id="cff23-136">Remove accessReview reviewer</span></span>](../api/accessreview-removereviewer.md) | <span data-ttu-id="cff23-137">Keine.</span><span class="sxs-lookup"><span data-stu-id="cff23-137">None.</span></span>  |   <span data-ttu-id="cff23-138">Entfernen Sie einen Prüfer aus einer AccessReview.</span><span class="sxs-lookup"><span data-stu-id="cff23-138">Remove a reviewer from an accessReview.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cff23-139">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="cff23-139">JSON representation</span></span>

<span data-ttu-id="cff23-140">Es folgt eine JSON-Darstellung des Typs.</span><span class="sxs-lookup"><span data-stu-id="cff23-140">Here is a JSON representation of the type.</span></span>

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
