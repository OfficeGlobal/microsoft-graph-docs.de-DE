---
title: Regel erstellen
description: 'Erstellen Sie ein  messageRule-Objekt, indem Sie eine Gruppe von Bedingungen und Aktionen angeben. '
ms.openlocfilehash: f725aa0a078938cf111782aedf1feb041a5a0e19
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065899"
---
# <a name="create-rule"></a><span data-ttu-id="613b6-103">Regel erstellen</span><span class="sxs-lookup"><span data-stu-id="613b6-103">Create rule</span></span>

> <span data-ttu-id="613b6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="613b6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="613b6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="613b6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="613b6-106">Erstellen Sie ein  [messageRule](../resources/messagerule.md)-Objekt, indem Sie eine Gruppe von Bedingungen und Aktionen angeben.</span><span class="sxs-lookup"><span data-stu-id="613b6-106">Create a [messageRule](../resources/messagerule.md) object by specifying a set of conditions and actions.</span></span> 

<span data-ttu-id="613b6-107">Outlook führt diese Aktionen aus, wenn eine eingehende Nachricht im Posteingang des Benutzers die angegebenen Bedingungen erfüllt.</span><span class="sxs-lookup"><span data-stu-id="613b6-107">Outlook carries out those actions if an incoming message in the user's Inbox meets the specified conditions.</span></span>

## <a name="permissions"></a><span data-ttu-id="613b6-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="613b6-108">Permissions</span></span>
<span data-ttu-id="613b6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="613b6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="613b6-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="613b6-111">Permission type</span></span>      | <span data-ttu-id="613b6-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="613b6-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="613b6-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="613b6-113">Delegated (work or school account)</span></span> | <span data-ttu-id="613b6-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="613b6-114">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="613b6-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="613b6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="613b6-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="613b6-116">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="613b6-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="613b6-117">Application</span></span> | <span data-ttu-id="613b6-118">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="613b6-118">MailboxSettings.ReadWrite</span></span> |


## <a name="http-request"></a><span data-ttu-id="613b6-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="613b6-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/inbox/messagerules
POST /users/{id | userPrincipalName}/mailFolders/inbox/messagerules
```
## <a name="request-headers"></a><span data-ttu-id="613b6-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="613b6-120">Request headers</span></span>
| <span data-ttu-id="613b6-121">Name</span><span class="sxs-lookup"><span data-stu-id="613b6-121">Name</span></span>       | <span data-ttu-id="613b6-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="613b6-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="613b6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="613b6-123">Authorization</span></span>  | <span data-ttu-id="613b6-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="613b6-p103">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="613b6-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="613b6-126">Request body</span></span>
<span data-ttu-id="613b6-127">Geben Sie im Anforderungstext die Parameter an, die auf die Regel angewendet werden können.</span><span class="sxs-lookup"><span data-stu-id="613b6-127">In the request body, supply the parameters that are applicable to your rule.</span></span> <span data-ttu-id="613b6-128">Nachfolgend finden Sie die Textparameter, die in der Regel beim Erstellen von Regeln verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="613b6-128">The following are body parameters that are typically used when creating rules.</span></span> <span data-ttu-id="613b6-129">Sie können bei Bedarf im Anforderungstext beliebige andere schreibbare **messageRule**-Eigenschaften angeben.</span><span class="sxs-lookup"><span data-stu-id="613b6-129">You can specify any other writable **messageRule** properties as appropriate in the request body.</span></span>

| <span data-ttu-id="613b6-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="613b6-130">Parameter</span></span>       | <span data-ttu-id="613b6-131">Typ</span><span class="sxs-lookup"><span data-stu-id="613b6-131">Type</span></span>|<span data-ttu-id="613b6-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="613b6-132">Description</span></span>|
|:--------|:-------|:----------|
|<span data-ttu-id="613b6-133">Aktionen</span><span class="sxs-lookup"><span data-stu-id="613b6-133">actions</span></span>|[<span data-ttu-id="613b6-134">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="613b6-134">messageRuleActions</span></span>](../resources/messageruleactions.md)|<span data-ttu-id="613b6-135">Aktionen, die auf eine Nachricht angewendet werden, wenn die entsprechenden Bedingungen (falls vorhanden) erfüllt sind.</span><span class="sxs-lookup"><span data-stu-id="613b6-135">Actions to be taken on a message when the corresponding conditions, if any, are fulfilled.</span></span> <span data-ttu-id="613b6-136">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="613b6-136">Required.</span></span>|
|<span data-ttu-id="613b6-137">Bedingungen</span><span class="sxs-lookup"><span data-stu-id="613b6-137">conditions</span></span>|[<span data-ttu-id="613b6-138">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="613b6-138">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)|<span data-ttu-id="613b6-139">Bedingungen, die bei Erfüllung die entsprechenden Aktionen für diese Regel auslösen.</span><span class="sxs-lookup"><span data-stu-id="613b6-139">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> <span data-ttu-id="613b6-140">Optional.</span><span class="sxs-lookup"><span data-stu-id="613b6-140">Optional.</span></span>|
|<span data-ttu-id="613b6-141">displayName</span><span class="sxs-lookup"><span data-stu-id="613b6-141">displayName</span></span>| <span data-ttu-id="613b6-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="613b6-142">String</span></span>  | <span data-ttu-id="613b6-143">Der Anzeigename der Regel.</span><span class="sxs-lookup"><span data-stu-id="613b6-143">The display name of the rule.</span></span> <span data-ttu-id="613b6-144">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="613b6-144">Required.</span></span>|
|<span data-ttu-id="613b6-145">Ausnahmen</span><span class="sxs-lookup"><span data-stu-id="613b6-145">exceptions</span></span>| [<span data-ttu-id="613b6-146">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="613b6-146">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)| <span data-ttu-id="613b6-147">Ausnahmebedingungen für die Regel.</span><span class="sxs-lookup"><span data-stu-id="613b6-147">Represents exception conditions for the rule.</span></span> <span data-ttu-id="613b6-148">Optional.</span><span class="sxs-lookup"><span data-stu-id="613b6-148">Optional.</span></span> |
|<span data-ttu-id="613b6-149">isEnabled</span><span class="sxs-lookup"><span data-stu-id="613b6-149">isEnabled</span></span> | <span data-ttu-id="613b6-150">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="613b6-150">Boolean</span></span> | <span data-ttu-id="613b6-151">Gibt an, ob die Regel auf Nachrichten angewendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="613b6-151">Indicates whether the rule is enabled to be applied to messages.</span></span> <span data-ttu-id="613b6-152">Optional.</span><span class="sxs-lookup"><span data-stu-id="613b6-152">Optional.</span></span> |
|<span data-ttu-id="613b6-153">sequence</span><span class="sxs-lookup"><span data-stu-id="613b6-153">sequence</span></span>| <span data-ttu-id="613b6-154">Int32</span><span class="sxs-lookup"><span data-stu-id="613b6-154">Int32</span></span> | <span data-ttu-id="613b6-155">Gibt die Reihenfolge an, in der die Regel zusammen mit anderen Regeln ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="613b6-155">Indicates the order in which the rule is executed, among other rules.</span></span> <span data-ttu-id="613b6-156">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="613b6-156">Required.</span></span>|

## <a name="response"></a><span data-ttu-id="613b6-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="613b6-157">Response</span></span>
<span data-ttu-id="613b6-158">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs **messageRule** im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="613b6-158">If successful, this method returns `201 Created` response code and a **messageRule** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="613b6-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="613b6-159">Example</span></span>
##### <a name="request"></a><span data-ttu-id="613b6-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="613b6-160">Request</span></span>
<span data-ttu-id="613b6-161">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="613b6-161">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_messagerule_from_mailfolder"
}-->
```http
POST https://graph.microsoft.com/beta/me/mailFolders/inbox/messagerules
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
##### <a name="response"></a><span data-ttu-id="613b6-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="613b6-162">Response</span></span>
<span data-ttu-id="613b6-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="613b6-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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