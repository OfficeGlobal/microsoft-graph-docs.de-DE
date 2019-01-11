---
title: Gruppe erstellen
description: 'Verwenden Sie diese API zum Erstellen einer neuen Gruppe gemäß der Angabe im Anforderungstext. Sie können drei Typen von Gruppen erstellen:'
author: dkershaw10
localization_priority: Priority
ms.openlocfilehash: 5876c1c327cd1095124675046089a0f8a71a7ca0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887640"
---
# <a name="create-group"></a><span data-ttu-id="23735-104">Gruppe erstellen</span><span class="sxs-lookup"><span data-stu-id="23735-104">Create group</span></span>

> <span data-ttu-id="23735-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="23735-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="23735-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="23735-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="23735-107">Verwenden Sie diese API zum Erstellen einer neuen [Gruppe](../resources/group.md) wie im Textkörper Anforderung angegeben.</span><span class="sxs-lookup"><span data-stu-id="23735-107">Use this API to create a new [group](../resources/group.md) as specified in the request body.</span></span> <span data-ttu-id="23735-108">Sie können eine der drei Arten von Gruppen erstellen:</span><span class="sxs-lookup"><span data-stu-id="23735-108">You can create one of three types of groups:</span></span>

* <span data-ttu-id="23735-109">Office 365-Gruppe (einheitliche Gruppe)</span><span class="sxs-lookup"><span data-stu-id="23735-109">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="23735-110">Dynamische Gruppe</span><span class="sxs-lookup"><span data-stu-id="23735-110">Dynamic group</span></span>
* <span data-ttu-id="23735-111">Sicherheitsgruppe</span><span class="sxs-lookup"><span data-stu-id="23735-111">Security group</span></span>

> <span data-ttu-id="23735-112">**Hinweis**: zum Erstellen ein [Team](../resources/team.md), zuerst erstellen Sie eine Gruppe, dann fügen Sie ein Team hinzu, finden Sie unter [Team erstellen](../api/team-put-teams.md).</span><span class="sxs-lookup"><span data-stu-id="23735-112">**Note**: To create a [team](../resources/team.md), first create a group then add a team to it, see [create team](../api/team-put-teams.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="23735-113">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="23735-113">Permissions</span></span>
<span data-ttu-id="23735-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23735-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23735-116">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="23735-116">Permission type</span></span>      | <span data-ttu-id="23735-117">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="23735-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23735-118">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="23735-118">Delegated (work or school account)</span></span> | <span data-ttu-id="23735-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23735-119">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="23735-120">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="23735-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23735-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="23735-121">Not supported.</span></span>    |
|<span data-ttu-id="23735-122">Anwendung</span><span class="sxs-lookup"><span data-stu-id="23735-122">Application</span></span> | <span data-ttu-id="23735-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23735-123">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="23735-124">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="23735-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="23735-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="23735-125">Request headers</span></span>
| <span data-ttu-id="23735-126">Name</span><span class="sxs-lookup"><span data-stu-id="23735-126">Name</span></span>       | <span data-ttu-id="23735-127">Typ</span><span class="sxs-lookup"><span data-stu-id="23735-127">Type</span></span> | <span data-ttu-id="23735-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="23735-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="23735-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="23735-129">Authorization</span></span>  | <span data-ttu-id="23735-130">string</span><span class="sxs-lookup"><span data-stu-id="23735-130">string</span></span>  | <span data-ttu-id="23735-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="23735-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="23735-133">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="23735-133">Request body</span></span>
<span data-ttu-id="23735-134">Die folgende Tabelle zeigt die Eigenschaften des [Group](../resources/group.md) -Ressource angeben, wenn Sie eine Gruppe zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="23735-134">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="23735-135">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="23735-135">Property</span></span> | <span data-ttu-id="23735-136">Typ</span><span class="sxs-lookup"><span data-stu-id="23735-136">Type</span></span> | <span data-ttu-id="23735-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="23735-137">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="23735-138">displayName</span><span class="sxs-lookup"><span data-stu-id="23735-138">displayName</span></span> | <span data-ttu-id="23735-139">string</span><span class="sxs-lookup"><span data-stu-id="23735-139">string</span></span> | <span data-ttu-id="23735-140">Der Name der Gruppe, der im Adressbuch angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="23735-140">The name to display in the address book for the group.</span></span> <span data-ttu-id="23735-141">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="23735-141">Required.</span></span> |
| <span data-ttu-id="23735-142">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="23735-142">mailEnabled</span></span> | <span data-ttu-id="23735-143">boolean</span><span class="sxs-lookup"><span data-stu-id="23735-143">boolean</span></span> | <span data-ttu-id="23735-144">**true** für E-Mail-aktivierte Gruppen.</span><span class="sxs-lookup"><span data-stu-id="23735-144">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="23735-145">Legen Sie dies auf **true** fest, wenn eine Office 365-Gruppe zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="23735-145">Set this to **true** if creating an Office 365 Group.</span></span> <span data-ttu-id="23735-146">Festlegen Sie diese Eigenschaft auf **"false"** Wenn dynamische Erstellen oder Sicherheitsgruppe.</span><span class="sxs-lookup"><span data-stu-id="23735-146">Set this to **false** if creating dynamic or security group.</span></span> <span data-ttu-id="23735-147">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="23735-147">Required.</span></span> |
| <span data-ttu-id="23735-148">mailNickname</span><span class="sxs-lookup"><span data-stu-id="23735-148">mailNickname</span></span> | <span data-ttu-id="23735-149">string</span><span class="sxs-lookup"><span data-stu-id="23735-149">string</span></span> | <span data-ttu-id="23735-150">Der E-Mail-Alias für die Gruppe.</span><span class="sxs-lookup"><span data-stu-id="23735-150">The mail alias for the group.</span></span> <span data-ttu-id="23735-151">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="23735-151">Required.</span></span> |
| <span data-ttu-id="23735-152">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="23735-152">securityEnabled</span></span> | <span data-ttu-id="23735-153">boolean</span><span class="sxs-lookup"><span data-stu-id="23735-153">boolean</span></span> | <span data-ttu-id="23735-154">Festgelegt auf **true** für Sicherheit-aktivierte Gruppen.</span><span class="sxs-lookup"><span data-stu-id="23735-154">Set to **true** for security-enabled groups.</span></span> <span data-ttu-id="23735-155">Legen Sie dies auf **true** fest, wenn eine dynamische oder eine Sicherheitsgruppe an erstellen.</span><span class="sxs-lookup"><span data-stu-id="23735-155">Set this to **true** if creating a dynamic or security group.</span></span> <span data-ttu-id="23735-156">Legen Sie dies auf **false fest** , wenn eine Office 365-Gruppe zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="23735-156">Set this to **false** if creating an Office 365 Group.</span></span> <span data-ttu-id="23735-157">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="23735-157">Required.</span></span> |
| <span data-ttu-id="23735-158">owners</span><span class="sxs-lookup"><span data-stu-id="23735-158">owners</span></span> | <span data-ttu-id="23735-159">string collection</span><span class="sxs-lookup"><span data-stu-id="23735-159">string collection</span></span> | <span data-ttu-id="23735-160">Diese Eigenschaft stellt den Besitzer für die Gruppe zum Zeitpunkt der Erstellung.</span><span class="sxs-lookup"><span data-stu-id="23735-160">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="23735-161">Optional.</span><span class="sxs-lookup"><span data-stu-id="23735-161">Optional.</span></span> |
| <span data-ttu-id="23735-162">Elemente</span><span class="sxs-lookup"><span data-stu-id="23735-162">members</span></span> | <span data-ttu-id="23735-163">string collection</span><span class="sxs-lookup"><span data-stu-id="23735-163">string collection</span></span> | <span data-ttu-id="23735-164">Diese Eigenschaft stellt die Mitglieder der Gruppe zum Zeitpunkt der Erstellung.</span><span class="sxs-lookup"><span data-stu-id="23735-164">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="23735-165">Optional.</span><span class="sxs-lookup"><span data-stu-id="23735-165">Optional.</span></span> |

<span data-ttu-id="23735-166">Geben Sie die **groupTypes** Eigenschaft an, wenn Sie eine Office 365 oder eine dynamische Gruppe erstellen, wie unten beschrieben.</span><span class="sxs-lookup"><span data-stu-id="23735-166">Specify the **groupTypes** property if you're creating an Office 365 or dynamic group, as stated below.</span></span>

| <span data-ttu-id="23735-167">Art der Gruppe</span><span class="sxs-lookup"><span data-stu-id="23735-167">Type of group</span></span> | <span data-ttu-id="23735-168">**groupTypes**-Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="23735-168">**groupTypes** property</span></span> |
|:--------------|:------------------------|
| <span data-ttu-id="23735-169">Office 365 (auch einheitliche Gruppe genannt)</span><span class="sxs-lookup"><span data-stu-id="23735-169">Office 365 (aka unified group)</span></span>| <span data-ttu-id="23735-170">„Unified“</span><span class="sxs-lookup"><span data-stu-id="23735-170">"Unified"</span></span> |
| <span data-ttu-id="23735-171">Dynamisch</span><span class="sxs-lookup"><span data-stu-id="23735-171">Dynamic</span></span> | <span data-ttu-id="23735-172">"DynamicMembership"</span><span class="sxs-lookup"><span data-stu-id="23735-172">"DynamicMembership"</span></span> |
| <span data-ttu-id="23735-173">Sicherheit</span><span class="sxs-lookup"><span data-stu-id="23735-173">Security</span></span> | <span data-ttu-id="23735-174">Nicht festlegen.</span><span class="sxs-lookup"><span data-stu-id="23735-174">Do not set.</span></span> |

<span data-ttu-id="23735-175">Da die **Group** -Ressource [Extensions](/graph/extensibility-overview)unterstützt, können Sie die `POST` Vorgang und benutzerdefinierte Eigenschaften mit Ihren eigenen Daten beim Erstellen der Gruppe hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="23735-175">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the group while creating it.</span></span>

><span data-ttu-id="23735-176">**Hinweis:** Erstellen einer Office 365-Gruppe programmgesteuert ohne einen Benutzerkontext und ohne Angabe von Besitzer erstellt die Gruppe anonym.</span><span class="sxs-lookup"><span data-stu-id="23735-176">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="23735-177">Dies kann führen, dass in der zugehörigen SharePoint Online-Website nicht automatisch erstellt werden, bis eine zusätzliche manuelle Aktion ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="23735-177">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="23735-p113">Geben Sie bei Bedarf andere beschreibbare Eigenschaften für Ihre Gruppe an. Weitere Informationen finden Sie in Themen zu Eigenschaften der [group](../resources/group.md)-Ressource.</span><span class="sxs-lookup"><span data-stu-id="23735-p113">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="23735-180">Antwort</span><span class="sxs-lookup"><span data-stu-id="23735-180">Response</span></span>
<span data-ttu-id="23735-181">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [group](../resources/group.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="23735-181">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23735-182">Beispiel</span><span class="sxs-lookup"><span data-stu-id="23735-182">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="23735-183">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="23735-183">Request 1</span></span>
<span data-ttu-id="23735-184">Die erste beispielanforderung erstellt eine Office 365-Gruppe.</span><span class="sxs-lookup"><span data-stu-id="23735-184">The first example request creates an Office 365 Group.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups
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

#### <a name="response"></a><span data-ttu-id="23735-185">Antwort</span><span class="sxs-lookup"><span data-stu-id="23735-185">Response</span></span>
<span data-ttu-id="23735-186">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="23735-186">The following is an example of the response.</span></span>
><span data-ttu-id="23735-187">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="23735-187">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="23735-188">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="23735-188">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 244

{
  "description": "Self help community for library",
  "displayName": "Library Assist",
  "groupTypes": [
    "Unified"
  ],
  "mail": "library@contoso.onmicrosoft.com",
  "mailEnabled": true,
  "mailNickname": "library",
  "securityEnabled": false
}
```

#### <a name="request-2"></a><span data-ttu-id="23735-189">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="23735-189">Request 2</span></span>
<span data-ttu-id="23735-190">Die zweite beispielanforderung erstellt eine Office 365-Gruppe mit Besitzer angegeben.</span><span class="sxs-lookup"><span data-stu-id="23735-190">The second example request creates an Office 365 Group with owners specified.</span></span>
<!-- {
  "blockType": "request"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups
Content-Type: application/json
 {
  "description": "Group with owners",
  "displayName": "Group1",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "group1",
  "securityEnabled": false,
  "owners@odata.bind": [
    "https://graph.microsoft.com/v1.0/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ]
}
```

 #### <a name="response-2"></a><span data-ttu-id="23735-191">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="23735-191">Response 2</span></span>
<span data-ttu-id="23735-192">Es folgt ein Beispiel für die erfolgreiche Antwort.</span><span class="sxs-lookup"><span data-stu-id="23735-192">The following is an example of the successful response.</span></span>
><span data-ttu-id="23735-p115">**Hinweis:** Das hier gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="23735-p115">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
 {
    "description": "Group with owners",
    "displayName": "Group1",
    "groupTypes": [
        "Unified"
    ],
    "mail": "group1@contoso.onmicrosoft.com",
    "mailEnabled": true,
    "mailNickname": "group1",
    "securityEnabled": false
}
```

## <a name="see-also"></a><span data-ttu-id="23735-195">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="23735-195">See also</span></span>

- [<span data-ttu-id="23735-196">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="23735-196">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="23735-197">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="23735-197">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="23735-198">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="23735-198">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
