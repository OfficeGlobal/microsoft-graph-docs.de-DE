---
title: Gruppe erstellen
description: 'Verwenden Sie diese API zum Erstellen einer neuen Gruppe gemäß der Angabe im Anforderungstext. Sie können drei Typen von Gruppen erstellen:'
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: de304cc4faaa6e4b64992ba0d7b2af35e8b5900a
ms.sourcegitcommit: 7d94b581f7c6dc1995efecf6ee21b604c0b80998
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/19/2019
ms.locfileid: "29353069"
---
# <a name="create-group"></a><span data-ttu-id="e399e-104">Gruppe erstellen</span><span class="sxs-lookup"><span data-stu-id="e399e-104">Create group</span></span>

> <span data-ttu-id="e399e-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e399e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e399e-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e399e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e399e-107">Verwenden Sie diese API zum Erstellen einer neuen [Gruppe](../resources/group.md) gemäß der Angabe im Anforderungstext.</span><span class="sxs-lookup"><span data-stu-id="e399e-107">Use this API to create a new group as specified in the request body. You can create one of three types of groups:</span></span> <span data-ttu-id="e399e-108">Sie können drei Typen von Gruppen erstellen:</span><span class="sxs-lookup"><span data-stu-id="e399e-108">You can create one of three types of groups:</span></span>

* <span data-ttu-id="e399e-109">Office 365-Gruppe (einheitliche Gruppe)</span><span class="sxs-lookup"><span data-stu-id="e399e-109">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="e399e-110">Dynamische Gruppe</span><span class="sxs-lookup"><span data-stu-id="e399e-110">Dynamic group</span></span>
* <span data-ttu-id="e399e-111">Sicherheitsgruppe</span><span class="sxs-lookup"><span data-stu-id="e399e-111">Security group</span></span>

<span data-ttu-id="e399e-112">Dieser Vorgang gibt standardmäßig nur eine Teilmenge der Eigenschaften für jede Gruppe zurück.</span><span class="sxs-lookup"><span data-stu-id="e399e-112">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="e399e-113">Diese Standardeigenschaften werden im Abschnitt [Eigenschaften](../resources/group.md#properties) aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="e399e-113">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span>

<span data-ttu-id="e399e-114">Um Eigenschaften abzurufen, die _nicht_ standardmäßig zurückgegeben werden, führen Sie eine GET-Operation aus, und geben Sie die Eigenschaften in einer OData-Abfrageoption `$select` an.</span><span class="sxs-lookup"><span data-stu-id="e399e-114">To get properties that are _not_ returned by default, do a GET operation and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="e399e-115">Sehen Sie sich das [Beispiel](group-get.md#request-2) an.</span><span class="sxs-lookup"><span data-stu-id="e399e-115">See an [example](group-get.md#request-2).</span></span>

> <span data-ttu-id="e399e-116">**Hinweis**: Zum Erstellen eines [Teams](../resources/team.md) erstellen Sie zuerst eine Gruppe und fügen ihr dann ein Team hinzu (siehe [Team erstellen](../api/team-put-teams.md)).</span><span class="sxs-lookup"><span data-stu-id="e399e-116">**Note**: To create a [team](../resources/team.md), first create a group then add a team to it, see [create team](../api/team-put-teams.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e399e-117">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e399e-117">Permissions</span></span>
<span data-ttu-id="e399e-p106">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e399e-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e399e-120">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e399e-120">Permission type</span></span>      | <span data-ttu-id="e399e-121">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e399e-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e399e-122">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e399e-122">Delegated (work or school account)</span></span> | <span data-ttu-id="e399e-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e399e-123">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e399e-124">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e399e-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e399e-125">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e399e-125">Not supported.</span></span>    |
|<span data-ttu-id="e399e-126">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e399e-126">Application</span></span> | <span data-ttu-id="e399e-127">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e399e-127">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e399e-128">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e399e-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="e399e-129">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e399e-129">Request headers</span></span>
| <span data-ttu-id="e399e-130">Name</span><span class="sxs-lookup"><span data-stu-id="e399e-130">Name</span></span>       | <span data-ttu-id="e399e-131">Typ</span><span class="sxs-lookup"><span data-stu-id="e399e-131">Type</span></span> | <span data-ttu-id="e399e-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e399e-132">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e399e-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="e399e-133">Authorization</span></span>  | <span data-ttu-id="e399e-134">string</span><span class="sxs-lookup"><span data-stu-id="e399e-134">string</span></span>  | <span data-ttu-id="e399e-p107">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e399e-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e399e-137">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e399e-137">Request body</span></span>
<span data-ttu-id="e399e-138">Die folgende Tabelle enthält die Eigenschaften der [group](../resources/group.md)-Ressource, die Sie beim Erstellen einer Gruppe angeben müssen.</span><span class="sxs-lookup"><span data-stu-id="e399e-138">The following table shows the properties of the [group](../resources/group.md) resource that you must specify at a minimum when you create a group.</span></span> 

| <span data-ttu-id="e399e-139">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e399e-139">Property</span></span> | <span data-ttu-id="e399e-140">Typ</span><span class="sxs-lookup"><span data-stu-id="e399e-140">Type</span></span> | <span data-ttu-id="e399e-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e399e-141">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e399e-142">displayName</span><span class="sxs-lookup"><span data-stu-id="e399e-142">displayName</span></span> | <span data-ttu-id="e399e-143">string</span><span class="sxs-lookup"><span data-stu-id="e399e-143">string</span></span> | <span data-ttu-id="e399e-144">Der Name der Gruppe, der im Adressbuch angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="e399e-144">The name to display in the address book for the group.</span></span> <span data-ttu-id="e399e-145">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e399e-145">Required.</span></span> |
| <span data-ttu-id="e399e-146">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="e399e-146">mailEnabled</span></span> | <span data-ttu-id="e399e-147">boolean</span><span class="sxs-lookup"><span data-stu-id="e399e-147">boolean</span></span> | <span data-ttu-id="e399e-148">**true** für E-Mail-aktivierte Gruppen.</span><span class="sxs-lookup"><span data-stu-id="e399e-148">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="e399e-149">**true**, wenn eine Office 365-Gruppe erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="e399e-149">Set this to **true** if creating an Office 365 Group.</span></span> <span data-ttu-id="e399e-150">**false**, wenn eine dynamische oder eine Sicherheitsgruppe erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="e399e-150">Set this to **false** if creating dynamic or security group.</span></span> <span data-ttu-id="e399e-151">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e399e-151">Required.</span></span> |
| <span data-ttu-id="e399e-152">mailNickname</span><span class="sxs-lookup"><span data-stu-id="e399e-152">mailNickname</span></span> | <span data-ttu-id="e399e-153">string</span><span class="sxs-lookup"><span data-stu-id="e399e-153">string</span></span> | <span data-ttu-id="e399e-154">Der E-Mail-Alias für die Gruppe.</span><span class="sxs-lookup"><span data-stu-id="e399e-154">The mail alias for the group.</span></span> <span data-ttu-id="e399e-155">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e399e-155">Required.</span></span> |
| <span data-ttu-id="e399e-156">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="e399e-156">securityEnabled</span></span> | <span data-ttu-id="e399e-157">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e399e-157">boolean</span></span> | <span data-ttu-id="e399e-158">**true** für Gruppen mit aktivierter Sicherheit.</span><span class="sxs-lookup"><span data-stu-id="e399e-158">Set to **true** for security-enabled groups.</span></span> <span data-ttu-id="e399e-159">**true**, wenn eine dynamische oder eine Sicherheitsgruppe erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="e399e-159">Set this to **true** if creating a dynamic or security group.</span></span> <span data-ttu-id="e399e-160">**false**, wenn eine Office 365-Gruppe erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="e399e-160">Set this to **false** if creating an Office 365 Group.</span></span> <span data-ttu-id="e399e-161">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e399e-161">Required.</span></span> |
| <span data-ttu-id="e399e-162">owners</span><span class="sxs-lookup"><span data-stu-id="e399e-162">owners</span></span> | <span data-ttu-id="e399e-163">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="e399e-163">string collection</span></span> | <span data-ttu-id="e399e-164">Diese Eigenschaft stellt die Besitzer für die Gruppe zum Zeitpunkt der Erstellung dar.</span><span class="sxs-lookup"><span data-stu-id="e399e-164">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="e399e-165">Optional.</span><span class="sxs-lookup"><span data-stu-id="e399e-165">Optional.</span></span> |
| <span data-ttu-id="e399e-166">members</span><span class="sxs-lookup"><span data-stu-id="e399e-166">members</span></span> | <span data-ttu-id="e399e-167">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="e399e-167">string collection</span></span> | <span data-ttu-id="e399e-168">Diese Eigenschaft stellt die Mitglieder der Gruppe zum Zeitpunkt der Erstellung dar.</span><span class="sxs-lookup"><span data-stu-id="e399e-168">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="e399e-169">Optional.</span><span class="sxs-lookup"><span data-stu-id="e399e-169">Optional.</span></span> |

<span data-ttu-id="e399e-170">Geben Sie die **groupTypes**-Eigenschaft an, wenn Sie eine Office 365- oder eine dynamische Gruppe erstellen, wie unten beschrieben.</span><span class="sxs-lookup"><span data-stu-id="e399e-170">Specify the **groupTypes** property if you're creating an Office 365 or dynamic group, as stated below.</span></span>

| <span data-ttu-id="e399e-171">Art der Gruppe</span><span class="sxs-lookup"><span data-stu-id="e399e-171">Type of group</span></span> | <span data-ttu-id="e399e-172">**groupTypes**-Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e399e-172">**groupTypes** property</span></span> |
|:--------------|:------------------------|
| <span data-ttu-id="e399e-173">Office 365 (auch einheitliche Gruppe genannt)</span><span class="sxs-lookup"><span data-stu-id="e399e-173">Office 365 (aka unified group)</span></span>| <span data-ttu-id="e399e-174">„Unified“</span><span class="sxs-lookup"><span data-stu-id="e399e-174">"Unified"</span></span> |
| <span data-ttu-id="e399e-175">Dynamisch</span><span class="sxs-lookup"><span data-stu-id="e399e-175">Dynamic</span></span> | <span data-ttu-id="e399e-176">"DynamicMembership"</span><span class="sxs-lookup"><span data-stu-id="e399e-176">"DynamicMembership"</span></span> |
| <span data-ttu-id="e399e-177">Sicherheit</span><span class="sxs-lookup"><span data-stu-id="e399e-177">Security</span></span> | <span data-ttu-id="e399e-178">Nicht festlegen.</span><span class="sxs-lookup"><span data-stu-id="e399e-178">Do not set.</span></span> |

<span data-ttu-id="e399e-179">Da die **group**-Ressource [Erweiterungen](/graph/extensibility-overview) unterstützt, können Sie den `POST`-Vorgang verwenden und beim Erstellen der Gruppe benutzerdefinierte Eigenschaften mit Ihren eigenen Daten hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="e399e-179">Since the **event** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the event while creating it.</span></span>

><span data-ttu-id="e399e-180">**Hinweis:** Beim programmgesteuerten Erstellen einer Office 365-Gruppe ohne Benutzerkontext und ohne Angabe von Besitzern wird die Gruppe anonym erstellt.</span><span class="sxs-lookup"><span data-stu-id="e399e-180">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="e399e-181">Dies kann dazu führen, dass die zugehörige SharePoint Online-Website nicht automatisch erstellt wird und weitere manuelle Aktionen nötig sind.</span><span class="sxs-lookup"><span data-stu-id="e399e-181">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="e399e-p115">Geben Sie bei Bedarf andere beschreibbare Eigenschaften für Ihre Gruppe an. Weitere Informationen finden Sie in Themen zu Eigenschaften der [group](../resources/group.md)-Ressource.</span><span class="sxs-lookup"><span data-stu-id="e399e-p115">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="e399e-184">Antwort</span><span class="sxs-lookup"><span data-stu-id="e399e-184">Response</span></span>
<span data-ttu-id="e399e-185">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [group](../resources/group.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e399e-185">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="e399e-186">Die Antwort enthält nur die Standardeigenschaften der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="e399e-186">The response includes only the default properties of the group.</span></span>

## <a name="example"></a><span data-ttu-id="e399e-187">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e399e-187">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="e399e-188">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="e399e-188">Request 1</span></span>
<span data-ttu-id="e399e-189">Die erste Beispielanfrage erstellt eine Office 365-Gruppe.</span><span class="sxs-lookup"><span data-stu-id="e399e-189">The following is an example of a request that creates an Office 365 Group.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups
Content-type: application/json
Content-length: 244

{
  "description": "Self help community for golf",
  "displayName": "Golf Assist",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "golfassist",
  "securityEnabled": false
}
```

#### <a name="response"></a><span data-ttu-id="e399e-190">Antwort</span><span class="sxs-lookup"><span data-stu-id="e399e-190">Response</span></span>
<span data-ttu-id="e399e-191">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e399e-191">The following is an example of the response.</span></span>
><span data-ttu-id="e399e-192">**Hinweis:**  Das hier gezeigte Antwortobjekt ist möglicherweise zur besseren Lesbarkeit gekürzt worden.</span><span class="sxs-lookup"><span data-stu-id="e399e-192">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e399e-193">Von einem tatsächlichen Aufruf werden alle Standardeigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e399e-193">All default properties are returned from the actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_group"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
     "id": "45b7d2e7-b882-4a80-ba97-10b7a63b8fa4",
     "deletedDateTime": null,
     "classification": null,
     "createdDateTime": "2018-12-22T02:21:05Z",
     "description": "Self help community for golf",
     "displayName": "Golf Assist",
     "expirationDateTime": null,
     "groupTypes": [
         "Unified"
     ],
     "mail": "golfassist@contoso.com",
     "mailEnabled": true,
     "mailNickname": "golfassist",
     "membershipRule": null,
     "membershipRuleProcessingState": null,
     "onPremisesLastSyncDateTime": null,
     "onPremisesSecurityIdentifier": null,
     "onPremisesSyncEnabled": null,
     "preferredDataLocation": "CAN",
     "preferredLanguage": null,
     "proxyAddresses": [
         "SMTP:golfassist@contoso.onmicrosoft.com"
     ],
     "renewedDateTime": "2018-12-22T02:21:05Z",
     "resourceBehaviorOptions": [],
     "resourceProvisioningOptions": [],
     "securityEnabled": false,
     "theme": null,
     "visibility": "Public",
     "onPremisesProvisioningErrors": []
}
```

#### <a name="request-2"></a><span data-ttu-id="e399e-194">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="e399e-194">Request 2</span></span>
<span data-ttu-id="e399e-195">Die zweite Beispielanfrage erstellt eine Office 365-Gruppe mit einem angegebenen Besitzer.</span><span class="sxs-lookup"><span data-stu-id="e399e-195">The second example request creates an Office 365 group with an owner specified.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_group_with_owner"
}-->
```http
POST https://graph.microsoft.com/beta/groups
Content-Type: application/json

{
  "description": "Group with designated owner",
  "displayName": "Operations group",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "operations2019",
  "securityEnabled": false,
  "owners@odata.bind": [
    "https://graph.microsoft.com/beta/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ]
}
```

 #### <a name="response-2"></a><span data-ttu-id="e399e-196">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="e399e-196">Response 2</span></span>
<span data-ttu-id="e399e-197">Es folgt ein Beispiel für eine erfolgreiche Antwort.</span><span class="sxs-lookup"><span data-stu-id="e399e-197">The following is an example of a response to a  event.</span></span> <span data-ttu-id="e399e-198">Es enthält nur Standardeigenschaften.</span><span class="sxs-lookup"><span data-stu-id="e399e-198">It includes only default properties.</span></span> <span data-ttu-id="e399e-199">Sie können anschließend die **owners**-Navigationseigenschaft der Gruppe abrufen, um die Details des Besitzers zu überprüfen.</span><span class="sxs-lookup"><span data-stu-id="e399e-199">You can subsequenty get the **owners** navigation property of the group to verify the details of the owner.</span></span> 
><span data-ttu-id="e399e-200">**Hinweis:**  Das hier gezeigte Antwortobjekt ist möglicherweise zur besseren Lesbarkeit gekürzt worden.</span><span class="sxs-lookup"><span data-stu-id="e399e-200">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e399e-201">Von einem tatsächlichen Aufruf werden alle Standardeigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e399e-201">All default properties are returned from the actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_group_with_owner"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
     "id": "502df398-d59c-469d-944f-34a50e60db3f",
     "deletedDateTime": null,
     "classification": null,
     "createdDateTime": "2018-12-27T22:17:07Z",
     "description": "Group with designated owner",
     "displayName": "Operations group",
     "expirationDateTime": null,
     "groupTypes": [
         "Unified"
     ],
     "mail": "operations2019@contoso.com",
     "mailEnabled": true,
     "mailNickname": "operations2019",
     "membershipRule": null,
     "membershipRuleProcessingState": null,
     "onPremisesLastSyncDateTime": null,
     "onPremisesSecurityIdentifier": null,
     "onPremisesSyncEnabled": null,
     "preferredDataLocation": "CAN",
     "preferredLanguage": null,
     "proxyAddresses": [
         "SMTP:operations2019@contoso.com"
     ],
     "renewedDateTime": "2018-12-27T22:17:07Z",
     "resourceBehaviorOptions": [],
     "resourceProvisioningOptions": [],
     "securityEnabled": false,
     "theme": null,
     "visibility": "Public",
     "onPremisesProvisioningErrors": []
}
```

## <a name="see-also"></a><span data-ttu-id="e399e-202">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="e399e-202">See also</span></span>

- [<span data-ttu-id="e399e-203">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="e399e-203">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="e399e-204">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="e399e-204">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="e399e-205">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="e399e-205">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
