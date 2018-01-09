# <a name="update-group"></a><span data-ttu-id="66935-101">Gruppe aktualisieren</span><span class="sxs-lookup"><span data-stu-id="66935-101">Update group</span></span>
<span data-ttu-id="66935-102">Mit dieser API können Sie die Eigenschaften eines Gruppenobjekts aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="66935-102">Update the properties of a group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="66935-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="66935-103">Permissions</span></span>
<span data-ttu-id="66935-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="66935-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="66935-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="66935-106">Permission type</span></span>      | <span data-ttu-id="66935-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="66935-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66935-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="66935-108">Delegated (work or school account)</span></span> | <span data-ttu-id="66935-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66935-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="66935-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="66935-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66935-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="66935-111">Not supported.</span></span>    |
|<span data-ttu-id="66935-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="66935-112">Application</span></span> | <span data-ttu-id="66935-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66935-113">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="66935-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="66935-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="66935-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="66935-115">Request headers</span></span>

| <span data-ttu-id="66935-116">Name</span><span class="sxs-lookup"><span data-stu-id="66935-116">Name</span></span>       | <span data-ttu-id="66935-117">Typ</span><span class="sxs-lookup"><span data-stu-id="66935-117">Type</span></span> | <span data-ttu-id="66935-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="66935-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="66935-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="66935-119">Authorization</span></span>  | <span data-ttu-id="66935-120">string</span><span class="sxs-lookup"><span data-stu-id="66935-120">string</span></span>  | <span data-ttu-id="66935-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="66935-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="66935-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="66935-123">Request body</span></span>

<span data-ttu-id="66935-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="66935-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="66935-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="66935-127">Property</span></span>     | <span data-ttu-id="66935-128">Typ</span><span class="sxs-lookup"><span data-stu-id="66935-128">Type</span></span>   |<span data-ttu-id="66935-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="66935-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66935-130">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="66935-130">autoSubscribeNewMembers</span></span>|<span data-ttu-id="66935-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="66935-131">Boolean</span></span>|<span data-ttu-id="66935-p104">Der Standardwert ist **false**. Zeigt an, ob neu zur Gruppe hinzugefügte Mitglieder automatisch E-Mail-Benachrichtigungen erhalten.</span><span class="sxs-lookup"><span data-stu-id="66935-p104">Default is **false**. Indicates if new members added to the group will be auto-subscribed to receive email notifications.</span></span>|
|<span data-ttu-id="66935-134">description</span><span class="sxs-lookup"><span data-stu-id="66935-134">description</span></span>|<span data-ttu-id="66935-135">String</span><span class="sxs-lookup"><span data-stu-id="66935-135">String</span></span>|<span data-ttu-id="66935-136">Eine optionale Beschreibung für die Gruppe.</span><span class="sxs-lookup"><span data-stu-id="66935-136">An optional description for the group.</span></span> |
|<span data-ttu-id="66935-137">displayName</span><span class="sxs-lookup"><span data-stu-id="66935-137">displayName</span></span>|<span data-ttu-id="66935-138">String</span><span class="sxs-lookup"><span data-stu-id="66935-138">String</span></span>|<span data-ttu-id="66935-p105">Der Anzeigename der Gruppe. Diese Eigenschaft ist beim Erstellen einer Gruppe erforderlich und kann bei Updates nicht deaktiviert werden. Unterstützt $Filter und $orderby.</span><span class="sxs-lookup"><span data-stu-id="66935-p105">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="66935-142">groupTypes</span><span class="sxs-lookup"><span data-stu-id="66935-142">groupTypes</span></span>|<span data-ttu-id="66935-143">String collection</span><span class="sxs-lookup"><span data-stu-id="66935-143">String collection</span></span>|<span data-ttu-id="66935-p106">Gibt den Typ der zu erstellenden Gruppe an. Mögliche Werte sind **Unified** zum Erstellen einer Office 365-Gruppe oder **DynamicMembership** für dynamische Gruppen.  Legen Sie für alle anderen Gruppentypen wie Gruppen mit aktivierter Sicherheit und E-Mail-aktivierte Sicherheitsgruppen diese Eigenschaft nicht fest.</span><span class="sxs-lookup"><span data-stu-id="66935-p106">Specifies the type of group to create. Possible values are **Unified** to create an Office 365 group, or **DynamicMembership** for dynamic groups.  For all other group types, like security-enabled groups and email-enabled security groups, do not set this property.</span></span>|
|<span data-ttu-id="66935-147">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="66935-147">mailEnabled</span></span>|<span data-ttu-id="66935-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="66935-148">Boolean</span></span>|<span data-ttu-id="66935-p107">Gibt an, ob es sich bei der Gruppe um eine E-Mail-fähige Gruppe handelt. Wenn die **securityEnabled**-Eigenschaft auch auf **true** festgelegt ist, handelt es sich bei der Gruppe um eine E-Mail-fähige Sicherheitsgruppe; andernfalls handelt es sich bei der Gruppe um eine Microsoft Exchange-Verteilergruppe.</span><span class="sxs-lookup"><span data-stu-id="66935-p107">Specifies whether the group is mail-enabled. If the **securityEnabled** property is also **true**, the group is a mail-enabled security group; otherwise, the group is a Microsoft Exchange distribution group.</span></span>|
|<span data-ttu-id="66935-151">mailNickname</span><span class="sxs-lookup"><span data-stu-id="66935-151">mailNickname</span></span>|<span data-ttu-id="66935-152">String</span><span class="sxs-lookup"><span data-stu-id="66935-152">String</span></span>|<span data-ttu-id="66935-p108">Der E-Mail-Alias für die Gruppe. Diese Eigenschaft muss beim Erstellen einer Gruppe angegeben werden. Unterstützt $filter.</span><span class="sxs-lookup"><span data-stu-id="66935-p108">The mail alias for the group. This property must be specified when a group is created. Supports $filter.</span></span>|
|<span data-ttu-id="66935-156">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="66935-156">securityEnabled</span></span>|<span data-ttu-id="66935-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="66935-157">Boolean</span></span>|<span data-ttu-id="66935-p109">Gibt an, ob es sich bei der Gruppe um eine Sicherheitsgruppe handelt. Wenn die **mailEnabled**-Eigenschaft auch auf „true“ festgelegt ist, handelt es sich bei der Gruppe um eine E-Mail-aktivierte Sicherheitsgruppe; andernfalls ist die Gruppe eine Sicherheitsgruppe. Muss für Office 365-Gruppen auf **false** festgelegt sein. Unterstützt $filter.</span><span class="sxs-lookup"><span data-stu-id="66935-p109">Specifies whether the group is a security group. If the **mailEnabled** property is also true, the group is a mail-enabled security group; otherwise it is a security group. Must be **false** for Office 365 groups. Supports $filter..</span></span>|
|<span data-ttu-id="66935-162">visibility</span><span class="sxs-lookup"><span data-stu-id="66935-162">visibility</span></span>|<span data-ttu-id="66935-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="66935-163">Boolean</span></span>|<span data-ttu-id="66935-p110">Gibt die Sichtbarkeit einer Office 365-Gruppe an. Die folgenden Werte sind möglich: **Private**, **Public** oder leer (als **öffentlich** interpretiert).</span><span class="sxs-lookup"><span data-stu-id="66935-p110">Specifies the visibility of an Office 365 group. Possible values are: **Private**, **Public**, or empty (which is interpreted as **Public**).</span></span>|

<span data-ttu-id="66935-166">**Hinweis**</span><span class="sxs-lookup"><span data-stu-id="66935-166">**Note**</span></span>

- <span data-ttu-id="66935-167">Sie können **autoSubscribeNewMembers** aktualisieren, indem Sie diese Eigenschaft in ihrer eigenen PATCH-Anforderung angeben, ohne die anderen Eigenschaften in der Tabelle oben einzuschließen.</span><span class="sxs-lookup"><span data-stu-id="66935-167">You can update **autoSubscribeNewMembers** by specifying it in its own PATCH request, without including the other properties in the table above.</span></span>
- <span data-ttu-id="66935-p111">Nur eine Teilmenge der Gruppen-API, die zur Hauptgruppenadministration und -verwaltung gehören, unterstützen Anwendungs- und delegierte Berechtigungen. Alle anderen Mitglieder der Gruppen-API, einschließlich des Aktualisierens von **autoSubscribeNewMembers**, unterstützen nur delegierte Berechtigungen. Beispiele finden Sie unter [Bekannte Probleme](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes).</span><span class="sxs-lookup"><span data-stu-id="66935-p111">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions. All other members of the group API, including updating  **autoSubscribeNewMembers**, support only delegated permissions. See [known issues](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes) for examples.</span></span>

## <a name="response"></a><span data-ttu-id="66935-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="66935-171">Response</span></span>
<span data-ttu-id="66935-172">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="66935-172">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="66935-173">Beispiel</span><span class="sxs-lookup"><span data-stu-id="66935-173">Example</span></span>

#### <a name="request"></a><span data-ttu-id="66935-174">Anforderung</span><span class="sxs-lookup"><span data-stu-id="66935-174">Request</span></span>
<span data-ttu-id="66935-175">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="66935-175">The following is an example of making the request in ASP.NET that uses the TokenHelper file:</span></span>
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

#### <a name="response"></a><span data-ttu-id="66935-176">Antwort</span><span class="sxs-lookup"><span data-stu-id="66935-176">Response</span></span>
<span data-ttu-id="66935-177">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="66935-177">Here is an example of the response.</span></span>
><span data-ttu-id="66935-178">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="66935-178">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="66935-179">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="66935-179">All the properties will be returned from an actual call.</span></span>
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