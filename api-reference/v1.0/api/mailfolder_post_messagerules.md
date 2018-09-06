# <a name="create-rule"></a><span data-ttu-id="52603-101">Regel erstellen</span><span class="sxs-lookup"><span data-stu-id="52603-101">Create rule</span></span>


<span data-ttu-id="52603-102">Erstellen Sie ein  [messageRule](../resources/messagerule.md)-Objekt, indem Sie eine Gruppe von Bedingungen und Aktionen angeben.</span><span class="sxs-lookup"><span data-stu-id="52603-102">Create a [messageRule](../resources/messagerule.md) object by specifying a set of conditions and actions.</span></span> 

<span data-ttu-id="52603-103">Outlook führt diese Aktionen aus, wenn eine eingehende Nachricht im Posteingang des Benutzers die angegebenen Bedingungen erfüllt.</span><span class="sxs-lookup"><span data-stu-id="52603-103">Outlook carries out those actions if an incoming message in the user's Inbox meets the specified conditions.</span></span>

## <a name="permissions"></a><span data-ttu-id="52603-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="52603-104">Permissions</span></span>
<span data-ttu-id="52603-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="52603-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="52603-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="52603-107">Permission type</span></span>      | <span data-ttu-id="52603-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="52603-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="52603-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="52603-109">Delegated (work or school account)</span></span> | <span data-ttu-id="52603-110">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="52603-110">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="52603-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="52603-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52603-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="52603-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="52603-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="52603-113">Application</span></span> | <span data-ttu-id="52603-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="52603-114">MailboxSettings.ReadWrite</span></span> |


## <a name="http-request"></a><span data-ttu-id="52603-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="52603-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/inbox/messageRules
POST /users/{id | userPrincipalName}/mailFolders/inbox/messageRules
```
## <a name="request-headers"></a><span data-ttu-id="52603-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="52603-116">Request headers</span></span>
| <span data-ttu-id="52603-117">Name</span><span class="sxs-lookup"><span data-stu-id="52603-117">Name</span></span>       | <span data-ttu-id="52603-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="52603-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="52603-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="52603-119">Authorization</span></span>  | <span data-ttu-id="52603-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="52603-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="52603-122">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="52603-122">Request body</span></span>
<span data-ttu-id="52603-123">Geben Sie im Anforderungstext die Parameter an, die auf die Regel angewendet werden können.</span><span class="sxs-lookup"><span data-stu-id="52603-123">In the request body, supply the parameters that are applicable to your rule.</span></span> <span data-ttu-id="52603-124">Nachfolgend finden Sie die Textparameter, die in der Regel beim Erstellen von Regeln verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="52603-124">The following are body parameters that are typically used when creating rules.</span></span> <span data-ttu-id="52603-125">Sie können bei Bedarf im Anforderungstext beliebige andere schreibbare **messageRule**-Eigenschaften angeben.</span><span class="sxs-lookup"><span data-stu-id="52603-125">You can specify any other writable **messageRule** properties as appropriate in the request body.</span></span>

| <span data-ttu-id="52603-126">Name</span><span class="sxs-lookup"><span data-stu-id="52603-126">Name</span></span>       | <span data-ttu-id="52603-127">Typ</span><span class="sxs-lookup"><span data-stu-id="52603-127">Type</span></span>|<span data-ttu-id="52603-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="52603-128">Description</span></span>|
|:--------|:-------|:----------|
|<span data-ttu-id="52603-129">Aktionen</span><span class="sxs-lookup"><span data-stu-id="52603-129">actions</span></span>|[<span data-ttu-id="52603-130">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="52603-130">messageRuleActions</span></span>](../resources/messageruleactions.md)|<span data-ttu-id="52603-131">Aktionen, die auf eine Nachricht angewendet werden, wenn die entsprechenden Bedingungen (falls vorhanden) erfüllt sind.</span><span class="sxs-lookup"><span data-stu-id="52603-131">Actions to be taken on a message when the corresponding conditions, if any, are fulfilled.</span></span> <span data-ttu-id="52603-132">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="52603-132">Required.</span></span>|
|<span data-ttu-id="52603-133">Bedingungen</span><span class="sxs-lookup"><span data-stu-id="52603-133">conditions</span></span>|[<span data-ttu-id="52603-134">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="52603-134">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)|<span data-ttu-id="52603-135">Bedingungen, die bei Erfüllung die entsprechenden Aktionen für diese Regel auslösen.</span><span class="sxs-lookup"><span data-stu-id="52603-135">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> <span data-ttu-id="52603-136">Optional.</span><span class="sxs-lookup"><span data-stu-id="52603-136">Optional.</span></span>|
|<span data-ttu-id="52603-137">displayName</span><span class="sxs-lookup"><span data-stu-id="52603-137">displayName</span></span>| <span data-ttu-id="52603-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="52603-138">String</span></span>  | <span data-ttu-id="52603-139">Der Anzeigename der Regel.</span><span class="sxs-lookup"><span data-stu-id="52603-139">The display name of the rule.</span></span> <span data-ttu-id="52603-140">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="52603-140">Required.</span></span>|
|<span data-ttu-id="52603-141">Ausnahmen</span><span class="sxs-lookup"><span data-stu-id="52603-141">exceptions</span></span>| [<span data-ttu-id="52603-142">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="52603-142">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)| <span data-ttu-id="52603-143">Ausnahmebedingungen für die Regel.</span><span class="sxs-lookup"><span data-stu-id="52603-143">Represents exception conditions for the rule.</span></span> <span data-ttu-id="52603-144">Optional.</span><span class="sxs-lookup"><span data-stu-id="52603-144">Optional.</span></span> |
|<span data-ttu-id="52603-145">isEnabled</span><span class="sxs-lookup"><span data-stu-id="52603-145">isEnabled</span></span> | <span data-ttu-id="52603-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="52603-146">Boolean</span></span> | <span data-ttu-id="52603-147">Gibt an, ob die Regel auf Nachrichten angewendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="52603-147">Indicates whether the rule is enabled to be applied to messages.</span></span> <span data-ttu-id="52603-148">Optional.</span><span class="sxs-lookup"><span data-stu-id="52603-148">Optional.</span></span> |
|<span data-ttu-id="52603-149">sequence</span><span class="sxs-lookup"><span data-stu-id="52603-149">sequence</span></span>| <span data-ttu-id="52603-150">Int32</span><span class="sxs-lookup"><span data-stu-id="52603-150">Int32</span></span> | <span data-ttu-id="52603-151">Gibt die Reihenfolge an, in der die Regel zusammen mit anderen Regeln ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="52603-151">Indicates the order in which the rule is executed, among other rules.</span></span> <span data-ttu-id="52603-152">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="52603-152">Required.</span></span>|

## <a name="response"></a><span data-ttu-id="52603-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="52603-153">Response</span></span>
<span data-ttu-id="52603-154">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs **messageRule** im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="52603-154">If successful, this method returns `201 Created` response code and a **messageRule** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52603-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="52603-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="52603-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="52603-156">Request</span></span>
<span data-ttu-id="52603-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="52603-157">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox"],
  "name": "create_messagerule_from_mailfolder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules
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
##### <a name="response"></a><span data-ttu-id="52603-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="52603-158">Response</span></span>
<span data-ttu-id="52603-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="52603-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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