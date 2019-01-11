---
title: Regel aktualisieren
description: Ändern Sie die schreibbaren Eigenschaften in einem messageRule-Objekt, und speichern Sie die Änderungen.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 3b034c7c428821c23b92d78644b43de9d7a2946d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886359"
---
# <a name="update-rule"></a><span data-ttu-id="7865a-103">Regel aktualisieren</span><span class="sxs-lookup"><span data-stu-id="7865a-103">Update rule</span></span>

> <span data-ttu-id="7865a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7865a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7865a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7865a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7865a-106">Ändern Sie die schreibbaren Eigenschaften in einem [messageRule](../resources/messagerule.md)-Objekt, und speichern Sie die Änderungen.</span><span class="sxs-lookup"><span data-stu-id="7865a-106">Change writable properties on a [messageRule](../resources/messagerule.md) object and save the changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="7865a-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7865a-107">Permissions</span></span>
<span data-ttu-id="7865a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7865a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7865a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7865a-110">Permission type</span></span>      | <span data-ttu-id="7865a-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7865a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7865a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7865a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7865a-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7865a-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="7865a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7865a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7865a-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7865a-115">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="7865a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7865a-116">Application</span></span> | <span data-ttu-id="7865a-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7865a-117">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7865a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7865a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/inbox/messagerules/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/inbox/messagerules/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="7865a-119">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7865a-119">Optional request headers</span></span>
| <span data-ttu-id="7865a-120">Name</span><span class="sxs-lookup"><span data-stu-id="7865a-120">Name</span></span>       | <span data-ttu-id="7865a-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7865a-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="7865a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7865a-122">Authorization</span></span>  | <span data-ttu-id="7865a-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7865a-p103">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="7865a-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7865a-125">Request body</span></span>
<span data-ttu-id="7865a-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="7865a-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7865a-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7865a-129">Property</span></span>     | <span data-ttu-id="7865a-130">Typ</span><span class="sxs-lookup"><span data-stu-id="7865a-130">Type</span></span>   |<span data-ttu-id="7865a-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7865a-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7865a-132">Aktionen</span><span class="sxs-lookup"><span data-stu-id="7865a-132">actions</span></span> | [<span data-ttu-id="7865a-133">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="7865a-133">messageRuleActions</span></span>](../resources/messageruleactions.md) | <span data-ttu-id="7865a-134">Aktionen, die auf eine Nachricht angewendet werden, wenn die entsprechenden Bedingungen erfüllt sind.</span><span class="sxs-lookup"><span data-stu-id="7865a-134">Actions to be taken on a message when the corresponding conditions are fulfilled.</span></span> |
| <span data-ttu-id="7865a-135">Bedingungen</span><span class="sxs-lookup"><span data-stu-id="7865a-135">conditions</span></span> | [<span data-ttu-id="7865a-136">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="7865a-136">messageRulePredicates</span></span>](../resources/messagerulepredicates.md) | <span data-ttu-id="7865a-137">Bedingungen, die bei Erfüllung die entsprechenden Aktionen für diese Regel auslösen.</span><span class="sxs-lookup"><span data-stu-id="7865a-137">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> |
| <span data-ttu-id="7865a-138">displayName</span><span class="sxs-lookup"><span data-stu-id="7865a-138">displayName</span></span> | <span data-ttu-id="7865a-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7865a-139">String</span></span> | <span data-ttu-id="7865a-140">Der Anzeigename der Regel.</span><span class="sxs-lookup"><span data-stu-id="7865a-140">The display name of the rule.</span></span> |
| <span data-ttu-id="7865a-141">Ausnahmen</span><span class="sxs-lookup"><span data-stu-id="7865a-141">exceptions</span></span> | [<span data-ttu-id="7865a-142">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="7865a-142">messageRulePredicates</span></span>](../resources/messagerulepredicates.md) | <span data-ttu-id="7865a-143">Ausnahmebedingungen für die Regel.</span><span class="sxs-lookup"><span data-stu-id="7865a-143">Exception conditions for the rule.</span></span> |
| <span data-ttu-id="7865a-144">isEnabled</span><span class="sxs-lookup"><span data-stu-id="7865a-144">isEnabled</span></span> | <span data-ttu-id="7865a-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7865a-145">Boolean</span></span> | <span data-ttu-id="7865a-146">Gibt an, ob die Regel auf Nachrichten angewendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="7865a-146">Indicates whether the rule is enabled to be applied to messages.</span></span> |
| <span data-ttu-id="7865a-147">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="7865a-147">isReadOnly</span></span> | <span data-ttu-id="7865a-148">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7865a-148">Boolean</span></span> | <span data-ttu-id="7865a-149">Gibt an, ob die Regel schreibgeschützt ist und von der Regel-REST-API nicht geändert oder gelöscht werden kann.</span><span class="sxs-lookup"><span data-stu-id="7865a-149">Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.</span></span> |
| <span data-ttu-id="7865a-150">sequence</span><span class="sxs-lookup"><span data-stu-id="7865a-150">sequence</span></span> | <span data-ttu-id="7865a-151">Int32</span><span class="sxs-lookup"><span data-stu-id="7865a-151">Int32</span></span> | <span data-ttu-id="7865a-152">Gibt die Reihenfolge an, in der die Regel zusammen mit anderen Regeln ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="7865a-152">Indicates the order in which the rule is executed, among other rules.</span></span> |


## <a name="response"></a><span data-ttu-id="7865a-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="7865a-153">Response</span></span>
<span data-ttu-id="7865a-154">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [messageRule](../resources/messagerule.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7865a-154">If successful, this method returns a `200 OK` response code and updated [messageRule](../resources/messagerule.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7865a-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7865a-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7865a-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7865a-156">Request</span></span>
<span data-ttu-id="7865a-157">Im folgenden Beispiel werden der Name der Regel sowie die Aktionen, die für diese Regel ausgeführt werden sollen, im [Beispiel](messagerule-get.md#example) in [Regel abrufen](messagerule-get.md) von der Weiterleitung an eine Adresse zur Markierung ihrer Wichtigkeit in „Hoch“ geändert.</span><span class="sxs-lookup"><span data-stu-id="7865a-157">The following example changes the name of the rule, and the actions to be taken for that rule in the [example](messagerule-get.md#example) in [Get rule](messagerule-get.md), from forwarding to an address to marking its importance as high.</span></span> 
<!-- {
  "blockType": "request",
  "name": "update_messagerule"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/mailfolders/inbox/messagerules('AQAAAJ5dZqA=')

Content-type: application/json

{
    "displayName": "Important from partner",
    "actions": {
        "markImportance": "high"
     }
} 
```
##### <a name="response"></a><span data-ttu-id="7865a-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="7865a-158">Response</span></span>
<span data-ttu-id="7865a-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7865a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.messageRule"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#Me/mailFolders('inbox')/messageRules/$entity",
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
