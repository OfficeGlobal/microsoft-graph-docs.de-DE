---
title: Gruppe erstellen
description: 'Verwenden Sie diese API zum Erstellen einer neuen Gruppe gemäß der Angabe im Anforderungstext. Sie können drei Typen von Gruppen erstellen:'
author: dkershaw10
localization_priority: Priority
ms.openlocfilehash: 3f6a73b6fd2dcf76bb1ebd0fab4c02a673a1be8e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849420"
---
# <a name="create-group"></a><span data-ttu-id="0991a-104">Gruppe erstellen</span><span class="sxs-lookup"><span data-stu-id="0991a-104">Create group</span></span>
<span data-ttu-id="0991a-p102">Verwenden Sie diese API zum Erstellen einer neuen Gruppe gemäß der Angabe im Anforderungstext. Sie können drei Typen von Gruppen erstellen:</span><span class="sxs-lookup"><span data-stu-id="0991a-p102">Use this API to create a new group as specified in the request body. You can create one of three types of groups:</span></span>

* <span data-ttu-id="0991a-107">Office 365-Gruppe (einheitliche Gruppe)</span><span class="sxs-lookup"><span data-stu-id="0991a-107">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="0991a-108">Dynamische Gruppe</span><span class="sxs-lookup"><span data-stu-id="0991a-108">Dynamic group</span></span>
* <span data-ttu-id="0991a-109">Sicherheitsgruppe</span><span class="sxs-lookup"><span data-stu-id="0991a-109">Security group</span></span>

> <span data-ttu-id="0991a-p103">**Hinweis**: Microsoft Teams basiert zwar auf Office 365-Gruppen, über diese API kann derzeit aber kein Team erstellt werden. Sie können die anderen Gruppen-APIs verwenden, um ein Team zu verwalten, das in der Microsoft Teams-Benutzeroberfläche erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="0991a-p103">**Note**: Although Microsoft Teams is built on Office 365 Groups, you can't currently create a team via this API. You can use the other group APIs to manage a team that has been created in the Microsoft Teams UI.</span></span>

## <a name="permissions"></a><span data-ttu-id="0991a-112">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0991a-112">Permissions</span></span>
<span data-ttu-id="0991a-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0991a-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0991a-115">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0991a-115">Permission type</span></span>      | <span data-ttu-id="0991a-116">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0991a-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0991a-117">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0991a-117">Delegated (work or school account)</span></span> | <span data-ttu-id="0991a-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0991a-118">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0991a-119">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0991a-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0991a-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0991a-120">Not supported.</span></span>    |
|<span data-ttu-id="0991a-121">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0991a-121">Application</span></span> | <span data-ttu-id="0991a-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0991a-122">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0991a-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0991a-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="0991a-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0991a-124">Request headers</span></span>
| <span data-ttu-id="0991a-125">Name</span><span class="sxs-lookup"><span data-stu-id="0991a-125">Name</span></span>       | <span data-ttu-id="0991a-126">Typ</span><span class="sxs-lookup"><span data-stu-id="0991a-126">Type</span></span> | <span data-ttu-id="0991a-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0991a-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0991a-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="0991a-128">Authorization</span></span>  | <span data-ttu-id="0991a-129">string</span><span class="sxs-lookup"><span data-stu-id="0991a-129">string</span></span>  | <span data-ttu-id="0991a-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0991a-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0991a-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0991a-132">Request body</span></span>
<span data-ttu-id="0991a-133">Die folgende Tabelle zeigt die Eigenschaften des [Group](../resources/group.md) -Ressource angeben, wenn Sie eine Gruppe zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="0991a-133">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="0991a-134">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0991a-134">Property</span></span> | <span data-ttu-id="0991a-135">Typ</span><span class="sxs-lookup"><span data-stu-id="0991a-135">Type</span></span> | <span data-ttu-id="0991a-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0991a-136">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0991a-137">displayName</span><span class="sxs-lookup"><span data-stu-id="0991a-137">displayName</span></span> | <span data-ttu-id="0991a-138">string</span><span class="sxs-lookup"><span data-stu-id="0991a-138">string</span></span> | <span data-ttu-id="0991a-139">Der Name der Gruppe, der im Adressbuch angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="0991a-139">The name to display in the address book for the group.</span></span> <span data-ttu-id="0991a-140">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0991a-140">Required.</span></span> |
| <span data-ttu-id="0991a-141">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="0991a-141">mailEnabled</span></span> | <span data-ttu-id="0991a-142">boolean</span><span class="sxs-lookup"><span data-stu-id="0991a-142">boolean</span></span> | <span data-ttu-id="0991a-143">**true** für E-Mail-aktivierte Gruppen.</span><span class="sxs-lookup"><span data-stu-id="0991a-143">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="0991a-144">Legen Sie dies auf **true** fest, wenn eine Office 365-Gruppe zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="0991a-144">Set this to **true** if creating an Office 365 Group.</span></span> <span data-ttu-id="0991a-145">Festlegen Sie diese Eigenschaft auf **"false"** Wenn dynamische Erstellen oder Sicherheitsgruppe.</span><span class="sxs-lookup"><span data-stu-id="0991a-145">Set this to **false** if creating dynamic or security group.</span></span> <span data-ttu-id="0991a-146">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0991a-146">Required.</span></span> |
| <span data-ttu-id="0991a-147">mailNickname</span><span class="sxs-lookup"><span data-stu-id="0991a-147">mailNickname</span></span> | <span data-ttu-id="0991a-148">string</span><span class="sxs-lookup"><span data-stu-id="0991a-148">string</span></span> | <span data-ttu-id="0991a-149">Der E-Mail-Alias für die Gruppe.</span><span class="sxs-lookup"><span data-stu-id="0991a-149">The mail alias for the group.</span></span> <span data-ttu-id="0991a-150">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0991a-150">Required.</span></span> |
| <span data-ttu-id="0991a-151">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="0991a-151">securityEnabled</span></span> | <span data-ttu-id="0991a-152">boolean</span><span class="sxs-lookup"><span data-stu-id="0991a-152">boolean</span></span> | <span data-ttu-id="0991a-153">Festgelegt auf **true** für Sicherheit-aktivierte Gruppen.</span><span class="sxs-lookup"><span data-stu-id="0991a-153">Set to **true** for security-enabled groups.</span></span> <span data-ttu-id="0991a-154">Legen Sie dies auf **true** fest, wenn eine dynamische oder eine Sicherheitsgruppe an erstellen.</span><span class="sxs-lookup"><span data-stu-id="0991a-154">Set this to **true** if creating a dynamic or security group.</span></span> <span data-ttu-id="0991a-155">Legen Sie dies auf **false fest** , wenn eine Office 365-Gruppe zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="0991a-155">Set this to **false** if creating an Office 365 group.</span></span> <span data-ttu-id="0991a-156">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0991a-156">Required.</span></span> |
| <span data-ttu-id="0991a-157">owners</span><span class="sxs-lookup"><span data-stu-id="0991a-157">owners</span></span> | <span data-ttu-id="0991a-158">string collection</span><span class="sxs-lookup"><span data-stu-id="0991a-158">string collection</span></span> | <span data-ttu-id="0991a-159">Diese Eigenschaft stellt den Besitzer für die Gruppe zum Zeitpunkt der Erstellung.</span><span class="sxs-lookup"><span data-stu-id="0991a-159">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="0991a-160">Optional.</span><span class="sxs-lookup"><span data-stu-id="0991a-160">Optional.</span></span> |
| <span data-ttu-id="0991a-161">Elemente</span><span class="sxs-lookup"><span data-stu-id="0991a-161">members</span></span> | <span data-ttu-id="0991a-162">string collection</span><span class="sxs-lookup"><span data-stu-id="0991a-162">string collection</span></span> | <span data-ttu-id="0991a-163">Diese Eigenschaft stellt die Mitglieder der Gruppe zum Zeitpunkt der Erstellung.</span><span class="sxs-lookup"><span data-stu-id="0991a-163">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="0991a-164">Optional.</span><span class="sxs-lookup"><span data-stu-id="0991a-164">Optional.</span></span> |


<span data-ttu-id="0991a-165">Geben Sie die **groupTypes** Eigenschaft an, wenn Sie eine Office 365 oder eine dynamische Gruppe erstellen, wie unten beschrieben.</span><span class="sxs-lookup"><span data-stu-id="0991a-165">Specify the **groupTypes** property if you're creating an Office 365 or dynamic group, as stated below.</span></span>

### <a name="grouptypes-options"></a><span data-ttu-id="0991a-166">GroupTypes-Optionen</span><span class="sxs-lookup"><span data-stu-id="0991a-166">groupTypes options</span></span>

| <span data-ttu-id="0991a-167">Art der Gruppe</span><span class="sxs-lookup"><span data-stu-id="0991a-167">Type of group</span></span> | <span data-ttu-id="0991a-168">**groupTypes**-Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0991a-168">**groupTypes** property</span></span> |
|:--------------|:------------------------|
| <span data-ttu-id="0991a-169">Office 365 (auch einheitliche Gruppe genannt)</span><span class="sxs-lookup"><span data-stu-id="0991a-169">Office 365 (aka unified group)</span></span>| <span data-ttu-id="0991a-170">„Unified“</span><span class="sxs-lookup"><span data-stu-id="0991a-170">"Unified"</span></span> |
| <span data-ttu-id="0991a-171">Dynamisch</span><span class="sxs-lookup"><span data-stu-id="0991a-171">Dynamic</span></span> | <span data-ttu-id="0991a-172">"DynamicMembership"</span><span class="sxs-lookup"><span data-stu-id="0991a-172">"DynamicMembership"</span></span> |
| <span data-ttu-id="0991a-173">Sicherheit</span><span class="sxs-lookup"><span data-stu-id="0991a-173">Security</span></span> | <span data-ttu-id="0991a-174">Nicht festlegen.</span><span class="sxs-lookup"><span data-stu-id="0991a-174">Do not set.</span></span> |


><span data-ttu-id="0991a-175">**Hinweis:** Erstellen einer Office 365-Gruppe programmgesteuert ohne einen Benutzerkontext und ohne Angabe von Besitzer erstellt die Gruppe anonym.</span><span class="sxs-lookup"><span data-stu-id="0991a-175">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="0991a-176">Dies kann führen, dass in der zugehörigen SharePoint Online-Website nicht automatisch erstellt werden, bis eine zusätzliche manuelle Aktion ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="0991a-176">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="0991a-p113">Geben Sie bei Bedarf andere beschreibbare Eigenschaften für Ihre Gruppe an. Weitere Informationen finden Sie in Themen zu Eigenschaften der [group](../resources/group.md)-Ressource.</span><span class="sxs-lookup"><span data-stu-id="0991a-p113">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="0991a-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="0991a-179">Response</span></span>
<span data-ttu-id="0991a-180">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [group](../resources/group.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0991a-180">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0991a-181">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0991a-181">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="0991a-182">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="0991a-182">Request 1</span></span>
<span data-ttu-id="0991a-183">Die erste beispielanforderung erstellt eine Office 365-Gruppe.</span><span class="sxs-lookup"><span data-stu-id="0991a-183">The first example request creates an Office 365 Group.</span></span>
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

#### <a name="response-1"></a><span data-ttu-id="0991a-184">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="0991a-184">Response 1</span></span>
<span data-ttu-id="0991a-185">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0991a-185">The following is an example of the response.</span></span>
><span data-ttu-id="0991a-186">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="0991a-186">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0991a-187">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="0991a-187">All the properties will be returned from an actual call.</span></span>
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

#### <a name="request-2"></a><span data-ttu-id="0991a-188">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="0991a-188">Request 2</span></span>
<span data-ttu-id="0991a-189">Die zweite beispielanforderung erstellt eine Office 365-Gruppe mit Besitzer angegeben.</span><span class="sxs-lookup"><span data-stu-id="0991a-189">The second example request creates an Office 365 Group with owners specified.</span></span>
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

#### <a name="response-2"></a><span data-ttu-id="0991a-190">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="0991a-190">Response 2</span></span>
<span data-ttu-id="0991a-191">Es folgt ein Beispiel für die erfolgreiche Antwort.</span><span class="sxs-lookup"><span data-stu-id="0991a-191">The following is an example of the successful response.</span></span>
><span data-ttu-id="0991a-192">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="0991a-192">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0991a-193">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="0991a-193">All the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
