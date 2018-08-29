# <a name="update-rule"></a><span data-ttu-id="d9d7f-101">Regel aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d9d7f-101">Update rule</span></span>


<span data-ttu-id="d9d7f-102">Ändern Sie die schreibbaren Eigenschaften in einem [messageRule](../resources/messagerule.md)-Objekt, und speichern Sie die Änderungen.</span><span class="sxs-lookup"><span data-stu-id="d9d7f-102">Change writable properties on a [messageRule](../resources/messagerule.md) object and save the changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9d7f-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d9d7f-103">Permissions</span></span>
<span data-ttu-id="d9d7f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d9d7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d9d7f-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d9d7f-106">Permission type</span></span>      | <span data-ttu-id="d9d7f-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d9d7f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9d7f-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d9d7f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="d9d7f-109">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d9d7f-109">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="d9d7f-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d9d7f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9d7f-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d9d7f-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="d9d7f-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d9d7f-112">Application</span></span> | <span data-ttu-id="d9d7f-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d9d7f-113">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9d7f-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d9d7f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/inbox/messageRules/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/inbox/messageRules/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="d9d7f-115">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d9d7f-115">Optional request headers</span></span>
| <span data-ttu-id="d9d7f-116">Name</span><span class="sxs-lookup"><span data-stu-id="d9d7f-116">Name</span></span>       | <span data-ttu-id="d9d7f-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d9d7f-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d9d7f-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="d9d7f-118">Authorization</span></span>  | <span data-ttu-id="d9d7f-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d9d7f-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="d9d7f-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d9d7f-121">Request body</span></span>
<span data-ttu-id="d9d7f-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="d9d7f-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d9d7f-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d9d7f-125">Property</span></span>     | <span data-ttu-id="d9d7f-126">Typ</span><span class="sxs-lookup"><span data-stu-id="d9d7f-126">Type</span></span>   |<span data-ttu-id="d9d7f-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d9d7f-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d9d7f-128">Aktionen</span><span class="sxs-lookup"><span data-stu-id="d9d7f-128">actions</span></span> | [<span data-ttu-id="d9d7f-129">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="d9d7f-129">messageRuleActions</span></span>](../resources/messageruleactions.md) | <span data-ttu-id="d9d7f-130">Aktionen, die auf eine Nachricht angewendet werden, wenn die entsprechenden Bedingungen erfüllt sind.</span><span class="sxs-lookup"><span data-stu-id="d9d7f-130">Actions to be taken on a message when the corresponding conditions are fulfilled.</span></span> |
| <span data-ttu-id="d9d7f-131">Bedingungen</span><span class="sxs-lookup"><span data-stu-id="d9d7f-131">conditions</span></span> | [<span data-ttu-id="d9d7f-132">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="d9d7f-132">messageRulePredicates</span></span>](../resources/messagerulepredicates.md) | <span data-ttu-id="d9d7f-133">Bedingungen, die bei Erfüllung die entsprechenden Aktionen für diese Regel auslösen.</span><span class="sxs-lookup"><span data-stu-id="d9d7f-133">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> |
| <span data-ttu-id="d9d7f-134">displayName</span><span class="sxs-lookup"><span data-stu-id="d9d7f-134">displayName</span></span> | <span data-ttu-id="d9d7f-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d9d7f-135">String</span></span> | <span data-ttu-id="d9d7f-136">Der Anzeigename der Regel.</span><span class="sxs-lookup"><span data-stu-id="d9d7f-136">The display name of the rule.</span></span> |
| <span data-ttu-id="d9d7f-137">Ausnahmen</span><span class="sxs-lookup"><span data-stu-id="d9d7f-137">exceptions</span></span> | [<span data-ttu-id="d9d7f-138">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="d9d7f-138">messageRulePredicates</span></span>](../resources/messagerulepredicates.md) | <span data-ttu-id="d9d7f-139">Ausnahmebedingungen für die Regel.</span><span class="sxs-lookup"><span data-stu-id="d9d7f-139">Exception conditions for the rule.</span></span> |
| <span data-ttu-id="d9d7f-140">isEnabled</span><span class="sxs-lookup"><span data-stu-id="d9d7f-140">isEnabled</span></span> | <span data-ttu-id="d9d7f-141">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d9d7f-141">Boolean</span></span> | <span data-ttu-id="d9d7f-142">Gibt an, ob die Regel auf Nachrichten angewendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="d9d7f-142">Indicates whether the rule is enabled to be applied to messages.</span></span> |
| <span data-ttu-id="d9d7f-143">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="d9d7f-143">isReadOnly</span></span> | <span data-ttu-id="d9d7f-144">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d9d7f-144">Boolean</span></span> | <span data-ttu-id="d9d7f-145">Gibt an, ob die Regel schreibgeschützt ist und von der Regel-REST-API nicht geändert oder gelöscht werden kann.</span><span class="sxs-lookup"><span data-stu-id="d9d7f-145">Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.</span></span> |
| <span data-ttu-id="d9d7f-146">sequence</span><span class="sxs-lookup"><span data-stu-id="d9d7f-146">sequence</span></span> | <span data-ttu-id="d9d7f-147">Int32</span><span class="sxs-lookup"><span data-stu-id="d9d7f-147">Int32</span></span> | <span data-ttu-id="d9d7f-148">Gibt die Reihenfolge an, in der die Regel zusammen mit anderen Regeln ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="d9d7f-148">Indicates the order in which the rule is executed, among other rules.</span></span> |


## <a name="response"></a><span data-ttu-id="d9d7f-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="d9d7f-149">Response</span></span>
<span data-ttu-id="d9d7f-150">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [messageRule](../resources/messagerule.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d9d7f-150">If successful, this method returns a `200 OK` response code and updated [messageRule](../resources/messagerule.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d9d7f-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d9d7f-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d9d7f-152">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d9d7f-152">Request</span></span>
<span data-ttu-id="d9d7f-153">Im folgenden Beispiel werden der Name der Regel sowie die Aktionen, die für diese Regel ausgeführt werden sollen, im [Beispiel](messagerule_get.md#example) in [Regel abrufen](messagerule_get.md) von der Weiterleitung an eine Adresse zur Markierung ihrer Wichtigkeit in „Hoch“ geändert.</span><span class="sxs-lookup"><span data-stu-id="d9d7f-153">The following example changes the name of the rule, and the actions to be taken for that rule in the [example](messagerule_get.md#example) in [Get rule](messagerule_get.md), from forwarding to an address to marking its importance as high.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox", "AQAAAJ5dZqA="],
  "name": "update_messagerule"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules/AQAAAJ5dZqA=
Content-type: application/json

{
    "displayName": "Important from partner",
    "actions": {
        "markImportance": "high"
     }
} 
```
##### <a name="response"></a><span data-ttu-id="d9d7f-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="d9d7f-154">Response</span></span>
<span data-ttu-id="d9d7f-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d9d7f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.messageRule"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Me/mailFolders('inbox')/messageRules/$entity",
  "id":"AQAAAJ5dZqA=",
  "displayName":"Important from partner",
  "sequence":2,
  "isEnabled":true,
  "hasError":false,
  "isReadOnly":false,
  "conditions":{
    "senderContains":[
      "ADELE"
    ]
  },
  "actions":{
    "markImportance": "high"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->