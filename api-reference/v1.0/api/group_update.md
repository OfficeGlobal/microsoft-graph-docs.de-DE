# <a name="update-group"></a><span data-ttu-id="274f4-101">Gruppe aktualisieren</span><span class="sxs-lookup"><span data-stu-id="274f4-101">Update group</span></span>

<span data-ttu-id="274f4-102">Aktualisieren Sie die Eigenschaften eines Gruppenobjekts.</span><span class="sxs-lookup"><span data-stu-id="274f4-102">Update the properties of a group object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="274f4-103">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="274f4-103">Prerequisites</span></span>
<span data-ttu-id="274f4-104">Der folgende **Bereich** ist erforderlich, um diese API auszuführen: *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="274f4-104">The following **scope** is required to execute this API: *Group.ReadWrite.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="274f4-105">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="274f4-105">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="274f4-106">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="274f4-106">Request headers</span></span>

| <span data-ttu-id="274f4-107">Name</span><span class="sxs-lookup"><span data-stu-id="274f4-107">Name</span></span>       | <span data-ttu-id="274f4-108">Typ</span><span class="sxs-lookup"><span data-stu-id="274f4-108">Type</span></span> | <span data-ttu-id="274f4-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="274f4-109">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="274f4-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="274f4-110">Authorization</span></span>  | <span data-ttu-id="274f4-111">string</span><span class="sxs-lookup"><span data-stu-id="274f4-111">string</span></span>  | <span data-ttu-id="274f4-p101">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="274f4-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="274f4-114">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="274f4-114">Request body</span></span>

<span data-ttu-id="274f4-p102">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="274f4-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="274f4-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="274f4-118">Property</span></span>     | <span data-ttu-id="274f4-119">Typ</span><span class="sxs-lookup"><span data-stu-id="274f4-119">Type</span></span>   |<span data-ttu-id="274f4-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="274f4-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="274f4-121">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="274f4-121">autoSubscribeNewMembers</span></span>|<span data-ttu-id="274f4-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="274f4-122">Boolean</span></span>|<span data-ttu-id="274f4-p103">Der Standardwert ist **false**. Zeigt an, ob neu zur Gruppe hinzugefügte Mitglieder automatisch E-Mail-Benachrichtigungen erhalten.</span><span class="sxs-lookup"><span data-stu-id="274f4-p103">Default is **false**. Indicates if new members added to the group will be auto-subscribed to receive email notifications.</span></span>|
|<span data-ttu-id="274f4-125">description</span><span class="sxs-lookup"><span data-stu-id="274f4-125">description</span></span>|<span data-ttu-id="274f4-126">String</span><span class="sxs-lookup"><span data-stu-id="274f4-126">String</span></span>|<span data-ttu-id="274f4-127">Eine optionale Beschreibung für die Gruppe.</span><span class="sxs-lookup"><span data-stu-id="274f4-127">An optional description for the group.</span></span> |
|<span data-ttu-id="274f4-128">displayName</span><span class="sxs-lookup"><span data-stu-id="274f4-128">displayName</span></span>|<span data-ttu-id="274f4-129">String</span><span class="sxs-lookup"><span data-stu-id="274f4-129">String</span></span>|<span data-ttu-id="274f4-p104">Der Anzeigename der Gruppe. Diese Eigenschaft ist beim Erstellen einer Gruppe erforderlich und kann bei Updates nicht deaktiviert werden. Unterstützt $Filter und $orderby.</span><span class="sxs-lookup"><span data-stu-id="274f4-p104">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="274f4-133">groupTypes</span><span class="sxs-lookup"><span data-stu-id="274f4-133">groupTypes</span></span>|<span data-ttu-id="274f4-134">String collection</span><span class="sxs-lookup"><span data-stu-id="274f4-134">String collection</span></span>|<span data-ttu-id="274f4-p105">Gibt den Typ der zu erstellenden Gruppe an. Mögliche Werte sind **Unified** zum Erstellen einer Office 365-Gruppe oder **DynamicMembership** für dynamische Gruppen.  Legen Sie für alle anderen Gruppentypen wie Gruppen mit aktivierter Sicherheit und E-Mail-aktivierte Sicherheitsgruppen diese Eigenschaft nicht fest.</span><span class="sxs-lookup"><span data-stu-id="274f4-p105">Specifies the type of group to create. Possible values are **Unified** to create an Office 365 group, or **DynamicMembership** for dynamic groups.  For all other group types, like security-enabled groups and email-enabled security groups, do not set this property.</span></span>|
|<span data-ttu-id="274f4-138">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="274f4-138">mailEnabled</span></span>|<span data-ttu-id="274f4-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="274f4-139">Boolean</span></span>|<span data-ttu-id="274f4-p106">Gibt an, ob es sich bei der Gruppe um eine E-Mail-fähige Gruppe handelt. Wenn die **securityEnabled**-Eigenschaft auch auf **true** festgelegt ist, handelt es sich bei der Gruppe um eine E-Mail-fähige Sicherheitsgruppe; andernfalls handelt es sich bei der Gruppe um eine Microsoft Exchange-Verteilergruppe.</span><span class="sxs-lookup"><span data-stu-id="274f4-p106">Specifies whether the group is mail-enabled. If the **securityEnabled** property is also **true**, the group is a mail-enabled security group; otherwise, the group is a Microsoft Exchange distribution group.</span></span>|
|<span data-ttu-id="274f4-142">mailNickname</span><span class="sxs-lookup"><span data-stu-id="274f4-142">mailNickname</span></span>|<span data-ttu-id="274f4-143">String</span><span class="sxs-lookup"><span data-stu-id="274f4-143">String</span></span>|<span data-ttu-id="274f4-p107">Der E-Mail-Alias für die Gruppe. Diese Eigenschaft muss beim Erstellen einer Gruppe angegeben werden. Unterstützt $filter.</span><span class="sxs-lookup"><span data-stu-id="274f4-p107">The mail alias for the group. This property must be specified when a group is created. Supports $filter.</span></span>|
|<span data-ttu-id="274f4-147">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="274f4-147">securityEnabled</span></span>|<span data-ttu-id="274f4-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="274f4-148">Boolean</span></span>|<span data-ttu-id="274f4-p108">Gibt an, ob es sich bei der Gruppe um eine Sicherheitsgruppe handelt. Wenn die **mailEnabled**-Eigenschaft auch auf „true“ festgelegt ist, handelt es sich bei der Gruppe um eine E-Mail-aktivierte Sicherheitsgruppe; andernfalls ist die Gruppe eine Sicherheitsgruppe. Muss für Office 365-Gruppen auf **false** festgelegt sein. Unterstützt $filter.</span><span class="sxs-lookup"><span data-stu-id="274f4-p108">Specifies whether the group is a security group. If the **mailEnabled** property is also true, the group is a mail-enabled security group; otherwise it is a security group. Must be **false** for Office 365 groups. Supports $filter..</span></span>|
|<span data-ttu-id="274f4-153">visibility</span><span class="sxs-lookup"><span data-stu-id="274f4-153">visibility</span></span>|<span data-ttu-id="274f4-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="274f4-154">Boolean</span></span>|<span data-ttu-id="274f4-p109">Gibt die Sichtbarkeit einer Office 365-Gruppe an. Die folgenden Werte sind möglich: **Private**, **Public** oder leer (als **Public** interpretiert).</span><span class="sxs-lookup"><span data-stu-id="274f4-p109">Specifies the visibility of an Office 365 group. Possible values are: **Private**, **Public**, or empty (which is interpreted as **Public**).</span></span>|

<span data-ttu-id="274f4-157">**Hinweis**</span><span class="sxs-lookup"><span data-stu-id="274f4-157">**Note**</span></span>

- <span data-ttu-id="274f4-158">Sie können **autoSubscribeNewMembers** aktualisieren, indem Sie diese Eigenschaft in ihrer eigenen PATCH-Anforderung angeben, ohne die anderen Eigenschaften in der Tabelle oben einzuschließen.</span><span class="sxs-lookup"><span data-stu-id="274f4-158">You can update **autoSubscribeNewMembers** by specifying it in its own PATCH request, without including the other properties in the table above.</span></span>
- <span data-ttu-id="274f4-p110">Nur eine Teilmenge der Gruppen-API, die zur Hauptgruppenadministration und -verwaltung gehören, unterstützen Anwendungs- und delegierte Berechtigungen. Alle anderen Mitglieder der Gruppen-API, einschließlich des Aktualisierens von **autoSubscribeNewMembers**, unterstützen nur delegierte Berechtigungen. Beispiele finden Sie unter [Bekannte Probleme](https://developer.microsoft.com/en-us/graph/docs/overview/release_notes#group-permission-scopes).</span><span class="sxs-lookup"><span data-stu-id="274f4-p110">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions. All other members of the group API, including updating  **autoSubscribeNewMembers**, support only delegated permissions. See [known issues](https://developer.microsoft.com/en-us/graph/docs/overview/release_notes#group-permission-scopes) for examples.</span></span>

## <a name="response"></a><span data-ttu-id="274f4-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="274f4-162">Response</span></span>

<span data-ttu-id="274f4-163">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="274f4-163">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="274f4-164">Beispiel</span><span class="sxs-lookup"><span data-stu-id="274f4-164">Example</span></span>

##### <a name="request"></a><span data-ttu-id="274f4-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="274f4-165">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_group"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/{id}
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

##### <a name="response"></a><span data-ttu-id="274f4-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="274f4-166">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->