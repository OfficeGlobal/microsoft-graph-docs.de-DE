---
title: Erstellen von accessReview
description: Zugriff auf in Azure AD Bewertungen Feature, Erstellen eines neuen AccessReview-Objekts.
localization_priority: Normal
ms.openlocfilehash: 1ee5ce696f1d71c57adf9e6c5ee30c067536c8ff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851443"
---
# <a name="create-accessreview"></a><span data-ttu-id="526f5-103">Erstellen von accessReview</span><span class="sxs-lookup"><span data-stu-id="526f5-103">Create accessReview</span></span>

> <span data-ttu-id="526f5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="526f5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="526f5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="526f5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="526f5-106">Erstellen Sie ein neues [AccessReview](../resources/accessreview.md) -Objekt in Azure AD [Access überprüft](../resources/accessreviews-root.md) Feature.</span><span class="sxs-lookup"><span data-stu-id="526f5-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="526f5-107">Vor dieser Anforderung ausführenden, der Anrufer benötigen zuvor [die Liste der Vorlagen für Unternehmen Fluss abgerufen](businessflowtemplate-list.md), auf dem Wert der `businessFlowTemplateId` in der Anforderung enthalten.</span><span class="sxs-lookup"><span data-stu-id="526f5-107">Prior to making this request, the caller must have previously [retrieved the list of business flow templates](businessflowtemplate-list.md), to have the value of `businessFlowTemplateId` to include in the request.</span></span>

<span data-ttu-id="526f5-108">Nach dem Ändern dieser Anforderung, sollte der Aufrufer [eine ProgramControl erstellen](programcontrol-create.md), um die Überprüfung des Zugriffs auf ein Programm verknüpfen.</span><span class="sxs-lookup"><span data-stu-id="526f5-108">After making this request, the caller should [create a programControl](programcontrol-create.md), to link the access review to a program.</span></span>  

## <a name="permissions"></a><span data-ttu-id="526f5-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="526f5-109">Permissions</span></span>
<span data-ttu-id="526f5-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="526f5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="526f5-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="526f5-112">Permission type</span></span>                        | <span data-ttu-id="526f5-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="526f5-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="526f5-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="526f5-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="526f5-115">AccessReview.ReadWrite.All, und sollten auch ProgramControl.ReadWrite.All vollständige Szenario mit den nachfolgenden Aufruf einer ProgramControl erstellen</span><span class="sxs-lookup"><span data-stu-id="526f5-115">AccessReview.ReadWrite.All, and should also have ProgramControl.ReadWrite.All to complete scenario with the subsequent call to create a programControl</span></span> |
|<span data-ttu-id="526f5-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="526f5-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="526f5-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="526f5-117">Not supported.</span></span> |
|<span data-ttu-id="526f5-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="526f5-118">Application</span></span>                            | <span data-ttu-id="526f5-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="526f5-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="526f5-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="526f5-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews
```
## <a name="request-headers"></a><span data-ttu-id="526f5-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="526f5-121">Request headers</span></span>
| <span data-ttu-id="526f5-122">Name</span><span class="sxs-lookup"><span data-stu-id="526f5-122">Name</span></span>         | <span data-ttu-id="526f5-123">Typ</span><span class="sxs-lookup"><span data-stu-id="526f5-123">Type</span></span>        | <span data-ttu-id="526f5-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="526f5-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="526f5-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="526f5-125">Authorization</span></span> | <span data-ttu-id="526f5-126">string</span><span class="sxs-lookup"><span data-stu-id="526f5-126">string</span></span> | <span data-ttu-id="526f5-127">Bearer \{token\}.</span><span class="sxs-lookup"><span data-stu-id="526f5-127">Bearer \{token\}.</span></span> <span data-ttu-id="526f5-128">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="526f5-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="526f5-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="526f5-129">Request body</span></span>
<span data-ttu-id="526f5-130">Geben Sie im Textkörper Anforderung eine JSON-Darstellung eines [AccessReview](../resources/accessreview.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="526f5-130">In the request body, supply a JSON representation of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="526f5-131">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie eine AccessReview erstellen.</span><span class="sxs-lookup"><span data-stu-id="526f5-131">The following table shows the properties that are required when you create an accessReview.</span></span>

| <span data-ttu-id="526f5-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="526f5-132">Property</span></span>     | <span data-ttu-id="526f5-133">Typ</span><span class="sxs-lookup"><span data-stu-id="526f5-133">Type</span></span>        | <span data-ttu-id="526f5-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="526f5-134">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | <span data-ttu-id="526f5-135">Der Name des Access überprüfen.</span><span class="sxs-lookup"><span data-stu-id="526f5-135">The access review name.</span></span>  |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="526f5-136">Den DateTime-Wert, wenn die Überprüfung geplant ist, gestartet werden.</span><span class="sxs-lookup"><span data-stu-id="526f5-136">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="526f5-137">Dies muss ein Datum in der Zukunft sein.</span><span class="sxs-lookup"><span data-stu-id="526f5-137">This must be a date in the future.</span></span>   |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="526f5-138">Den DateTime-Wert, wenn die Überprüfung geplant ist, um zu beenden.</span><span class="sxs-lookup"><span data-stu-id="526f5-138">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="526f5-139">Dies muss mindestens einen Tag später als das Startdatum sein.</span><span class="sxs-lookup"><span data-stu-id="526f5-139">This must be at least one day later than the start date.</span></span>   |
| `description`             |`String`                                                        | <span data-ttu-id="526f5-140">Die Beschreibung für die Bearbeiter angezeigt.</span><span class="sxs-lookup"><span data-stu-id="526f5-140">The description, to show to the reviewers.</span></span> |
| `businessFlowTemplateId`  |`String`                                                        | <span data-ttu-id="526f5-141">Der Business-Fluss Vorlagenbezeichner, von einem [BusinessFlowTemplate](../resources/businessflowtemplate.md)abgerufen.</span><span class="sxs-lookup"><span data-stu-id="526f5-141">The business flow template identifier, obtained from a [businessFlowTemplate](../resources/businessflowtemplate.md).</span></span>  |
| `reviewerType`            |`String`                                                        | <span data-ttu-id="526f5-142">Die Beziehungstyp des Reviewer über die Zugriffsrechte des überarbeiteten-Objekts, eines `self`, `delegate` oder `entityOwners`.</span><span class="sxs-lookup"><span data-stu-id="526f5-142">The relationship type of reviewer to the access rights of the reviewed object, one of `self`, `delegate` or `entityOwners`.</span></span> | 
| `reviewedEntity`          |`microsoft.graph.identity`                                      | <span data-ttu-id="526f5-143">Das Objekt, für das eine Überprüfung Access, wie eine Mitgliedschaft in einer Gruppe oder die Zuweisung von Benutzern zu einer Anwendung erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="526f5-143">The object for which an access review is created, such as a memberships of an group or the assignments of users to an application.</span></span> | 


<span data-ttu-id="526f5-144">Wenn die ReviewerType gesendet wird den Wert `delegate`, und klicken Sie dann der Anrufer auch umfassen muss die `reviewers` -Eigenschaft, mit einer Auflistung von [Benutzeridentität](../resources/useridentity.md) der Bearbeiter.</span><span class="sxs-lookup"><span data-stu-id="526f5-144">If the reviewerType being supplied has the value `delegate`, then the caller must also include the `reviewers` property, with a collection of [userIdentity](../resources/useridentity.md) of the reviewers.</span></span>

<span data-ttu-id="526f5-145">Darüber hinaus kann der Aufrufer Einstellungen, zum Erstellen einer Terminserie überprüfen oder So ändern Sie das Standardverhalten für die Überprüfung umfassen.</span><span class="sxs-lookup"><span data-stu-id="526f5-145">In addition, the caller can include settings, to create a recurring review series or to change from the default review behavior.</span></span> <span data-ttu-id="526f5-146">Zum Erstellen einer wiederkehrenden Überprüfung der Anrufer muss sich insbesondere die `accessReviewRecurrenceSettings` überprüfen Sie in die Access-Einstellungen</span><span class="sxs-lookup"><span data-stu-id="526f5-146">In particular, to create a recurring review, the caller must include the `accessReviewRecurrenceSettings` within the access review settings,</span></span>


## <a name="response"></a><span data-ttu-id="526f5-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="526f5-147">Response</span></span>
<span data-ttu-id="526f5-148">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `201, Created` Antwortcode und eines [AccessReview](../resources/accessreview.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="526f5-148">If successful, this method returns a `201, Created` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="526f5-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="526f5-149">Example</span></span>

<span data-ttu-id="526f5-150">Dies ist ein Beispiel zum Erstellen einer einmaligen (nicht wiederkehrende) Access Überprüfung als Bearbeiter zwei Benutzer explizit angeben.</span><span class="sxs-lookup"><span data-stu-id="526f5-150">This is an example of creating a one-time (not recurring) access review, explicitly specifying two users as the reviewers.</span></span>

##### <a name="request"></a><span data-ttu-id="526f5-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="526f5-151">Request</span></span>
<span data-ttu-id="526f5-152">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [AccessReview](../resources/accessreview.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="526f5-152">In the request body, supply a JSON representation of the [accessReview](../resources/accessreview.md) object.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_accessReview_from_accessReviews"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews
Content-type: application/json

{
    "displayName":"TestReview",
    "startDateTime":"2017-02-10T00:35:53.214Z",
    "endDateTime":"2017-03-12T00:35:53.214Z",
    "reviewedEntity": {
        "id": "99025615-a0b1-47ec-9117-35377b10998b",
    },
    "reviewerType" : "delegate",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "description":"Sample description",
    "reviewers":
    [
        {
            "id":"f260246a-09b1-4fd5-8d18-daed736071ec"
        },
        {
            "id":"5a4e184c-4ee5-4883-96e9-b371f8da88e3"
        }
    ],
    "settings":
    {
        "justificationRequiredOnApproval": true,
        "activityHistoryInDays":30,
        "mailNotificationsEnabled":true,
        "remindersEnabled":true
    }
}
```

##### <a name="response"></a><span data-ttu-id="526f5-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="526f5-153">Response</span></span>
><span data-ttu-id="526f5-p107">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="526f5-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReview"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "006111db-0810-4494-a6df-904d368bd81b",
    "displayName": "TestReview",
    "startDateTime": "2017-02-10T00:35:53.214Z",
    "endDateTime": "2017-03-12T00:35:53.214Z",
    "status": "Initializing",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "reviewerType": "delegate",
    "description": "Sample description"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Create accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
