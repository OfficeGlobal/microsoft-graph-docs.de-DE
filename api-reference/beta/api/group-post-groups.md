---
title: Gruppe erstellen
description: 'Verwenden Sie diese API zum Erstellen einer neuen Gruppe gemäß der Angabe im Anforderungstext. Sie können drei Typen von Gruppen erstellen:'
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 87494b309dd731c519f0d999396f283c5a2fa583
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515909"
---
# <a name="create-group"></a><span data-ttu-id="7dbba-104">Gruppe erstellen</span><span class="sxs-lookup"><span data-stu-id="7dbba-104">Create group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7dbba-p102">Verwenden Sie diese API zum Erstellen einer neuen [Gruppe](../resources/group.md) gemäß der Angabe im Anforderungstext. Sie können drei Typen von Gruppen erstellen:</span><span class="sxs-lookup"><span data-stu-id="7dbba-p102">Use this API to create a new [group](../resources/group.md) as specified in the request body. You can create one of three types of groups:</span></span>

* <span data-ttu-id="7dbba-107">Office 365-Gruppe (einheitliche Gruppe)</span><span class="sxs-lookup"><span data-stu-id="7dbba-107">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="7dbba-108">Dynamische Gruppe</span><span class="sxs-lookup"><span data-stu-id="7dbba-108">Dynamic group</span></span>
* <span data-ttu-id="7dbba-109">Sicherheitsgruppe</span><span class="sxs-lookup"><span data-stu-id="7dbba-109">Security group</span></span>

<span data-ttu-id="7dbba-110">Dieser Vorgang gibt standardmäßig nur eine Teilmenge der Eigenschaften für jede Gruppe zurück.</span><span class="sxs-lookup"><span data-stu-id="7dbba-110">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="7dbba-111">Diese Standardeigenschaften werden im Abschnitt [Eigenschaften](../resources/group.md#properties) aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="7dbba-111">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span>

<span data-ttu-id="7dbba-112">Um Eigenschaften abzurufen, die _nicht_ standardmäßig zurückgegeben werden, führen Sie eine GET-Operation aus, und geben Sie die Eigenschaften in einer OData-Abfrageoption `$select` an.</span><span class="sxs-lookup"><span data-stu-id="7dbba-112">To get properties that are _not_ returned by default, do a GET operation and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="7dbba-113">Sehen Sie sich das [Beispiel](group-get.md#request-2) an.</span><span class="sxs-lookup"><span data-stu-id="7dbba-113">See an [example](group-get.md#request-2).</span></span>

> <span data-ttu-id="7dbba-114">**Hinweis**: Zum Erstellen eines [Teams](../resources/team.md) erstellen Sie zuerst eine Gruppe und fügen ihr dann ein Team hinzu (siehe [Team erstellen](../api/team-put-teams.md)).</span><span class="sxs-lookup"><span data-stu-id="7dbba-114">**Note**: To create a [team](../resources/team.md), first create a group then add a team to it, see [create team](../api/team-put-teams.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7dbba-115">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7dbba-115">Permissions</span></span>
<span data-ttu-id="7dbba-p105">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7dbba-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7dbba-118">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7dbba-118">Permission type</span></span>      | <span data-ttu-id="7dbba-119">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7dbba-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7dbba-120">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7dbba-120">Delegated (work or school account)</span></span> | <span data-ttu-id="7dbba-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7dbba-121">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7dbba-122">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7dbba-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7dbba-123">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7dbba-123">Not supported.</span></span>    |
|<span data-ttu-id="7dbba-124">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7dbba-124">Application</span></span> | <span data-ttu-id="7dbba-125">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7dbba-125">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7dbba-126">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7dbba-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="7dbba-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7dbba-127">Request headers</span></span>
| <span data-ttu-id="7dbba-128">Name</span><span class="sxs-lookup"><span data-stu-id="7dbba-128">Name</span></span>       | <span data-ttu-id="7dbba-129">Typ</span><span class="sxs-lookup"><span data-stu-id="7dbba-129">Type</span></span> | <span data-ttu-id="7dbba-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7dbba-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7dbba-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="7dbba-131">Authorization</span></span>  | <span data-ttu-id="7dbba-132">string</span><span class="sxs-lookup"><span data-stu-id="7dbba-132">string</span></span>  | <span data-ttu-id="7dbba-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7dbba-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7dbba-135">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7dbba-135">Request body</span></span>
<span data-ttu-id="7dbba-136">Die folgende Tabelle enthält die Eigenschaften der [group](../resources/group.md)-Ressource, die Sie beim Erstellen einer Gruppe angeben müssen.</span><span class="sxs-lookup"><span data-stu-id="7dbba-136">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="7dbba-137">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7dbba-137">Property</span></span> | <span data-ttu-id="7dbba-138">Typ</span><span class="sxs-lookup"><span data-stu-id="7dbba-138">Type</span></span> | <span data-ttu-id="7dbba-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7dbba-139">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7dbba-140">displayName</span><span class="sxs-lookup"><span data-stu-id="7dbba-140">displayName</span></span> | <span data-ttu-id="7dbba-141">string</span><span class="sxs-lookup"><span data-stu-id="7dbba-141">string</span></span> | <span data-ttu-id="7dbba-142">Der Name der Gruppe, der im Adressbuch angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="7dbba-142">The name to display in the address book for the group.</span></span> <span data-ttu-id="7dbba-143">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7dbba-143">Required.</span></span> |
| <span data-ttu-id="7dbba-144">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="7dbba-144">mailEnabled</span></span> | <span data-ttu-id="7dbba-145">boolean</span><span class="sxs-lookup"><span data-stu-id="7dbba-145">boolean</span></span> | <span data-ttu-id="7dbba-146">**true** für E-Mail-aktivierte Gruppen.</span><span class="sxs-lookup"><span data-stu-id="7dbba-146">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="7dbba-147">**true**, wenn eine Office 365-Gruppe erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="7dbba-147">Set this to **true** if creating an Office 365 Group.</span></span> <span data-ttu-id="7dbba-148">**false**, wenn eine dynamische oder eine Sicherheitsgruppe erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="7dbba-148">Set this to **false** if creating dynamic or security group.</span></span> <span data-ttu-id="7dbba-149">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7dbba-149">Required.</span></span> |
| <span data-ttu-id="7dbba-150">mailNickname</span><span class="sxs-lookup"><span data-stu-id="7dbba-150">mailNickname</span></span> | <span data-ttu-id="7dbba-151">string</span><span class="sxs-lookup"><span data-stu-id="7dbba-151">string</span></span> | <span data-ttu-id="7dbba-152">Der E-Mail-Alias für die Gruppe.</span><span class="sxs-lookup"><span data-stu-id="7dbba-152">The mail alias for the group.</span></span> <span data-ttu-id="7dbba-153">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7dbba-153">Required.</span></span> |
| <span data-ttu-id="7dbba-154">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="7dbba-154">securityEnabled</span></span> | <span data-ttu-id="7dbba-155">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7dbba-155">boolean</span></span> | <span data-ttu-id="7dbba-156">**true** für Gruppen mit aktivierter Sicherheit.</span><span class="sxs-lookup"><span data-stu-id="7dbba-156">Set to **true** for security-enabled groups.</span></span> <span data-ttu-id="7dbba-157">**true**, wenn eine dynamische oder eine Sicherheitsgruppe erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="7dbba-157">Set this to **true** if creating a dynamic or security group.</span></span> <span data-ttu-id="7dbba-158">**false**, wenn eine Office 365-Gruppe erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="7dbba-158">Set this to **false** if creating an Office 365 Group.</span></span> <span data-ttu-id="7dbba-159">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7dbba-159">Required.</span></span> |
| <span data-ttu-id="7dbba-160">owners</span><span class="sxs-lookup"><span data-stu-id="7dbba-160">owners</span></span> | <span data-ttu-id="7dbba-161">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="7dbba-161">string collection</span></span> | <span data-ttu-id="7dbba-162">Diese Eigenschaft stellt die Besitzer für die Gruppe zum Zeitpunkt der Erstellung dar.</span><span class="sxs-lookup"><span data-stu-id="7dbba-162">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="7dbba-163">Optional.</span><span class="sxs-lookup"><span data-stu-id="7dbba-163">Optional.</span></span> |
| <span data-ttu-id="7dbba-164">members</span><span class="sxs-lookup"><span data-stu-id="7dbba-164">members</span></span> | <span data-ttu-id="7dbba-165">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="7dbba-165">string collection</span></span> | <span data-ttu-id="7dbba-166">Diese Eigenschaft stellt die Mitglieder der Gruppe zum Zeitpunkt der Erstellung dar.</span><span class="sxs-lookup"><span data-stu-id="7dbba-166">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="7dbba-167">Optional.</span><span class="sxs-lookup"><span data-stu-id="7dbba-167">Optional.</span></span> |

<span data-ttu-id="7dbba-168">Geben Sie die **groupTypes**-Eigenschaft an, wenn Sie eine Office 365- oder eine dynamische Gruppe erstellen, wie unten beschrieben.</span><span class="sxs-lookup"><span data-stu-id="7dbba-168">Specify the **groupTypes** property if you're creating an Office 365 or dynamic group, as stated below.</span></span>

| <span data-ttu-id="7dbba-169">Art der Gruppe</span><span class="sxs-lookup"><span data-stu-id="7dbba-169">Type of group</span></span> | <span data-ttu-id="7dbba-170">**groupTypes**-Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7dbba-170">**groupTypes** property</span></span> |
|:--------------|:------------------------|
| <span data-ttu-id="7dbba-171">Office 365 (auch einheitliche Gruppe genannt)</span><span class="sxs-lookup"><span data-stu-id="7dbba-171">Office 365 (aka unified group)</span></span>| <span data-ttu-id="7dbba-172">„Unified“</span><span class="sxs-lookup"><span data-stu-id="7dbba-172">"Unified"</span></span> |
| <span data-ttu-id="7dbba-173">Dynamisch</span><span class="sxs-lookup"><span data-stu-id="7dbba-173">Dynamic</span></span> | <span data-ttu-id="7dbba-174">"DynamicMembership"</span><span class="sxs-lookup"><span data-stu-id="7dbba-174">"DynamicMembership"</span></span> |
| <span data-ttu-id="7dbba-175">Sicherheit</span><span class="sxs-lookup"><span data-stu-id="7dbba-175">Security</span></span> | <span data-ttu-id="7dbba-176">Nicht festlegen.</span><span class="sxs-lookup"><span data-stu-id="7dbba-176">Do not set.</span></span> |

<span data-ttu-id="7dbba-177">Da die **group**-Ressource [Erweiterungen](/graph/extensibility-overview) unterstützt, können Sie den `POST`-Vorgang verwenden und beim Erstellen der Gruppe benutzerdefinierte Eigenschaften mit Ihren eigenen Daten hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="7dbba-177">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the group while creating it.</span></span>

><span data-ttu-id="7dbba-178">**Hinweis:** Beim programmgesteuerten Erstellen einer Office 365-Gruppe ohne Benutzerkontext und ohne Angabe von Besitzern wird die Gruppe anonym erstellt.</span><span class="sxs-lookup"><span data-stu-id="7dbba-178">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="7dbba-179">Dies kann dazu führen, dass die zugehörige SharePoint Online-Website nicht automatisch erstellt wird und weitere manuelle Aktionen nötig sind.</span><span class="sxs-lookup"><span data-stu-id="7dbba-179">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="7dbba-p114">Geben Sie bei Bedarf andere beschreibbare Eigenschaften für Ihre Gruppe an. Weitere Informationen finden Sie in Themen zu Eigenschaften der [group](../resources/group.md)-Ressource.</span><span class="sxs-lookup"><span data-stu-id="7dbba-p114">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="7dbba-182">Antwort</span><span class="sxs-lookup"><span data-stu-id="7dbba-182">Response</span></span>
<span data-ttu-id="7dbba-183">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [group](../resources/group.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7dbba-183">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="7dbba-184">Die Antwort enthält nur die Standardeigenschaften der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="7dbba-184">The response includes only the default properties of the group.</span></span>

## <a name="example"></a><span data-ttu-id="7dbba-185">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7dbba-185">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="7dbba-186">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="7dbba-186">Request 1</span></span>
<span data-ttu-id="7dbba-187">Die erste Beispielanfrage erstellt eine Office 365-Gruppe.</span><span class="sxs-lookup"><span data-stu-id="7dbba-187">The first example request creates an Office 365 Group.</span></span>
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

#### <a name="response"></a><span data-ttu-id="7dbba-188">Antwort</span><span class="sxs-lookup"><span data-stu-id="7dbba-188">Response</span></span>
<span data-ttu-id="7dbba-189">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7dbba-189">The following is an example of the response.</span></span>
><span data-ttu-id="7dbba-190">**Hinweis:**  Das hier gezeigte Antwortobjekt ist möglicherweise zur besseren Lesbarkeit gekürzt worden.</span><span class="sxs-lookup"><span data-stu-id="7dbba-190">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7dbba-191">Von einem tatsächlichen Aufruf werden alle Standardeigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7dbba-191">All the default properties are returned from an actual call.</span></span>
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

#### <a name="request-2"></a><span data-ttu-id="7dbba-192">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="7dbba-192">Request 2</span></span>
<span data-ttu-id="7dbba-193">Die zweite Beispielanfrage erstellt eine Office 365-Gruppe mit einem angegebenen Besitzer und Mitgliedern.</span><span class="sxs-lookup"><span data-stu-id="7dbba-193">The second example request creates an Office 365 group with an owner and members specified.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_prepopulated_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups
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
    "https://graph.microsoft.com/beta/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ],
  "members@odata.bind": [
    "https://graph.microsoft.com/beta/users/ff7cb387-6688-423c-8188-3da9532a73cc",
    "https://graph.microsoft.com/beta/users/69456242-0067-49d3-ba96-9de6f2728e14"
  ]
}
```

#### <a name="response-2"></a><span data-ttu-id="7dbba-194">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="7dbba-194">Response 2</span></span>
<span data-ttu-id="7dbba-195">Es folgt ein Beispiel für eine erfolgreiche Antwort.</span><span class="sxs-lookup"><span data-stu-id="7dbba-195">The following is an example of a successful response.</span></span> <span data-ttu-id="7dbba-196">Es enthält nur Standardeigenschaften.</span><span class="sxs-lookup"><span data-stu-id="7dbba-196">It includes only default properties.</span></span> <span data-ttu-id="7dbba-197">Sie können anschließend die **owners**- oder **members**-Navigationseigenschaft der Gruppe abrufen, um den Besitzer oder die Mitglieder zu überprüfen.</span><span class="sxs-lookup"><span data-stu-id="7dbba-197">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 
><span data-ttu-id="7dbba-198">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="7dbba-198">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7dbba-199">Von einem tatsächlichen Aufruf werden alle Standardeigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7dbba-199">All the default properties are returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
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

## <a name="see-also"></a><span data-ttu-id="7dbba-200">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="7dbba-200">See also</span></span>

- [<span data-ttu-id="7dbba-201">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="7dbba-201">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="7dbba-202">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="7dbba-202">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="7dbba-203">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="7dbba-203">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-post-groups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
