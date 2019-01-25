---
title: Ressourcentyp accessReviewDecision
description: In Azure AD Access Feature, überprüft die `accessReviewDecision` eine Azure AD Access Treffen einer Entscheidung anhand des Zugriffs für eine bestimmte Entität darstellt.  In einer Access-Überprüfung oder eine Instanz einer wiederkehrenden Access Überprüfung, ist eine `accessReviewDecision` pro überprüfter Benutzer.  Beispielsweise eine Gruppe besitzt zwei Gäste und einen anderen Typ als Mitglieder und einer Access-Überprüfung von Gästen für diese Gruppe erfolgt dann zwei Access überprüfen Entscheidung-Objekte werden.  Wenn ein Bearbeiter ihre Entscheidung ändert oder einen anderen Prüfer diese überschreibt, und klicken Sie dann die `accessReviewDecision` wird aktualisiert.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9642c8a51e4e9efe1a1748243b0e24aeff07cfa0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517400"
---
# <a name="accessreviewdecision-resource-type"></a><span data-ttu-id="c91fd-106">Ressourcentyp accessReviewDecision</span><span class="sxs-lookup"><span data-stu-id="c91fd-106">accessReviewDecision resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c91fd-107">In der Azure AD [Access überprüft](accessreviews-root.md) -Funktion die `accessReviewDecision` eine Azure AD Access Treffen einer Entscheidung anhand des Zugriffs für eine bestimmte Entität darstellt.</span><span class="sxs-lookup"><span data-stu-id="c91fd-107">In the Azure AD [access reviews](accessreviews-root.md) feature, the `accessReviewDecision` represents an Azure AD access review decision of a particular entity's access.</span></span>  <span data-ttu-id="c91fd-108">In einer Access-Überprüfung oder eine Instanz einer wiederkehrenden Access Überprüfung, ist eine `accessReviewDecision` pro überprüfter Benutzer.</span><span class="sxs-lookup"><span data-stu-id="c91fd-108">Within an access review, or an instance of a recurring access review, there is one `accessReviewDecision` per reviewed user.</span></span>  <span data-ttu-id="c91fd-109">Beispielsweise eine Gruppe besitzt zwei Gäste und einen anderen Typ als Mitglieder und einer Access-Überprüfung von Gästen für diese Gruppe erfolgt dann zwei Access überprüfen Entscheidung-Objekte werden.</span><span class="sxs-lookup"><span data-stu-id="c91fd-109">For example, if a group has two guests and one non-guest as members, and an access review of guests is performed for that group, then there will be two access review decision objects.</span></span>  <span data-ttu-id="c91fd-110">Wenn ein Bearbeiter ihre Entscheidung ändert oder einen anderen Prüfer diese überschreibt, und klicken Sie dann die `accessReviewDecision` wird aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="c91fd-110">If a reviewer changes their decision, or another reviewer overrides them, then the `accessReviewDecision` is updated.</span></span>


## <a name="methods"></a><span data-ttu-id="c91fd-111">Methoden</span><span class="sxs-lookup"><span data-stu-id="c91fd-111">Methods</span></span>

<span data-ttu-id="c91fd-112">Keine.</span><span class="sxs-lookup"><span data-stu-id="c91fd-112">None.</span></span>  <span data-ttu-id="c91fd-113">Objekte dieses Typs werden automatisch vom Feature erstellt, wenn eine Access initialisiert überprüfen, und kann nicht gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="c91fd-113">Objects of this type are automatically created by the feature when an access review initializes, and cannot be deleted.</span></span>  <span data-ttu-id="c91fd-114">Sie können von einer Access-Überprüfung mit den Beziehungen [Entscheidungen](../api/accessreview-listdecisions.md) und [Mydecisions](../api/accessreview-listmydecisions.md) abgerufen werden.</span><span class="sxs-lookup"><span data-stu-id="c91fd-114">They can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships.</span></span>

## <a name="properties"></a><span data-ttu-id="c91fd-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c91fd-115">Properties</span></span>

<span data-ttu-id="c91fd-116">Die folgende Tabelle zeigt die Basiseigenschaften Objekte dieses Typs.</span><span class="sxs-lookup"><span data-stu-id="c91fd-116">This table illustrates the base properties of objects of this type.</span></span> 

| <span data-ttu-id="c91fd-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c91fd-117">Property</span></span>                        | <span data-ttu-id="c91fd-118">Typ</span><span class="sxs-lookup"><span data-stu-id="c91fd-118">Type</span></span>                         | <span data-ttu-id="c91fd-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c91fd-119">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `id`                            |`String`                      | <span data-ttu-id="c91fd-120">Die Id der Entscheidung in die Access-Überprüfung.</span><span class="sxs-lookup"><span data-stu-id="c91fd-120">The id of the decision within the access review.</span></span>                                                                                     |
| `accessReviewId`                |`String`                      | <span data-ttu-id="c91fd-121">Die Funktion generierte Id der Überprüfung Zugriff.</span><span class="sxs-lookup"><span data-stu-id="c91fd-121">The feature-generated id of the access review.</span></span>                                                                                       |
| `reviewedBy`                    |[<span data-ttu-id="c91fd-122">Benutzeridentität</span><span class="sxs-lookup"><span data-stu-id="c91fd-122">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="c91fd-123">Die Identität des Bearbeiters.</span><span class="sxs-lookup"><span data-stu-id="c91fd-123">The identity of the reviewer.</span></span>                                                                                       |
| `reviewedDate`                  |`DateTimeOffset`              | <span data-ttu-id="c91fd-124">Datum und Uhrzeit die letzte Überprüfung für dieses Zugriffsrecht angegeben wurde.</span><span class="sxs-lookup"><span data-stu-id="c91fd-124">The date and time the most recent review for this access right was supplied.</span></span>                                                                         |
| `reviewResult`                  |`String`                      | <span data-ttu-id="c91fd-125">Das Ergebnis der Überprüfung.</span><span class="sxs-lookup"><span data-stu-id="c91fd-125">The result of the review.</span></span>                                                                                    |
| `justification`                 |`String`                      | <span data-ttu-id="c91fd-126">Der Prüfer-unternehmensvorgabe, wenn angegeben.</span><span class="sxs-lookup"><span data-stu-id="c91fd-126">The reviewer's business justification, if supplied.</span></span>                                                                         |
| `appliedBy`                     |[<span data-ttu-id="c91fd-127">Benutzeridentität</span><span class="sxs-lookup"><span data-stu-id="c91fd-127">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="c91fd-128">Wenn die Überprüfung abgeschlossen ist, wenn die Ergebnisse manuell angewendet wurden, die Benutzeridentität des Benutzers, der die Entscheidung angewendet.</span><span class="sxs-lookup"><span data-stu-id="c91fd-128">When the review completes, if the results were manually applied, the user identity of the user who applied the decision.</span></span>                                                           |
| `appliedDateTime`               |`DateTimeOffset`              | <span data-ttu-id="c91fd-129">Datum und Uhrzeit, wann die Überprüfung Entscheidung angewendet wurde.</span><span class="sxs-lookup"><span data-stu-id="c91fd-129">The date and time when the review decision was applied.</span></span>                                                          |
| `applyResult`                   |`String`                      | <span data-ttu-id="c91fd-130">Das Ergebnis der Anwendung der Entscheidung, eine der `NotApplied`, `Success`, `Failed`, `NotFound` oder `NotSupported`.</span><span class="sxs-lookup"><span data-stu-id="c91fd-130">The outcome of applying the decision, one of `NotApplied`, `Success`, `Failed`, `NotFound` or `NotSupported`.</span></span>                      |
| `accessRecommendation`          |`String`                      | <span data-ttu-id="c91fd-131">Die Feature-generiert Empfehlung dargestellt, um der Prüfer, eine der `Approve`, `Deny` oder `NotAvailable`.</span><span class="sxs-lookup"><span data-stu-id="c91fd-131">The feature- generated recommendation shown to the reviewer, one of `Approve`, `Deny` or `NotAvailable`.</span></span> |


<span data-ttu-id="c91fd-132">Darüber hinaus können zusätzliche Eigenschaften vorhanden sein, je nach Typ des des-Objekts mit dem Zugriff, der beschlossen wurde.</span><span class="sxs-lookup"><span data-stu-id="c91fd-132">In addition, additional properties may be present depending on the object type of the object possessing the access that was decided upon.</span></span>  <span data-ttu-id="c91fd-133">Ist die Entscheidung Access überprüfen Gruppenmitgliedschaft eines bestimmten Benutzers oder Anwendungszugriff, wird der Benutzer potenziell ihre entfernt werden, werden über diese Eigenschaften identifiziert:</span><span class="sxs-lookup"><span data-stu-id="c91fd-133">For example, if the access review decision is a particular user's group membership or application access, the user who is potentially going to have their access be removed is identified through these properties:</span></span>

| <span data-ttu-id="c91fd-134">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c91fd-134">Property</span></span>                        | <span data-ttu-id="c91fd-135">Typ</span><span class="sxs-lookup"><span data-stu-id="c91fd-135">Type</span></span>                         | <span data-ttu-id="c91fd-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c91fd-136">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `userId`                            |`String`                      | <span data-ttu-id="c91fd-137">Die Id des Benutzers, dessen Zugriff überprüft wurde.</span><span class="sxs-lookup"><span data-stu-id="c91fd-137">The id of user whose access was reviewed.</span></span>                                                                                    |
| `userDisplayName`                            |`String`                      | <span data-ttu-id="c91fd-138">Der Anzeigename des Benutzers, dessen Zugriff überprüft wurde.</span><span class="sxs-lookup"><span data-stu-id="c91fd-138">The display name of the user whose access was reviewed.</span></span>                                                                                     |
| `userPrincipalName`                            |`String`                      | <span data-ttu-id="c91fd-139">Der Benutzerprinzipalname des Benutzers, dessen Zugriff überprüft wurde.</span><span class="sxs-lookup"><span data-stu-id="c91fd-139">The user principal name of the user whose access was reviewed.</span></span>                                                                                     |



## <a name="relationships"></a><span data-ttu-id="c91fd-140">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c91fd-140">Relationships</span></span>

<span data-ttu-id="c91fd-141">Keine.</span><span class="sxs-lookup"><span data-stu-id="c91fd-141">None.</span></span>  <span data-ttu-id="c91fd-142">Objekte dieses Typs können aus einer Access-Überprüfung mit den Beziehungen [Entscheidungen](../api/accessreview-listdecisions.md) und [Mydecisions](../api/accessreview-listmydecisions.md) des [AccessReview](accessreview.md) -Objekts abgerufen werden.</span><span class="sxs-lookup"><span data-stu-id="c91fd-142">Objects of this type can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships of the [accessReview](accessreview.md) object.</span></span>

## <a name="see-also"></a><span data-ttu-id="c91fd-143">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="c91fd-143">See also</span></span>

| <span data-ttu-id="c91fd-144">Methode</span><span class="sxs-lookup"><span data-stu-id="c91fd-144">Method</span></span>           | <span data-ttu-id="c91fd-145">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="c91fd-145">Return Type</span></span>    |<span data-ttu-id="c91fd-146">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c91fd-146">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c91fd-147">Liste AccessReview Entscheidungen</span><span class="sxs-lookup"><span data-stu-id="c91fd-147">List accessReview decisions</span></span>](../api/accessreview-listdecisions.md) |      <span data-ttu-id="c91fd-148">[AccessReviewDecision](accessreviewdecision.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="c91fd-148">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="c91fd-149">Rufen Sie die Entscheidungen des ein AccessReview.</span><span class="sxs-lookup"><span data-stu-id="c91fd-149">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="c91fd-150">Meine AccessReview Entscheidungen auflisten</span><span class="sxs-lookup"><span data-stu-id="c91fd-150">List my accessReview decisions</span></span>](../api/accessreview-listmydecisions.md) |     <span data-ttu-id="c91fd-151">[AccessReviewDecision](accessreviewdecision.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="c91fd-151">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="c91fd-152">Rufen Sie als "Leser" Mein Entscheidungen von einer AccessReview.</span><span class="sxs-lookup"><span data-stu-id="c91fd-152">As a reviewer, get my decisions of an accessReview.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c91fd-153">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c91fd-153">JSON representation</span></span>

<span data-ttu-id="c91fd-154">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c91fd-154">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessReviewDecision"
}-->

```json
{
"id": "string (identifier)",
"accessReviewId": "string (identifier)",
"reviewedBy": "microsoft.graph.userIdentity",
"reviewedDate": "string (timestamp)",
"reviewResult": "string",
"justification": "string",
"appliedBy": "microsoft.graph.userIdentity",
"appliedDateTime": "string (timestamp)",
"applyResult": "string",
"accessRecommendation": "string",
"userId": "string",
"userDisplayName": "string",
"userPrincipalName": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewDecision resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/accessreviewdecision.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
