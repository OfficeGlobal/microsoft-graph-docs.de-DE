---
title: Gruppe aktualisieren
description: Mit dieser API können Sie die Eigenschaften eines Gruppenobjekts aktualisieren.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: c60ff8eaf95401c5c3e8eb44017d9a6d37ac0ea4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520634"
---
# <a name="update-group"></a><span data-ttu-id="5e1a9-103">Gruppe aktualisieren</span><span class="sxs-lookup"><span data-stu-id="5e1a9-103">Update group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e1a9-104">Aktualisieren Sie die Eigenschaften eines [Group](../resources/group.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="5e1a9-104">Update the properties of a [group](../resources/group.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5e1a9-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5e1a9-105">Permissions</span></span>

<span data-ttu-id="5e1a9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e1a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e1a9-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5e1a9-108">Permission type</span></span>      | <span data-ttu-id="5e1a9-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5e1a9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e1a9-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5e1a9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5e1a9-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e1a9-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5e1a9-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5e1a9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e1a9-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5e1a9-113">Not supported.</span></span>    |
|<span data-ttu-id="5e1a9-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5e1a9-114">Application</span></span> | <span data-ttu-id="5e1a9-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e1a9-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5e1a9-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5e1a9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5e1a9-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5e1a9-117">Request headers</span></span>

| <span data-ttu-id="5e1a9-118">Name</span><span class="sxs-lookup"><span data-stu-id="5e1a9-118">Name</span></span>       | <span data-ttu-id="5e1a9-119">Typ</span><span class="sxs-lookup"><span data-stu-id="5e1a9-119">Type</span></span> | <span data-ttu-id="5e1a9-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5e1a9-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5e1a9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e1a9-121">Authorization</span></span>  | <span data-ttu-id="5e1a9-122">string</span><span class="sxs-lookup"><span data-stu-id="5e1a9-122">string</span></span>  | <span data-ttu-id="5e1a9-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5e1a9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5e1a9-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5e1a9-125">Request body</span></span>

<span data-ttu-id="5e1a9-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="5e1a9-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5e1a9-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5e1a9-129">Property</span></span>   | <span data-ttu-id="5e1a9-130">Typ</span><span class="sxs-lookup"><span data-stu-id="5e1a9-130">Type</span></span> |<span data-ttu-id="5e1a9-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5e1a9-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e1a9-132">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="5e1a9-132">allowExternalSenders</span></span>|<span data-ttu-id="5e1a9-133">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="5e1a9-133">Boolean</span></span>|<span data-ttu-id="5e1a9-p104">Der Standardwert ist **false**. Gibt an, ob Personen außerhalb der Organisation Nachrichten an die Gruppe senden können.</span><span class="sxs-lookup"><span data-stu-id="5e1a9-p104">Default is **false**. Indicates if people external to the organization can send messages to the group.</span></span>|
|<span data-ttu-id="5e1a9-136">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="5e1a9-136">autoSubscribeNewMembers</span></span>|<span data-ttu-id="5e1a9-137">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="5e1a9-137">Boolean</span></span>|<span data-ttu-id="5e1a9-p105">Der Standardwert ist **false**. Zeigt an, ob neu zur Gruppe hinzugefügte Mitglieder automatisch E-Mail-Benachrichtigungen erhalten.</span><span class="sxs-lookup"><span data-stu-id="5e1a9-p105">Default is **false**. Indicates if new members added to the group will be auto-subscribed to receive email notifications.</span></span>|
|<span data-ttu-id="5e1a9-140">description</span><span class="sxs-lookup"><span data-stu-id="5e1a9-140">description</span></span>|<span data-ttu-id="5e1a9-141">String</span><span class="sxs-lookup"><span data-stu-id="5e1a9-141">String</span></span>|<span data-ttu-id="5e1a9-142">Eine optionale Beschreibung für die Gruppe.</span><span class="sxs-lookup"><span data-stu-id="5e1a9-142">An optional description for the group.</span></span> |
|<span data-ttu-id="5e1a9-143">displayName</span><span class="sxs-lookup"><span data-stu-id="5e1a9-143">displayName</span></span>|<span data-ttu-id="5e1a9-144">String</span><span class="sxs-lookup"><span data-stu-id="5e1a9-144">String</span></span>|<span data-ttu-id="5e1a9-p106">Der Anzeigename der Gruppe. Diese Eigenschaft ist beim Erstellen einer Gruppe erforderlich und kann bei Updates nicht deaktiviert werden. Unterstützt $Filter und $orderby.</span><span class="sxs-lookup"><span data-stu-id="5e1a9-p106">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="5e1a9-148">groupTypes</span><span class="sxs-lookup"><span data-stu-id="5e1a9-148">groupTypes</span></span>|<span data-ttu-id="5e1a9-149">String collection</span><span class="sxs-lookup"><span data-stu-id="5e1a9-149">String collection</span></span>|<span data-ttu-id="5e1a9-p107">Gibt den Typ der zu erstellenden Gruppe an. Mögliche Werte sind **Unified** zum Erstellen einer Office 365-Gruppe oder **DynamicMembership** für dynamische Gruppen.  Legen Sie für alle anderen Gruppentypen wie Gruppen mit aktivierter Sicherheit und E-Mail-aktivierte Sicherheitsgruppen diese Eigenschaft nicht fest.</span><span class="sxs-lookup"><span data-stu-id="5e1a9-p107">Specifies the type of group to create. Possible values are **Unified** to create an Office 365 group, or **DynamicMembership** for dynamic groups.  For all other group types, like security-enabled groups and email-enabled security groups, do not set this property.</span></span>|
|<span data-ttu-id="5e1a9-153">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="5e1a9-153">mailEnabled</span></span>|<span data-ttu-id="5e1a9-154">Boolesch</span><span class="sxs-lookup"><span data-stu-id="5e1a9-154">Boolean</span></span>|<span data-ttu-id="5e1a9-p108">Gibt an, ob es sich bei der Gruppe um eine E-Mail-fähige Gruppe handelt. Wenn die **securityEnabled**-Eigenschaft auch auf **true** festgelegt ist, handelt es sich bei der Gruppe um eine E-Mail-fähige Sicherheitsgruppe; andernfalls handelt es sich bei der Gruppe um eine Microsoft Exchange-Verteilergruppe.</span><span class="sxs-lookup"><span data-stu-id="5e1a9-p108">Specifies whether the group is mail-enabled. If the **securityEnabled** property is also **true**, the group is a mail-enabled security group; otherwise, the group is a Microsoft Exchange distribution group.</span></span>|
|<span data-ttu-id="5e1a9-157">mailNickname</span><span class="sxs-lookup"><span data-stu-id="5e1a9-157">mailNickname</span></span>|<span data-ttu-id="5e1a9-158">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5e1a9-158">String</span></span>|<span data-ttu-id="5e1a9-p109">Der E-Mail-Alias für die Gruppe. Diese Eigenschaft muss beim Erstellen einer Gruppe angegeben werden. Unterstützt $filter.</span><span class="sxs-lookup"><span data-stu-id="5e1a9-p109">The mail alias for the group. This property must be specified when a group is created. Supports $filter.</span></span>|
|<span data-ttu-id="5e1a9-162">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="5e1a9-162">securityEnabled</span></span>|<span data-ttu-id="5e1a9-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e1a9-163">Boolean</span></span>|<span data-ttu-id="5e1a9-p110">Gibt an, ob es sich bei der Gruppe um eine Sicherheitsgruppe handelt. Wenn die **mailEnabled**-Eigenschaft auch auf „true“ festgelegt ist, handelt es sich bei der Gruppe um eine E-Mail-aktivierte Sicherheitsgruppe; andernfalls ist die Gruppe eine Sicherheitsgruppe. Muss für Office 365-Gruppen auf **false** festgelegt sein. Unterstützt $filter.</span><span class="sxs-lookup"><span data-stu-id="5e1a9-p110">Specifies whether the group is a security group. If the **mailEnabled** property is also true, the group is a mail-enabled security group; otherwise it is a security group. Must be **false** for Office 365 groups. Supports $filter..</span></span>|
|<span data-ttu-id="5e1a9-168">visibility</span><span class="sxs-lookup"><span data-stu-id="5e1a9-168">visibility</span></span>|<span data-ttu-id="5e1a9-169">String</span><span class="sxs-lookup"><span data-stu-id="5e1a9-169">String</span></span>|<span data-ttu-id="5e1a9-p111">Gibt die Sichtbarkeit einer Office 365-Gruppe an. Die folgenden Werte sind möglich: **Private**, **Public** oder leer (als **öffentlich** interpretiert).</span><span class="sxs-lookup"><span data-stu-id="5e1a9-p111">Specifies the visibility of an Office 365 group. Possible values are: **Private**, **Public**, or empty (which is interpreted as **Public**).</span></span>|

<span data-ttu-id="5e1a9-172">Da die **Group** -Ressource [Extensions](/graph/extensibility-overview)unterstützt, können Sie die `PATCH` Vorgang hinzufügen, aktualisieren oder Löschen von Ihren eigenen app-spezifischen Daten in benutzerdefinierten Eigenschaften einer Erweiterung in einer vorhandenen **Gruppe** -Instanz.</span><span class="sxs-lookup"><span data-stu-id="5e1a9-172">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **group** instance.</span></span>

> <span data-ttu-id="5e1a9-173">**Hinweis:**</span><span class="sxs-lookup"><span data-stu-id="5e1a9-173">**Note:**</span></span>
>
> - <span data-ttu-id="5e1a9-174">Sie können **autoSubscribeNewMembers** aktualisieren, indem Sie diese Eigenschaft in ihrer eigenen PATCH-Anforderung angeben, ohne die anderen Eigenschaften in der Tabelle oben einzuschließen.</span><span class="sxs-lookup"><span data-stu-id="5e1a9-174">You can update **autoSubscribeNewMembers** by specifying it in its own PATCH request, without including the other properties in the table above.</span></span>
> - <span data-ttu-id="5e1a9-p112">Nur eine Teilmenge der Gruppen-API, die zur Hauptgruppenadministration und -verwaltung gehören, unterstützen Anwendungs- und delegierte Berechtigungen. Alle anderen Mitglieder der Gruppen-API, einschließlich des Aktualisierens von **autoSubscribeNewMembers**, unterstützen nur delegierte Berechtigungen. Beispiele finden Sie unter [Bekannte Probleme](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes).</span><span class="sxs-lookup"><span data-stu-id="5e1a9-p112">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions. All other members of the group API, including updating  **autoSubscribeNewMembers**, support only delegated permissions. See [known issues](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes) for examples.</span></span>

## <a name="response"></a><span data-ttu-id="5e1a9-178">Antwort</span><span class="sxs-lookup"><span data-stu-id="5e1a9-178">Response</span></span>

<span data-ttu-id="5e1a9-179">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5e1a9-179">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5e1a9-180">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5e1a9-180">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5e1a9-181">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5e1a9-181">Request</span></span>

<span data-ttu-id="5e1a9-182">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5e1a9-182">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_group"
}-->

```http
PATCH https://graph.microsoft.com/beta/groups/{id}
Content-type: application/json
Content-length: 211

{
  "description": "description-value",
  "displayName": "displayName-value",
  "groupTypes": [
    "groupTypes-value"
  ],
  "mail": "mail-value",
  "mailEnabled": true,
  "mailNickname": "mailNickname-value"
}
```

#### <a name="response"></a><span data-ttu-id="5e1a9-183">Antwort</span><span class="sxs-lookup"><span data-stu-id="5e1a9-183">Response</span></span>

<span data-ttu-id="5e1a9-184">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5e1a9-184">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="5e1a9-185">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="5e1a9-185">See also</span></span>

- [<span data-ttu-id="5e1a9-186">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="5e1a9-186">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="5e1a9-187">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="5e1a9-187">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="5e1a9-188">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="5e1a9-188">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
