# <a name="create-rule"></a><span data-ttu-id="65f74-101">Regel erstellen</span><span class="sxs-lookup"><span data-stu-id="65f74-101">Create rule</span></span>


<span data-ttu-id="65f74-102">Erstellen Sie ein  [messageRule](../resources/messagerule.md)-Objekt, indem Sie eine Gruppe von Bedingungen und Aktionen angeben.</span><span class="sxs-lookup"><span data-stu-id="65f74-102">Create a [messageRule](../resources/messagerule.md) object by specifying a set of conditions and actions.</span></span> 

<span data-ttu-id="65f74-103">Outlook führt diese Aktionen aus, wenn eine eingehende Nachricht im Posteingang des Benutzers die angegebenen Bedingungen erfüllt.</span><span class="sxs-lookup"><span data-stu-id="65f74-103">Outlook carries out those actions if an incoming message in the user's Inbox meets the specified conditions.</span></span>

## <a name="permissions"></a><span data-ttu-id="65f74-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="65f74-104">Permissions</span></span>
<span data-ttu-id="65f74-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="65f74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="65f74-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="65f74-107">Permission type</span></span>      | <span data-ttu-id="65f74-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="65f74-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="65f74-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="65f74-109">Delegated (work or school account)</span></span> | <span data-ttu-id="65f74-110">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="65f74-110">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="65f74-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="65f74-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65f74-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="65f74-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="65f74-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="65f74-113">Application</span></span> | <span data-ttu-id="65f74-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="65f74-114">MailboxSettings.ReadWrite</span></span> |


## <a name="http-request"></a><span data-ttu-id="65f74-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="65f74-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/inbox/messagerules
POST /users/{id | userPrincipalName}/mailFolders/inbox/messagerules
```
## <a name="request-headers"></a><span data-ttu-id="65f74-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="65f74-116">Request headers</span></span>
| <span data-ttu-id="65f74-117">Name</span><span class="sxs-lookup"><span data-stu-id="65f74-117">Name</span></span>       | <span data-ttu-id="65f74-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="65f74-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="65f74-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="65f74-119">Authorization</span></span>  | <span data-ttu-id="65f74-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="65f74-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="65f74-122">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="65f74-122">Request body</span></span>
<span data-ttu-id="65f74-123">Geben Sie im Anforderungstext die Parameter an, die auf die Regel angewendet werden können.</span><span class="sxs-lookup"><span data-stu-id="65f74-123">In the request body, supply the parameters that are applicable to your rule.</span></span> <span data-ttu-id="65f74-124">Nachfolgend finden Sie die Textparameter, die in der Regel beim Erstellen von Regeln verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="65f74-124">The following are body parameters that are typically used when creating rules.</span></span> <span data-ttu-id="65f74-125">Sie können bei Bedarf im Anforderungstext beliebige andere schreibbare **messageRule**-Eigenschaften angeben.</span><span class="sxs-lookup"><span data-stu-id="65f74-125">You can specify any other writable **messageRule** properties as appropriate in the request body.</span></span>

### <a name="request-parameters"></a><span data-ttu-id="65f74-126">Anforderungsparameter</span><span class="sxs-lookup"><span data-stu-id="65f74-126">Request parameters</span></span>
| <span data-ttu-id="65f74-127">Name</span><span class="sxs-lookup"><span data-stu-id="65f74-127">Name</span></span>       | <span data-ttu-id="65f74-128">Typ</span><span class="sxs-lookup"><span data-stu-id="65f74-128">Type</span></span>|<span data-ttu-id="65f74-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="65f74-129">Description</span></span>|
|:--------|:-------|:----------|
|<span data-ttu-id="65f74-130">Aktionen</span><span class="sxs-lookup"><span data-stu-id="65f74-130">Actions</span></span>|[<span data-ttu-id="65f74-131">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="65f74-131">messageRuleActions</span></span>](../resources/messageruleactions.md)|<span data-ttu-id="65f74-132">Aktionen, die auf eine Nachricht angewendet werden, wenn die entsprechenden Bedingungen (falls vorhanden) erfüllt sind.</span><span class="sxs-lookup"><span data-stu-id="65f74-132">Actions to be taken on a message when the corresponding conditions, if any, are fulfilled.</span></span> <span data-ttu-id="65f74-133">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="65f74-133">Required.</span></span>|
|<span data-ttu-id="65f74-134">Bedingungen</span><span class="sxs-lookup"><span data-stu-id="65f74-134">Conditions</span></span>|[<span data-ttu-id="65f74-135">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="65f74-135">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)|<span data-ttu-id="65f74-136">Bedingungen, die bei Erfüllung die entsprechenden Aktionen für diese Regel auslösen.</span><span class="sxs-lookup"><span data-stu-id="65f74-136">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> <span data-ttu-id="65f74-137">Optional.</span><span class="sxs-lookup"><span data-stu-id="65f74-137">Optional.</span></span>|
|<span data-ttu-id="65f74-138">displayName</span><span class="sxs-lookup"><span data-stu-id="65f74-138">displayName</span></span>| <span data-ttu-id="65f74-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="65f74-139">String</span></span>  | <span data-ttu-id="65f74-140">Der Anzeigename der Regel.</span><span class="sxs-lookup"><span data-stu-id="65f74-140">The name of the new formatting rule.</span></span> <span data-ttu-id="65f74-141">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="65f74-141">Required.</span></span>|
|<span data-ttu-id="65f74-142">Ausnahmen</span><span class="sxs-lookup"><span data-stu-id="65f74-142">exceptions</span></span>| [<span data-ttu-id="65f74-143">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="65f74-143">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)| <span data-ttu-id="65f74-144">Ausnahmebedingungen für die Regel.</span><span class="sxs-lookup"><span data-stu-id="65f74-144">Represents exception conditions for the rule.</span></span> <span data-ttu-id="65f74-145">Optional.</span><span class="sxs-lookup"><span data-stu-id="65f74-145">Optional.</span></span> |
|<span data-ttu-id="65f74-146">isEnabled</span><span class="sxs-lookup"><span data-stu-id="65f74-146">isEnabled</span></span> | <span data-ttu-id="65f74-147">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65f74-147">Boolean</span></span> | <span data-ttu-id="65f74-148">Gibt an, ob die Regel auf Nachrichten angewendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="65f74-148">Indicates whether the rule is enabled to be applied to messages.</span></span> <span data-ttu-id="65f74-149">Optional.</span><span class="sxs-lookup"><span data-stu-id="65f74-149">Optional.</span></span> |
|<span data-ttu-id="65f74-150">sequence</span><span class="sxs-lookup"><span data-stu-id="65f74-150">Sequence</span></span>| <span data-ttu-id="65f74-151">Int32</span><span class="sxs-lookup"><span data-stu-id="65f74-151">Int32</span></span> | <span data-ttu-id="65f74-152">Gibt die Reihenfolge an, in der die Regel zusammen mit anderen Regeln ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="65f74-152">Indicates the order in which the rule is executed, among other rules.</span></span> <span data-ttu-id="65f74-153">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="65f74-153">Required.</span></span>|

## <a name="response"></a><span data-ttu-id="65f74-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="65f74-154">Response</span></span>
<span data-ttu-id="65f74-155">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs **messageRule** im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="65f74-155">If successful, this method returns a `201 Created` response code and a **deviceAndAppManagementRoleDefinition** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65f74-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="65f74-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="65f74-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="65f74-157">Request</span></span>
<span data-ttu-id="65f74-158">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="65f74-158">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_messagerule_from_mailfolder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messagerules
Content-type: application/json

{      
    "displayName": "From partner",      
    "sequence": 2,      
    "isEnabled": true,          
    "conditions": {
        "senderContains": [
          "adele"       
        ]
     },
     "actions": {
        "forwardTo": [
          {
             "emailAddress": {
                "name": "Alex Wilbur",
                "address": "AlexW@contoso.onmicrosoft.com"
              }
           }
        ],
        "stopProcessingRules": true
     }    
}

```
##### <a name="response"></a><span data-ttu-id="65f74-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="65f74-159">Response</span></span>
<span data-ttu-id="65f74-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="65f74-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.messageRule"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id":"AQAAAJ5dZqA=",
  "displayName":"From partner",
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
      "stopProcessingRules":true,
      "forwardTo":[
        {
          "emailAddress":{
            "name":"Alex Wilbur",
            "address":"AlexW@contoso.onmicrosoft.com"
          }
        }
      ]
  }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->