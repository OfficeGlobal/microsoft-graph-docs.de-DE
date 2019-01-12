---
title: Ressourcentyp accessReviewDecision
description: In Azure AD Access Feature, überprüft die `accessReviewDecision` eine Azure AD Access Treffen einer Entscheidung anhand des Zugriffs für eine bestimmte Entität darstellt.  In einer Access-Überprüfung oder eine Instanz einer wiederkehrenden Access Überprüfung, ist eine `accessReviewDecision` pro überprüfter Benutzer.  Beispielsweise eine Gruppe besitzt zwei Gäste und einen anderen Typ als Mitglieder und einer Access-Überprüfung von Gästen für diese Gruppe erfolgt dann zwei Access überprüfen Entscheidung-Objekte werden.  Wenn ein Bearbeiter ihre Entscheidung ändert oder einen anderen Prüfer diese überschreibt, und klicken Sie dann die `accessReviewDecision` wird aktualisiert.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b6b10a53726e12c37a598f8df735a3f70174c807
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977556"
---
# <a name="accessreviewdecision-resource-type"></a><span data-ttu-id="230e9-106">Ressourcentyp accessReviewDecision</span><span class="sxs-lookup"><span data-stu-id="230e9-106">accessReviewDecision resource type</span></span>

> <span data-ttu-id="230e9-107">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="230e9-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="230e9-108">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="230e9-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="230e9-109">In der Azure AD [Access überprüft](accessreviews-root.md) -Funktion die `accessReviewDecision` eine Azure AD Access Treffen einer Entscheidung anhand des Zugriffs für eine bestimmte Entität darstellt.</span><span class="sxs-lookup"><span data-stu-id="230e9-109">In the Azure AD [access reviews](accessreviews-root.md) feature, the `accessReviewDecision` represents an Azure AD access review decision of a particular entity's access.</span></span>  <span data-ttu-id="230e9-110">In einer Access-Überprüfung oder eine Instanz einer wiederkehrenden Access Überprüfung, ist eine `accessReviewDecision` pro überprüfter Benutzer.</span><span class="sxs-lookup"><span data-stu-id="230e9-110">Within an access review, or an instance of a recurring access review, there is one `accessReviewDecision` per reviewed user.</span></span>  <span data-ttu-id="230e9-111">Beispielsweise eine Gruppe besitzt zwei Gäste und einen anderen Typ als Mitglieder und einer Access-Überprüfung von Gästen für diese Gruppe erfolgt dann zwei Access überprüfen Entscheidung-Objekte werden.</span><span class="sxs-lookup"><span data-stu-id="230e9-111">For example, if a group has two guests and one non-guest as members, and an access review of guests is performed for that group, then there will be two access review decision objects.</span></span>  <span data-ttu-id="230e9-112">Wenn ein Bearbeiter ihre Entscheidung ändert oder einen anderen Prüfer diese überschreibt, und klicken Sie dann die `accessReviewDecision` wird aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="230e9-112">If a reviewer changes their decision, or another reviewer overrides them, then the `accessReviewDecision` is updated.</span></span>


## <a name="methods"></a><span data-ttu-id="230e9-113">Methoden</span><span class="sxs-lookup"><span data-stu-id="230e9-113">Methods</span></span>

<span data-ttu-id="230e9-114">Keine.</span><span class="sxs-lookup"><span data-stu-id="230e9-114">None.</span></span>  <span data-ttu-id="230e9-115">Objekte dieses Typs werden automatisch vom Feature erstellt, wenn eine Access initialisiert überprüfen, und kann nicht gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="230e9-115">Objects of this type are automatically created by the feature when an access review initializes, and cannot be deleted.</span></span>  <span data-ttu-id="230e9-116">Sie können von einer Access-Überprüfung mit den Beziehungen [Entscheidungen](../api/accessreview-listdecisions.md) und [Mydecisions](../api/accessreview-listmydecisions.md) abgerufen werden.</span><span class="sxs-lookup"><span data-stu-id="230e9-116">They can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships.</span></span>

## <a name="properties"></a><span data-ttu-id="230e9-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="230e9-117">Properties</span></span>

<span data-ttu-id="230e9-118">Die folgende Tabelle zeigt die Basiseigenschaften Objekte dieses Typs.</span><span class="sxs-lookup"><span data-stu-id="230e9-118">This table illustrates the base properties of objects of this type.</span></span> 

| <span data-ttu-id="230e9-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="230e9-119">Property</span></span>                        | <span data-ttu-id="230e9-120">Typ</span><span class="sxs-lookup"><span data-stu-id="230e9-120">Type</span></span>                         | <span data-ttu-id="230e9-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="230e9-121">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `id`                            |`String`                      | <span data-ttu-id="230e9-122">Die Id der Entscheidung in die Access-Überprüfung.</span><span class="sxs-lookup"><span data-stu-id="230e9-122">The id of the decision within the access review.</span></span>                                                                                     |
| `accessReviewId`                |`String`                      | <span data-ttu-id="230e9-123">Die Funktion generierte Id der Überprüfung Zugriff.</span><span class="sxs-lookup"><span data-stu-id="230e9-123">The feature-generated id of the access review.</span></span>                                                                                       |
| `reviewedBy`                    |[<span data-ttu-id="230e9-124">Benutzeridentität</span><span class="sxs-lookup"><span data-stu-id="230e9-124">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="230e9-125">Die Identität des Bearbeiters.</span><span class="sxs-lookup"><span data-stu-id="230e9-125">The identity of the reviewer.</span></span>                                                                                       |
| `reviewedDate`                  |`DateTimeOffset`              | <span data-ttu-id="230e9-126">Datum und Uhrzeit die letzte Überprüfung für dieses Zugriffsrecht angegeben wurde.</span><span class="sxs-lookup"><span data-stu-id="230e9-126">The date and time the most recent review for this access right was supplied.</span></span>                                                                         |
| `reviewResult`                  |`String`                      | <span data-ttu-id="230e9-127">Das Ergebnis der Überprüfung.</span><span class="sxs-lookup"><span data-stu-id="230e9-127">The result of the review.</span></span>                                                                                    |
| `justification`                 |`String`                      | <span data-ttu-id="230e9-128">Der Prüfer-unternehmensvorgabe, wenn angegeben.</span><span class="sxs-lookup"><span data-stu-id="230e9-128">The reviewer's business justification, if supplied.</span></span>                                                                         |
| `appliedBy`                     |[<span data-ttu-id="230e9-129">Benutzeridentität</span><span class="sxs-lookup"><span data-stu-id="230e9-129">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="230e9-130">Wenn die Überprüfung abgeschlossen ist, wenn die Ergebnisse manuell angewendet wurden, die Benutzeridentität des Benutzers, der die Entscheidung angewendet.</span><span class="sxs-lookup"><span data-stu-id="230e9-130">When the review completes, if the results were manually applied, the user identity of the user who applied the decision.</span></span>                                                           |
| `appliedDateTime`               |`DateTimeOffset`              | <span data-ttu-id="230e9-131">Datum und Uhrzeit, wann die Überprüfung Entscheidung angewendet wurde.</span><span class="sxs-lookup"><span data-stu-id="230e9-131">The date and time when the review decision was applied.</span></span>                                                          |
| `applyResult`                   |`String`                      | <span data-ttu-id="230e9-132">Das Ergebnis der Anwendung der Entscheidung, eine der `NotApplied`, `Success`, `Failed`, `NotFound` oder `NotSupported`.</span><span class="sxs-lookup"><span data-stu-id="230e9-132">The outcome of applying the decision, one of `NotApplied`, `Success`, `Failed`, `NotFound` or `NotSupported`.</span></span>                      |
| `accessRecommendation`          |`String`                      | <span data-ttu-id="230e9-133">Die Feature-generiert Empfehlung dargestellt, um der Prüfer, eine der `Approve`, `Deny` oder `NotAvailable`.</span><span class="sxs-lookup"><span data-stu-id="230e9-133">The feature- generated recommendation shown to the reviewer, one of `Approve`, `Deny` or `NotAvailable`.</span></span> |


<span data-ttu-id="230e9-134">Darüber hinaus können zusätzliche Eigenschaften vorhanden sein, je nach Typ des des-Objekts mit dem Zugriff, der beschlossen wurde.</span><span class="sxs-lookup"><span data-stu-id="230e9-134">In addition, additional properties may be present depending on the object type of the object possessing the access that was decided upon.</span></span>  <span data-ttu-id="230e9-135">Ist die Entscheidung Access überprüfen Gruppenmitgliedschaft eines bestimmten Benutzers oder Anwendungszugriff, wird der Benutzer potenziell ihre entfernt werden, werden über diese Eigenschaften identifiziert:</span><span class="sxs-lookup"><span data-stu-id="230e9-135">For example, if the access review decision is a particular user's group membership or application access, the user who is potentially going to have their access be removed is identified through these properties:</span></span>

| <span data-ttu-id="230e9-136">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="230e9-136">Property</span></span>                        | <span data-ttu-id="230e9-137">Typ</span><span class="sxs-lookup"><span data-stu-id="230e9-137">Type</span></span>                         | <span data-ttu-id="230e9-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="230e9-138">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `userId`                            |`String`                      | <span data-ttu-id="230e9-139">Die Id des Benutzers, dessen Zugriff überprüft wurde.</span><span class="sxs-lookup"><span data-stu-id="230e9-139">The id of user whose access was reviewed.</span></span>                                                                                    |
| `userDisplayName`                            |`String`                      | <span data-ttu-id="230e9-140">Der Anzeigename des Benutzers, dessen Zugriff überprüft wurde.</span><span class="sxs-lookup"><span data-stu-id="230e9-140">The display name of the user whose access was reviewed.</span></span>                                                                                     |
| `userPrincipalName`                            |`String`                      | <span data-ttu-id="230e9-141">Der Benutzerprinzipalname des Benutzers, dessen Zugriff überprüft wurde.</span><span class="sxs-lookup"><span data-stu-id="230e9-141">The user principal name of the user whose access was reviewed.</span></span>                                                                                     |



## <a name="relationships"></a><span data-ttu-id="230e9-142">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="230e9-142">Relationships</span></span>

<span data-ttu-id="230e9-143">Keine.</span><span class="sxs-lookup"><span data-stu-id="230e9-143">None.</span></span>  <span data-ttu-id="230e9-144">Objekte dieses Typs können aus einer Access-Überprüfung mit den Beziehungen [Entscheidungen](../api/accessreview-listdecisions.md) und [Mydecisions](../api/accessreview-listmydecisions.md) des [AccessReview](accessreview.md) -Objekts abgerufen werden.</span><span class="sxs-lookup"><span data-stu-id="230e9-144">Objects of this type can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships of the [accessReview](accessreview.md) object.</span></span>

## <a name="see-also"></a><span data-ttu-id="230e9-145">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="230e9-145">See also</span></span>

| <span data-ttu-id="230e9-146">Methode</span><span class="sxs-lookup"><span data-stu-id="230e9-146">Method</span></span>           | <span data-ttu-id="230e9-147">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="230e9-147">Return Type</span></span>    |<span data-ttu-id="230e9-148">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="230e9-148">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="230e9-149">Liste AccessReview Entscheidungen</span><span class="sxs-lookup"><span data-stu-id="230e9-149">List accessReview decisions</span></span>](../api/accessreview-listdecisions.md) |      <span data-ttu-id="230e9-150">[AccessReviewDecision](accessreviewdecision.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="230e9-150">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="230e9-151">Rufen Sie die Entscheidungen des ein AccessReview.</span><span class="sxs-lookup"><span data-stu-id="230e9-151">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="230e9-152">Meine AccessReview Entscheidungen auflisten</span><span class="sxs-lookup"><span data-stu-id="230e9-152">List my accessReview decisions</span></span>](../api/accessreview-listmydecisions.md) |     <span data-ttu-id="230e9-153">[AccessReviewDecision](accessreviewdecision.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="230e9-153">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="230e9-154">Rufen Sie als "Leser" Mein Entscheidungen von einer AccessReview.</span><span class="sxs-lookup"><span data-stu-id="230e9-154">As a reviewer, get my decisions of an accessReview.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="230e9-155">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="230e9-155">JSON representation</span></span>

<span data-ttu-id="230e9-156">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="230e9-156">Here is a JSON representation of the resource.</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "accessReviewDecision resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
