---
title: Regel erstellen
description: 'Erstellen Sie ein  messageRule-Objekt, indem Sie eine Gruppe von Bedingungen und Aktionen angeben. '
ms.openlocfilehash: fdea3920e272581c8d08e04c01c385575e6c6df1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017795"
---
# <a name="create-rule"></a><span data-ttu-id="bc8af-103">Regel erstellen</span><span class="sxs-lookup"><span data-stu-id="bc8af-103">Create rule</span></span>


<span data-ttu-id="bc8af-104">Erstellen Sie ein  [messageRule](../resources/messagerule.md)-Objekt, indem Sie eine Gruppe von Bedingungen und Aktionen angeben.</span><span class="sxs-lookup"><span data-stu-id="bc8af-104">Create a [messageRule](../resources/messagerule.md) object by specifying a set of conditions and actions.</span></span> 

<span data-ttu-id="bc8af-105">Outlook führt diese Aktionen aus, wenn eine eingehende Nachricht im Posteingang des Benutzers die angegebenen Bedingungen erfüllt.</span><span class="sxs-lookup"><span data-stu-id="bc8af-105">Outlook carries out those actions if an incoming message in the user's Inbox meets the specified conditions.</span></span>

## <a name="permissions"></a><span data-ttu-id="bc8af-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bc8af-106">Permissions</span></span>
<span data-ttu-id="bc8af-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc8af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc8af-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bc8af-109">Permission type</span></span>      | <span data-ttu-id="bc8af-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bc8af-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc8af-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bc8af-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bc8af-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc8af-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="bc8af-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bc8af-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc8af-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc8af-114">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="bc8af-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bc8af-115">Application</span></span> | <span data-ttu-id="bc8af-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc8af-116">MailboxSettings.ReadWrite</span></span> |


## <a name="http-request"></a><span data-ttu-id="bc8af-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bc8af-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/inbox/messageRules
POST /users/{id | userPrincipalName}/mailFolders/inbox/messageRules
```
## <a name="request-headers"></a><span data-ttu-id="bc8af-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bc8af-118">Request headers</span></span>
| <span data-ttu-id="bc8af-119">Name</span><span class="sxs-lookup"><span data-stu-id="bc8af-119">Name</span></span>       | <span data-ttu-id="bc8af-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bc8af-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bc8af-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc8af-121">Authorization</span></span>  | <span data-ttu-id="bc8af-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bc8af-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="bc8af-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bc8af-124">Request body</span></span>
<span data-ttu-id="bc8af-125">Geben Sie im Anforderungstext die Parameter an, die auf die Regel angewendet werden können.</span><span class="sxs-lookup"><span data-stu-id="bc8af-125">In the request body, supply the parameters that are applicable to your rule.</span></span> <span data-ttu-id="bc8af-126">Nachfolgend finden Sie die Textparameter, die in der Regel beim Erstellen von Regeln verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="bc8af-126">The following are body parameters that are typically used when creating rules.</span></span> <span data-ttu-id="bc8af-127">Sie können bei Bedarf im Anforderungstext beliebige andere schreibbare **messageRule**-Eigenschaften angeben.</span><span class="sxs-lookup"><span data-stu-id="bc8af-127">You can specify any other writable **messageRule** properties as appropriate in the request body.</span></span>

| <span data-ttu-id="bc8af-128">Name</span><span class="sxs-lookup"><span data-stu-id="bc8af-128">Name</span></span>       | <span data-ttu-id="bc8af-129">Typ</span><span class="sxs-lookup"><span data-stu-id="bc8af-129">Type</span></span>|<span data-ttu-id="bc8af-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bc8af-130">Description</span></span>|
|:--------|:-------|:----------|
|<span data-ttu-id="bc8af-131">Aktionen</span><span class="sxs-lookup"><span data-stu-id="bc8af-131">actions</span></span>|[<span data-ttu-id="bc8af-132">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="bc8af-132">messageRuleActions</span></span>](../resources/messageruleactions.md)|<span data-ttu-id="bc8af-133">Aktionen, die auf eine Nachricht angewendet werden, wenn die entsprechenden Bedingungen (falls vorhanden) erfüllt sind.</span><span class="sxs-lookup"><span data-stu-id="bc8af-133">Actions to be taken on a message when the corresponding conditions, if any, are fulfilled.</span></span> <span data-ttu-id="bc8af-134">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="bc8af-134">Required.</span></span>|
|<span data-ttu-id="bc8af-135">Bedingungen</span><span class="sxs-lookup"><span data-stu-id="bc8af-135">conditions</span></span>|[<span data-ttu-id="bc8af-136">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="bc8af-136">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)|<span data-ttu-id="bc8af-137">Bedingungen, die bei Erfüllung die entsprechenden Aktionen für diese Regel auslösen.</span><span class="sxs-lookup"><span data-stu-id="bc8af-137">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> <span data-ttu-id="bc8af-138">Optional.</span><span class="sxs-lookup"><span data-stu-id="bc8af-138">Optional.</span></span>|
|<span data-ttu-id="bc8af-139">displayName</span><span class="sxs-lookup"><span data-stu-id="bc8af-139">displayName</span></span>| <span data-ttu-id="bc8af-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bc8af-140">String</span></span>  | <span data-ttu-id="bc8af-141">Der Anzeigename der Regel.</span><span class="sxs-lookup"><span data-stu-id="bc8af-141">The display name of the rule.</span></span> <span data-ttu-id="bc8af-142">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="bc8af-142">Required.</span></span>|
|<span data-ttu-id="bc8af-143">Ausnahmen</span><span class="sxs-lookup"><span data-stu-id="bc8af-143">exceptions</span></span>| [<span data-ttu-id="bc8af-144">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="bc8af-144">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)| <span data-ttu-id="bc8af-145">Ausnahmebedingungen für die Regel.</span><span class="sxs-lookup"><span data-stu-id="bc8af-145">Represents exception conditions for the rule.</span></span> <span data-ttu-id="bc8af-146">Optional.</span><span class="sxs-lookup"><span data-stu-id="bc8af-146">Optional.</span></span> |
|<span data-ttu-id="bc8af-147">isEnabled</span><span class="sxs-lookup"><span data-stu-id="bc8af-147">isEnabled</span></span> | <span data-ttu-id="bc8af-148">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="bc8af-148">Boolean</span></span> | <span data-ttu-id="bc8af-149">Gibt an, ob die Regel auf Nachrichten angewendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="bc8af-149">Indicates whether the rule is enabled to be applied to messages.</span></span> <span data-ttu-id="bc8af-150">Optional.</span><span class="sxs-lookup"><span data-stu-id="bc8af-150">Optional.</span></span> |
|<span data-ttu-id="bc8af-151">sequence</span><span class="sxs-lookup"><span data-stu-id="bc8af-151">sequence</span></span>| <span data-ttu-id="bc8af-152">Int32</span><span class="sxs-lookup"><span data-stu-id="bc8af-152">Int32</span></span> | <span data-ttu-id="bc8af-153">Gibt die Reihenfolge an, in der die Regel zusammen mit anderen Regeln ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="bc8af-153">Indicates the order in which the rule is executed, among other rules.</span></span> <span data-ttu-id="bc8af-154">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="bc8af-154">Required.</span></span>|

## <a name="response"></a><span data-ttu-id="bc8af-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="bc8af-155">Response</span></span>
<span data-ttu-id="bc8af-156">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs **messageRule** im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="bc8af-156">If successful, this method returns `201 Created` response code and a **messageRule** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc8af-157">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bc8af-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bc8af-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bc8af-158">Request</span></span>
<span data-ttu-id="bc8af-159">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bc8af-159">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="bc8af-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="bc8af-160">Response</span></span>
<span data-ttu-id="bc8af-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bc8af-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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