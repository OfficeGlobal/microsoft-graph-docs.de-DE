---
title: Gruppe erstellen
description: 'Verwenden Sie diese API zum Erstellen einer neuen Gruppe gemäß der Angabe im Anforderungstext. Sie können drei Typen von Gruppen erstellen:'
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: bc83ccc3c32dbde12b93c1d22eb7640e4e72fcb8
ms.sourcegitcommit: 71368f59d267c8188567529e74486e54cc122804
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29442318"
---
# <a name="create-group"></a><span data-ttu-id="1cf61-104">Gruppe erstellen</span><span class="sxs-lookup"><span data-stu-id="1cf61-104">Create group</span></span>
<span data-ttu-id="1cf61-p102">Verwenden Sie diese API zum Erstellen einer neuen Gruppe gemäß der Angabe im Anforderungstext. Sie können drei Typen von Gruppen erstellen:</span><span class="sxs-lookup"><span data-stu-id="1cf61-p102">Use this API to create a new group as specified in the request body. You can create one of three types of groups:</span></span>

* <span data-ttu-id="1cf61-107">Office 365-Gruppe (einheitliche Gruppe)</span><span class="sxs-lookup"><span data-stu-id="1cf61-107">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="1cf61-108">Dynamische Gruppe</span><span class="sxs-lookup"><span data-stu-id="1cf61-108">Dynamic group</span></span>
* <span data-ttu-id="1cf61-109">Sicherheitsgruppe</span><span class="sxs-lookup"><span data-stu-id="1cf61-109">Security group</span></span>

<span data-ttu-id="1cf61-110">Dieser Vorgang gibt standardmäßig nur eine Teilmenge der Eigenschaften für jede Gruppe zurück.</span><span class="sxs-lookup"><span data-stu-id="1cf61-110">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="1cf61-111">Diese Standardeigenschaften werden im Abschnitt [Eigenschaften](../resources/group.md#properties) aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="1cf61-111">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span>

<span data-ttu-id="1cf61-112">Um Eigenschaften abzurufen, die _nicht_ standardmäßig zurückgegeben werden, führen Sie eine GET-Operation aus, und geben Sie die Eigenschaften in einer OData-Abfrageoption `$select` an.</span><span class="sxs-lookup"><span data-stu-id="1cf61-112">To get properties that are _not_ returned by default, do a GET operation and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="1cf61-113">Sehen Sie sich das [Beispiel](group-get.md#request-2) an.</span><span class="sxs-lookup"><span data-stu-id="1cf61-113">See an [example](group-get.md#request-2).</span></span>

> <span data-ttu-id="1cf61-p105">**Hinweis**: Microsoft Teams basiert zwar auf Office 365-Gruppen, über diese API kann derzeit aber kein Team erstellt werden. Sie können die anderen Gruppen-APIs verwenden, um ein Team zu verwalten, das in der Microsoft Teams-Benutzeroberfläche erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="1cf61-p105">**Note**: Although Microsoft Teams is built on Office 365 Groups, you can't currently create a team via this API. You can use the other group APIs to manage a team that has been created in the Microsoft Teams UI.</span></span>

## <a name="permissions"></a><span data-ttu-id="1cf61-116">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1cf61-116">Permissions</span></span>
<span data-ttu-id="1cf61-p106">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1cf61-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1cf61-119">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1cf61-119">Permission type</span></span>      | <span data-ttu-id="1cf61-120">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1cf61-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1cf61-121">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1cf61-121">Delegated (work or school account)</span></span> | <span data-ttu-id="1cf61-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cf61-122">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1cf61-123">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1cf61-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1cf61-124">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1cf61-124">Not supported.</span></span>    |
|<span data-ttu-id="1cf61-125">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1cf61-125">Application</span></span> | <span data-ttu-id="1cf61-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cf61-126">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1cf61-127">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1cf61-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="1cf61-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1cf61-128">Request headers</span></span>
| <span data-ttu-id="1cf61-129">Name</span><span class="sxs-lookup"><span data-stu-id="1cf61-129">Name</span></span>       | <span data-ttu-id="1cf61-130">Typ</span><span class="sxs-lookup"><span data-stu-id="1cf61-130">Type</span></span> | <span data-ttu-id="1cf61-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1cf61-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1cf61-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="1cf61-132">Authorization</span></span>  | <span data-ttu-id="1cf61-133">string</span><span class="sxs-lookup"><span data-stu-id="1cf61-133">string</span></span>  | <span data-ttu-id="1cf61-p107">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1cf61-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1cf61-136">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1cf61-136">Request body</span></span>
<span data-ttu-id="1cf61-137">Die folgende Tabelle enthält die Eigenschaften der [group](../resources/group.md)-Ressource, die Sie beim Erstellen einer Gruppe angeben müssen.</span><span class="sxs-lookup"><span data-stu-id="1cf61-137">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="1cf61-138">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1cf61-138">Property</span></span> | <span data-ttu-id="1cf61-139">Typ</span><span class="sxs-lookup"><span data-stu-id="1cf61-139">Type</span></span> | <span data-ttu-id="1cf61-140">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1cf61-140">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1cf61-141">displayName</span><span class="sxs-lookup"><span data-stu-id="1cf61-141">displayName</span></span> | <span data-ttu-id="1cf61-142">string</span><span class="sxs-lookup"><span data-stu-id="1cf61-142">string</span></span> | <span data-ttu-id="1cf61-143">Der Name der Gruppe, der im Adressbuch angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="1cf61-143">The name to display in the address book for the group.</span></span> <span data-ttu-id="1cf61-144">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1cf61-144">Required.</span></span> |
| <span data-ttu-id="1cf61-145">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="1cf61-145">mailEnabled</span></span> | <span data-ttu-id="1cf61-146">boolean</span><span class="sxs-lookup"><span data-stu-id="1cf61-146">boolean</span></span> | <span data-ttu-id="1cf61-147">**true** für E-Mail-aktivierte Gruppen.</span><span class="sxs-lookup"><span data-stu-id="1cf61-147">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="1cf61-148">**true**, wenn eine Office 365-Gruppe erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="1cf61-148">Set this to **true** if creating an Office 365 Group.</span></span> <span data-ttu-id="1cf61-149">**false**, wenn eine dynamische oder eine Sicherheitsgruppe erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="1cf61-149">Set this to **false** if creating dynamic or security group.</span></span> <span data-ttu-id="1cf61-150">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1cf61-150">Required.</span></span> |
| <span data-ttu-id="1cf61-151">mailNickname</span><span class="sxs-lookup"><span data-stu-id="1cf61-151">mailNickname</span></span> | <span data-ttu-id="1cf61-152">string</span><span class="sxs-lookup"><span data-stu-id="1cf61-152">string</span></span> | <span data-ttu-id="1cf61-153">Der E-Mail-Alias für die Gruppe.</span><span class="sxs-lookup"><span data-stu-id="1cf61-153">The mail alias for the group.</span></span> <span data-ttu-id="1cf61-154">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1cf61-154">Required.</span></span> |
| <span data-ttu-id="1cf61-155">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="1cf61-155">securityEnabled</span></span> | <span data-ttu-id="1cf61-156">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1cf61-156">boolean</span></span> | <span data-ttu-id="1cf61-157">**true** für Gruppen mit aktivierter Sicherheit.</span><span class="sxs-lookup"><span data-stu-id="1cf61-157">Set to **true** for security-enabled groups.</span></span> <span data-ttu-id="1cf61-158">**true**, wenn eine dynamische oder eine Sicherheitsgruppe erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="1cf61-158">Set this to **true** if creating a dynamic or security group.</span></span> <span data-ttu-id="1cf61-159">**false**, wenn eine Office 365-Gruppe erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="1cf61-159">Set this to **false** if creating an Office 365 group.</span></span> <span data-ttu-id="1cf61-160">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1cf61-160">Required.</span></span> |
| <span data-ttu-id="1cf61-161">owners</span><span class="sxs-lookup"><span data-stu-id="1cf61-161">owners</span></span> | <span data-ttu-id="1cf61-162">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="1cf61-162">string collection</span></span> | <span data-ttu-id="1cf61-163">Diese Eigenschaft stellt die Besitzer für die Gruppe zum Zeitpunkt der Erstellung dar.</span><span class="sxs-lookup"><span data-stu-id="1cf61-163">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="1cf61-164">Optional.</span><span class="sxs-lookup"><span data-stu-id="1cf61-164">Optional.</span></span> |
| <span data-ttu-id="1cf61-165">members</span><span class="sxs-lookup"><span data-stu-id="1cf61-165">members</span></span> | <span data-ttu-id="1cf61-166">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="1cf61-166">string collection</span></span> | <span data-ttu-id="1cf61-167">Diese Eigenschaft stellt die Mitglieder der Gruppe zum Zeitpunkt der Erstellung dar.</span><span class="sxs-lookup"><span data-stu-id="1cf61-167">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="1cf61-168">Optional.</span><span class="sxs-lookup"><span data-stu-id="1cf61-168">Optional.</span></span> |


<span data-ttu-id="1cf61-169">Geben Sie die **groupTypes**-Eigenschaft an, wenn Sie eine Office 365- oder eine dynamische Gruppe erstellen, wie unten beschrieben.</span><span class="sxs-lookup"><span data-stu-id="1cf61-169">Specify the **groupTypes** property if you're creating an Office 365 or dynamic group, as stated below.</span></span>

### <a name="grouptypes-options"></a><span data-ttu-id="1cf61-170">groupTypes-Optionen</span><span class="sxs-lookup"><span data-stu-id="1cf61-170">groupTypes options</span></span>

| <span data-ttu-id="1cf61-171">Typ der Gruppe</span><span class="sxs-lookup"><span data-stu-id="1cf61-171">Type of group</span></span> | <span data-ttu-id="1cf61-172">**groupTypes**-Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1cf61-172">**groupTypes** property</span></span> |
|:--------------|:------------------------|
| <span data-ttu-id="1cf61-173">Office 365 (auch einheitliche Gruppe genannt)</span><span class="sxs-lookup"><span data-stu-id="1cf61-173">Office 365 (aka unified group)</span></span>| <span data-ttu-id="1cf61-174">„Unified“</span><span class="sxs-lookup"><span data-stu-id="1cf61-174">"Unified"</span></span> |
| <span data-ttu-id="1cf61-175">Dynamisch</span><span class="sxs-lookup"><span data-stu-id="1cf61-175">Dynamic</span></span> | <span data-ttu-id="1cf61-176">"DynamicMembership"</span><span class="sxs-lookup"><span data-stu-id="1cf61-176">"DynamicMembership"</span></span> |
| <span data-ttu-id="1cf61-177">Sicherheit</span><span class="sxs-lookup"><span data-stu-id="1cf61-177">Security</span></span> | <span data-ttu-id="1cf61-178">Nicht festlegen.</span><span class="sxs-lookup"><span data-stu-id="1cf61-178">Do not set.</span></span> |


><span data-ttu-id="1cf61-179">**Hinweis:** Beim programmgesteuerten Erstellen einer Office 365-Gruppe ohne Benutzerkontext und ohne Angabe von Besitzern wird die Gruppe anonym erstellt.</span><span class="sxs-lookup"><span data-stu-id="1cf61-179">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="1cf61-180">Dies kann dazu führen, dass die zugehörige SharePoint Online-Website nicht automatisch erstellt wird und weitere manuelle Aktionen nötig sind.</span><span class="sxs-lookup"><span data-stu-id="1cf61-180">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="1cf61-p115">Geben Sie bei Bedarf andere beschreibbare Eigenschaften für Ihre Gruppe an. Weitere Informationen finden Sie in Themen zu Eigenschaften der [group](../resources/group.md)-Ressource.</span><span class="sxs-lookup"><span data-stu-id="1cf61-p115">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="1cf61-183">Antwort</span><span class="sxs-lookup"><span data-stu-id="1cf61-183">Response</span></span>
<span data-ttu-id="1cf61-184">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [group](../resources/group.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1cf61-184">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="1cf61-185">Die Antwort enthält nur die Standardeigenschaften der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="1cf61-185">The response includes only the default properties of the group.</span></span>

## <a name="example"></a><span data-ttu-id="1cf61-186">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1cf61-186">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="1cf61-187">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="1cf61-187">Request 1</span></span>
<span data-ttu-id="1cf61-188">Die erste Beispielanfrage erstellt eine Office 365-Gruppe.</span><span class="sxs-lookup"><span data-stu-id="1cf61-188">The first example request creates an Office 365 Group.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups
Content-type: application/json
Content-length: 244

{
  "description": "Self help community for library",
  "displayName": "Library Assist",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "library",
  "securityEnabled": false
}
```

#### <a name="response-1"></a><span data-ttu-id="1cf61-189">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="1cf61-189">Response 1</span></span>
<span data-ttu-id="1cf61-190">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1cf61-190">The following is an example of the response.</span></span>
><span data-ttu-id="1cf61-191">**Hinweis:**  Das hier gezeigte Antwortobjekt ist möglicherweise zur besseren Lesbarkeit gekürzt worden.</span><span class="sxs-lookup"><span data-stu-id="1cf61-191">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1cf61-192">Von einem tatsächlichen Aufruf werden alle Standardeigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1cf61-192">All the default properties are returned from an actual call.</span></span>
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
    "id": "b320ee12-b1cd-4cca-b648-a437be61c5cd",
      "deletedDateTime": null,
      "classification": null,
      "createdDateTime": "2018-12-22T00:51:37Z",
      "creationOptions": [],
      "description": "Self help community for library",
      "displayName": "Library Assist",
      "groupTypes": [
          "Unified"
      ],
      "mail": "library7423@contoso.com",
      "mailEnabled": true,
      "mailNickname": "library",
      "onPremisesLastSyncDateTime": null,
      "onPremisesSecurityIdentifier": null,
      "onPremisesSyncEnabled": null,
      "preferredDataLocation": "CAN",
      "proxyAddresses": [
          "SMTP:library7423@contoso.com"
      ],
      "renewedDateTime": "2018-12-22T00:51:37Z",
      "resourceBehaviorOptions": [],
      "resourceProvisioningOptions": [],
      "securityEnabled": false,
      "visibility": "Public",
      "onPremisesProvisioningErrors": []
}
```

#### <a name="request-2"></a><span data-ttu-id="1cf61-193">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="1cf61-193">Request 2</span></span>
<span data-ttu-id="1cf61-194">Die zweite Beispielanfrage erstellt eine Office 365-Gruppe mit einem angegebenen Besitzer und Mitgliedern.</span><span class="sxs-lookup"><span data-stu-id="1cf61-194">The second example request creates an Office 365 group with an owner specified.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_prepopulated_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups
Content-Type: application/json

{
  "description": "Group with designated owner and members",
  "displayName": "Operations group",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "operations2019",
  "securityEnabled": false,
  "owners@odata.bind": [
    "https://graph.microsoft.com/v1.0/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ],
  "members@odata.bind": [
    "https://graph.microsoft.com/v1.0/users/ff7cb387-6688-423c-8188-3da9532a73cc",
    "https://graph.microsoft.com/v1.0/users/69456242-0067-49d3-ba96-9de6f2728e14"
  ]
}
```

#### <a name="response-2"></a><span data-ttu-id="1cf61-195">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="1cf61-195">Response 2</span></span>
<span data-ttu-id="1cf61-196">Es folgt ein Beispiel für eine erfolgreiche Antwort.</span><span class="sxs-lookup"><span data-stu-id="1cf61-196">The following is an example of a successful response.</span></span> <span data-ttu-id="1cf61-197">Es enthält nur Standardeigenschaften.</span><span class="sxs-lookup"><span data-stu-id="1cf61-197">It includes only default properties.</span></span> <span data-ttu-id="1cf61-198">Sie können anschließend die **owners**- oder **members**-Navigationseigenschaft der Gruppe abrufen, um den Besitzer oder die Mitglieder zu überprüfen.</span><span class="sxs-lookup"><span data-stu-id="1cf61-198">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 
><span data-ttu-id="1cf61-199">**Hinweis:**  Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="1cf61-199">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1cf61-200">Von einem tatsächlichen Aufruf werden alle Standardeigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1cf61-200">All the default properties are returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_prepopulated_group"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
    "id": "502df398-d59c-469d-944f-34a50e60db3f",
    "deletedDateTime": null,
    "classification": null,
    "createdDateTime": "2018-12-27T22:17:07Z",
    "creationOptions": [],
    "description": "Group with designated owner and members",
    "displayName": "Operations group",
    "groupTypes": [
        "Unified"
    ],
    "mail": "operations2019@contoso.com",
    "mailEnabled": true,
    "mailNickname": "operations2019",
    "onPremisesLastSyncDateTime": null,
    "onPremisesSecurityIdentifier": null,
    "onPremisesSyncEnabled": null,
    "preferredDataLocation": "CAN",
    "proxyAddresses": [
        "SMTP:operations2019@contoso.com"
    ],
    "renewedDateTime": "2018-12-27T22:17:07Z",
    "resourceBehaviorOptions": [],
    "resourceProvisioningOptions": [],
    "securityEnabled": false,
    "visibility": "Public",
    "onPremisesProvisioningErrors": []
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
