---
title: Regel erstellen
description: 'Erstellen Sie ein  messageRule-Objekt, indem Sie eine Gruppe von Bedingungen und Aktionen angeben. '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: f2c06fce207728af6d89b5284eda2458d9b65438
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528158"
---
# <a name="create-rule"></a><span data-ttu-id="e4fc4-103">Regel erstellen</span><span class="sxs-lookup"><span data-stu-id="e4fc4-103">Create rule</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4fc4-104">Erstellen Sie ein  [messageRule](../resources/messagerule.md)-Objekt, indem Sie eine Gruppe von Bedingungen und Aktionen angeben.</span><span class="sxs-lookup"><span data-stu-id="e4fc4-104">Create a [messageRule](../resources/messagerule.md) object by specifying a set of conditions and actions.</span></span> 

<span data-ttu-id="e4fc4-105">Outlook führt diese Aktionen aus, wenn eine eingehende Nachricht im Posteingang des Benutzers die angegebenen Bedingungen erfüllt.</span><span class="sxs-lookup"><span data-stu-id="e4fc4-105">Outlook carries out those actions if an incoming message in the user's Inbox meets the specified conditions.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4fc4-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e4fc4-106">Permissions</span></span>
<span data-ttu-id="e4fc4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4fc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4fc4-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e4fc4-109">Permission type</span></span>      | <span data-ttu-id="e4fc4-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e4fc4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4fc4-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e4fc4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e4fc4-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e4fc4-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="e4fc4-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e4fc4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4fc4-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e4fc4-114">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="e4fc4-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e4fc4-115">Application</span></span> | <span data-ttu-id="e4fc4-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e4fc4-116">MailboxSettings.ReadWrite</span></span> |


## <a name="http-request"></a><span data-ttu-id="e4fc4-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e4fc4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/inbox/messagerules
POST /users/{id | userPrincipalName}/mailFolders/inbox/messagerules
```
## <a name="request-headers"></a><span data-ttu-id="e4fc4-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e4fc4-118">Request headers</span></span>
| <span data-ttu-id="e4fc4-119">Name</span><span class="sxs-lookup"><span data-stu-id="e4fc4-119">Name</span></span>       | <span data-ttu-id="e4fc4-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e4fc4-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e4fc4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4fc4-121">Authorization</span></span>  | <span data-ttu-id="e4fc4-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e4fc4-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="e4fc4-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e4fc4-124">Request body</span></span>
<span data-ttu-id="e4fc4-125">Geben Sie im Anforderungstext die Parameter an, die auf die Regel angewendet werden können.</span><span class="sxs-lookup"><span data-stu-id="e4fc4-125">In the request body, supply the parameters that are applicable to your rule.</span></span> <span data-ttu-id="e4fc4-126">Nachfolgend finden Sie die Textparameter, die in der Regel beim Erstellen von Regeln verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="e4fc4-126">The following are body parameters that are typically used when creating rules.</span></span> <span data-ttu-id="e4fc4-127">Sie können bei Bedarf im Anforderungstext beliebige andere schreibbare **messageRule**-Eigenschaften angeben.</span><span class="sxs-lookup"><span data-stu-id="e4fc4-127">You can specify any other writable **messageRule** properties as appropriate in the request body.</span></span>

| <span data-ttu-id="e4fc4-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="e4fc4-128">Parameter</span></span>       | <span data-ttu-id="e4fc4-129">Typ</span><span class="sxs-lookup"><span data-stu-id="e4fc4-129">Type</span></span>|<span data-ttu-id="e4fc4-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e4fc4-130">Description</span></span>|
|:--------|:-------|:----------|
|<span data-ttu-id="e4fc4-131">Aktionen</span><span class="sxs-lookup"><span data-stu-id="e4fc4-131">actions</span></span>|[<span data-ttu-id="e4fc4-132">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="e4fc4-132">messageRuleActions</span></span>](../resources/messageruleactions.md)|<span data-ttu-id="e4fc4-133">Aktionen, die auf eine Nachricht angewendet werden, wenn die entsprechenden Bedingungen (falls vorhanden) erfüllt sind.</span><span class="sxs-lookup"><span data-stu-id="e4fc4-133">Actions to be taken on a message when the corresponding conditions, if any, are fulfilled.</span></span> <span data-ttu-id="e4fc4-134">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e4fc4-134">Required.</span></span>|
|<span data-ttu-id="e4fc4-135">Bedingungen</span><span class="sxs-lookup"><span data-stu-id="e4fc4-135">conditions</span></span>|[<span data-ttu-id="e4fc4-136">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="e4fc4-136">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)|<span data-ttu-id="e4fc4-137">Bedingungen, die bei Erfüllung die entsprechenden Aktionen für diese Regel auslösen.</span><span class="sxs-lookup"><span data-stu-id="e4fc4-137">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> <span data-ttu-id="e4fc4-138">Optional.</span><span class="sxs-lookup"><span data-stu-id="e4fc4-138">Optional.</span></span>|
|<span data-ttu-id="e4fc4-139">displayName</span><span class="sxs-lookup"><span data-stu-id="e4fc4-139">displayName</span></span>| <span data-ttu-id="e4fc4-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e4fc4-140">String</span></span>  | <span data-ttu-id="e4fc4-141">Der Anzeigename der Regel.</span><span class="sxs-lookup"><span data-stu-id="e4fc4-141">The display name of the rule.</span></span> <span data-ttu-id="e4fc4-142">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e4fc4-142">Required.</span></span>|
|<span data-ttu-id="e4fc4-143">Ausnahmen</span><span class="sxs-lookup"><span data-stu-id="e4fc4-143">exceptions</span></span>| [<span data-ttu-id="e4fc4-144">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="e4fc4-144">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)| <span data-ttu-id="e4fc4-145">Ausnahmebedingungen für die Regel.</span><span class="sxs-lookup"><span data-stu-id="e4fc4-145">Represents exception conditions for the rule.</span></span> <span data-ttu-id="e4fc4-146">Optional.</span><span class="sxs-lookup"><span data-stu-id="e4fc4-146">Optional.</span></span> |
|<span data-ttu-id="e4fc4-147">isEnabled</span><span class="sxs-lookup"><span data-stu-id="e4fc4-147">isEnabled</span></span> | <span data-ttu-id="e4fc4-148">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e4fc4-148">Boolean</span></span> | <span data-ttu-id="e4fc4-149">Gibt an, ob die Regel auf Nachrichten angewendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="e4fc4-149">Indicates whether the rule is enabled to be applied to messages.</span></span> <span data-ttu-id="e4fc4-150">Optional.</span><span class="sxs-lookup"><span data-stu-id="e4fc4-150">Optional.</span></span> |
|<span data-ttu-id="e4fc4-151">sequence</span><span class="sxs-lookup"><span data-stu-id="e4fc4-151">sequence</span></span>| <span data-ttu-id="e4fc4-152">Int32</span><span class="sxs-lookup"><span data-stu-id="e4fc4-152">Int32</span></span> | <span data-ttu-id="e4fc4-153">Gibt die Reihenfolge an, in der die Regel zusammen mit anderen Regeln ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="e4fc4-153">Indicates the order in which the rule is executed, among other rules.</span></span> <span data-ttu-id="e4fc4-154">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="e4fc4-154">Required.</span></span>|

## <a name="response"></a><span data-ttu-id="e4fc4-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="e4fc4-155">Response</span></span>
<span data-ttu-id="e4fc4-156">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs **messageRule** im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e4fc4-156">If successful, this method returns `201 Created` response code and a **messageRule** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4fc4-157">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e4fc4-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e4fc4-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e4fc4-158">Request</span></span>
<span data-ttu-id="e4fc4-159">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e4fc4-159">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="e4fc4-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="e4fc4-160">Response</span></span>
<span data-ttu-id="e4fc4-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e4fc4-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/mailfolder-post-messagerules.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
