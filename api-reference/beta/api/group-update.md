---
title: Gruppe aktualisieren
description: Mit dieser API können Sie die Eigenschaften eines Gruppenobjekts aktualisieren.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: f1f86067771a4732c8839f48bc02dd3edd15c19b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915235"
---
# <a name="update-group"></a><span data-ttu-id="91098-103">Gruppe aktualisieren</span><span class="sxs-lookup"><span data-stu-id="91098-103">Update group</span></span>

> <span data-ttu-id="91098-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="91098-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91098-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="91098-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="91098-106">Aktualisieren Sie die Eigenschaften eines [Group](../resources/group.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="91098-106">Update the properties of a [group](../resources/group.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="91098-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="91098-107">Permissions</span></span>

<span data-ttu-id="91098-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91098-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91098-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="91098-110">Permission type</span></span>      | <span data-ttu-id="91098-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="91098-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91098-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="91098-112">Delegated (work or school account)</span></span> | <span data-ttu-id="91098-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91098-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="91098-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="91098-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91098-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="91098-115">Not supported.</span></span>    |
|<span data-ttu-id="91098-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="91098-116">Application</span></span> | <span data-ttu-id="91098-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91098-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="91098-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="91098-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="91098-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="91098-119">Request headers</span></span>

| <span data-ttu-id="91098-120">Name</span><span class="sxs-lookup"><span data-stu-id="91098-120">Name</span></span>       | <span data-ttu-id="91098-121">Typ</span><span class="sxs-lookup"><span data-stu-id="91098-121">Type</span></span> | <span data-ttu-id="91098-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="91098-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="91098-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="91098-123">Authorization</span></span>  | <span data-ttu-id="91098-124">string</span><span class="sxs-lookup"><span data-stu-id="91098-124">string</span></span>  | <span data-ttu-id="91098-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="91098-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="91098-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="91098-127">Request body</span></span>

<span data-ttu-id="91098-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="91098-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="91098-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="91098-131">Property</span></span>   | <span data-ttu-id="91098-132">Typ</span><span class="sxs-lookup"><span data-stu-id="91098-132">Type</span></span> |<span data-ttu-id="91098-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="91098-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="91098-134">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="91098-134">allowExternalSenders</span></span>|<span data-ttu-id="91098-135">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="91098-135">Boolean</span></span>|<span data-ttu-id="91098-p105">Der Standardwert ist **false**. Gibt an, ob Personen außerhalb der Organisation Nachrichten an die Gruppe senden können.</span><span class="sxs-lookup"><span data-stu-id="91098-p105">Default is **false**. Indicates if people external to the organization can send messages to the group.</span></span>|
|<span data-ttu-id="91098-138">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="91098-138">autoSubscribeNewMembers</span></span>|<span data-ttu-id="91098-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="91098-139">Boolean</span></span>|<span data-ttu-id="91098-p106">Der Standardwert ist **false**. Zeigt an, ob neu zur Gruppe hinzugefügte Mitglieder automatisch E-Mail-Benachrichtigungen erhalten.</span><span class="sxs-lookup"><span data-stu-id="91098-p106">Default is **false**. Indicates if new members added to the group will be auto-subscribed to receive email notifications.</span></span>|
|<span data-ttu-id="91098-142">description</span><span class="sxs-lookup"><span data-stu-id="91098-142">description</span></span>|<span data-ttu-id="91098-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="91098-143">String</span></span>|<span data-ttu-id="91098-144">Eine optionale Beschreibung für die Gruppe.</span><span class="sxs-lookup"><span data-stu-id="91098-144">An optional description for the group.</span></span> |
|<span data-ttu-id="91098-145">displayName</span><span class="sxs-lookup"><span data-stu-id="91098-145">displayName</span></span>|<span data-ttu-id="91098-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="91098-146">String</span></span>|<span data-ttu-id="91098-p107">Der Anzeigename der Gruppe. Diese Eigenschaft ist beim Erstellen einer Gruppe erforderlich und kann bei Updates nicht deaktiviert werden. Unterstützt $Filter und $orderby.</span><span class="sxs-lookup"><span data-stu-id="91098-p107">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="91098-150">groupTypes</span><span class="sxs-lookup"><span data-stu-id="91098-150">groupTypes</span></span>|<span data-ttu-id="91098-151">String collection</span><span class="sxs-lookup"><span data-stu-id="91098-151">String collection</span></span>|<span data-ttu-id="91098-p108">Gibt den Typ der zu erstellenden Gruppe an. Mögliche Werte sind **Unified** zum Erstellen einer Office 365-Gruppe oder **DynamicMembership** für dynamische Gruppen.  Legen Sie für alle anderen Gruppentypen wie Gruppen mit aktivierter Sicherheit und E-Mail-aktivierte Sicherheitsgruppen diese Eigenschaft nicht fest.</span><span class="sxs-lookup"><span data-stu-id="91098-p108">Specifies the type of group to create. Possible values are **Unified** to create an Office 365 group, or **DynamicMembership** for dynamic groups.  For all other group types, like security-enabled groups and email-enabled security groups, do not set this property.</span></span>|
|<span data-ttu-id="91098-155">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="91098-155">mailEnabled</span></span>|<span data-ttu-id="91098-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="91098-156">Boolean</span></span>|<span data-ttu-id="91098-p109">Gibt an, ob es sich bei der Gruppe um eine E-Mail-fähige Gruppe handelt. Wenn die **securityEnabled**-Eigenschaft auch auf **true** festgelegt ist, handelt es sich bei der Gruppe um eine E-Mail-fähige Sicherheitsgruppe; andernfalls handelt es sich bei der Gruppe um eine Microsoft Exchange-Verteilergruppe.</span><span class="sxs-lookup"><span data-stu-id="91098-p109">Specifies whether the group is mail-enabled. If the **securityEnabled** property is also **true**, the group is a mail-enabled security group; otherwise, the group is a Microsoft Exchange distribution group.</span></span>|
|<span data-ttu-id="91098-159">mailNickname</span><span class="sxs-lookup"><span data-stu-id="91098-159">mailNickname</span></span>|<span data-ttu-id="91098-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="91098-160">String</span></span>|<span data-ttu-id="91098-p110">Der E-Mail-Alias für die Gruppe. Diese Eigenschaft muss beim Erstellen einer Gruppe angegeben werden. Unterstützt $filter.</span><span class="sxs-lookup"><span data-stu-id="91098-p110">The mail alias for the group. This property must be specified when a group is created. Supports $filter.</span></span>|
|<span data-ttu-id="91098-164">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="91098-164">securityEnabled</span></span>|<span data-ttu-id="91098-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="91098-165">Boolean</span></span>|<span data-ttu-id="91098-p111">Gibt an, ob es sich bei der Gruppe um eine Sicherheitsgruppe handelt. Wenn die **mailEnabled**-Eigenschaft auch auf „true“ festgelegt ist, handelt es sich bei der Gruppe um eine E-Mail-aktivierte Sicherheitsgruppe; andernfalls ist die Gruppe eine Sicherheitsgruppe. Muss für Office 365-Gruppen auf **false** festgelegt sein. Unterstützt $filter.</span><span class="sxs-lookup"><span data-stu-id="91098-p111">Specifies whether the group is a security group. If the **mailEnabled** property is also true, the group is a mail-enabled security group; otherwise it is a security group. Must be **false** for Office 365 groups. Supports $filter..</span></span>|
|<span data-ttu-id="91098-170">visibility</span><span class="sxs-lookup"><span data-stu-id="91098-170">visibility</span></span>|<span data-ttu-id="91098-171">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="91098-171">String</span></span>|<span data-ttu-id="91098-p112">Gibt die Sichtbarkeit einer Office 365-Gruppe an. Die folgenden Werte sind möglich: **Private**, **Public** oder leer (als **öffentlich** interpretiert).</span><span class="sxs-lookup"><span data-stu-id="91098-p112">Specifies the visibility of an Office 365 group. Possible values are: **Private**, **Public**, or empty (which is interpreted as **Public**).</span></span>|

<span data-ttu-id="91098-174">Da die **Group** -Ressource [Extensions](/graph/extensibility-overview)unterstützt, können Sie die `PATCH` Vorgang hinzufügen, aktualisieren oder Löschen von Ihren eigenen app-spezifischen Daten in benutzerdefinierten Eigenschaften einer Erweiterung in einer vorhandenen **Gruppe** -Instanz.</span><span class="sxs-lookup"><span data-stu-id="91098-174">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **group** instance.</span></span>

> <span data-ttu-id="91098-175">**Hinweis:**</span><span class="sxs-lookup"><span data-stu-id="91098-175">**Note:**</span></span>
>
> - <span data-ttu-id="91098-176">Sie können **autoSubscribeNewMembers** aktualisieren, indem Sie diese Eigenschaft in ihrer eigenen PATCH-Anforderung angeben, ohne die anderen Eigenschaften in der Tabelle oben einzuschließen.</span><span class="sxs-lookup"><span data-stu-id="91098-176">You can update **autoSubscribeNewMembers** by specifying it in its own PATCH request, without including the other properties in the table above.</span></span>
> - <span data-ttu-id="91098-p113">Nur eine Teilmenge der Gruppen-API, die zur Hauptgruppenadministration und -verwaltung gehören, unterstützen Anwendungs- und delegierte Berechtigungen. Alle anderen Mitglieder der Gruppen-API, einschließlich des Aktualisierens von **autoSubscribeNewMembers**, unterstützen nur delegierte Berechtigungen. Beispiele finden Sie unter [Bekannte Probleme](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes).</span><span class="sxs-lookup"><span data-stu-id="91098-p113">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions. All other members of the group API, including updating  **autoSubscribeNewMembers**, support only delegated permissions. See [known issues](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes) for examples.</span></span>

## <a name="response"></a><span data-ttu-id="91098-180">Antwort</span><span class="sxs-lookup"><span data-stu-id="91098-180">Response</span></span>

<span data-ttu-id="91098-181">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="91098-181">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="91098-182">Beispiel</span><span class="sxs-lookup"><span data-stu-id="91098-182">Example</span></span>

#### <a name="request"></a><span data-ttu-id="91098-183">Anforderung</span><span class="sxs-lookup"><span data-stu-id="91098-183">Request</span></span>

<span data-ttu-id="91098-184">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="91098-184">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="91098-185">Antwort</span><span class="sxs-lookup"><span data-stu-id="91098-185">Response</span></span>

<span data-ttu-id="91098-186">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="91098-186">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="91098-187">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="91098-187">See also</span></span>

- [<span data-ttu-id="91098-188">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="91098-188">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="91098-189">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="91098-189">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="91098-190">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="91098-190">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
