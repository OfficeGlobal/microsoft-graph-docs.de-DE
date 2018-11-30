---
title: Regel aktualisieren
description: Ändern Sie die schreibbaren Eigenschaften in einem messageRule-Objekt, und speichern Sie die Änderungen.
ms.openlocfilehash: 1096006176b455052556de5f1afc1d882db8d8e1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019288"
---
# <a name="update-rule"></a><span data-ttu-id="cf605-103">Regel aktualisieren</span><span class="sxs-lookup"><span data-stu-id="cf605-103">Update rule</span></span>


<span data-ttu-id="cf605-104">Ändern Sie die schreibbaren Eigenschaften in einem [messageRule](../resources/messagerule.md)-Objekt, und speichern Sie die Änderungen.</span><span class="sxs-lookup"><span data-stu-id="cf605-104">Change writable properties on a [messageRule](../resources/messagerule.md) object and save the changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="cf605-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cf605-105">Permissions</span></span>
<span data-ttu-id="cf605-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf605-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf605-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cf605-108">Permission type</span></span>      | <span data-ttu-id="cf605-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cf605-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf605-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cf605-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cf605-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cf605-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="cf605-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cf605-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf605-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cf605-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="cf605-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cf605-114">Application</span></span> | <span data-ttu-id="cf605-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cf605-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf605-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cf605-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/inbox/messageRules/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/inbox/messageRules/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="cf605-117">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cf605-117">Optional request headers</span></span>
| <span data-ttu-id="cf605-118">Name</span><span class="sxs-lookup"><span data-stu-id="cf605-118">Name</span></span>       | <span data-ttu-id="cf605-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cf605-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="cf605-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf605-120">Authorization</span></span>  | <span data-ttu-id="cf605-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cf605-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="cf605-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cf605-123">Request body</span></span>
<span data-ttu-id="cf605-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="cf605-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="cf605-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cf605-127">Property</span></span>     | <span data-ttu-id="cf605-128">Typ</span><span class="sxs-lookup"><span data-stu-id="cf605-128">Type</span></span>   |<span data-ttu-id="cf605-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cf605-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cf605-130">Aktionen</span><span class="sxs-lookup"><span data-stu-id="cf605-130">actions</span></span> | [<span data-ttu-id="cf605-131">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="cf605-131">messageRuleActions</span></span>](../resources/messageruleactions.md) | <span data-ttu-id="cf605-132">Aktionen, die auf eine Nachricht angewendet werden, wenn die entsprechenden Bedingungen erfüllt sind.</span><span class="sxs-lookup"><span data-stu-id="cf605-132">Actions to be taken on a message when the corresponding conditions are fulfilled.</span></span> |
| <span data-ttu-id="cf605-133">Bedingungen</span><span class="sxs-lookup"><span data-stu-id="cf605-133">conditions</span></span> | [<span data-ttu-id="cf605-134">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="cf605-134">messageRulePredicates</span></span>](../resources/messagerulepredicates.md) | <span data-ttu-id="cf605-135">Bedingungen, die bei Erfüllung die entsprechenden Aktionen für diese Regel auslösen.</span><span class="sxs-lookup"><span data-stu-id="cf605-135">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> |
| <span data-ttu-id="cf605-136">displayName</span><span class="sxs-lookup"><span data-stu-id="cf605-136">displayName</span></span> | <span data-ttu-id="cf605-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cf605-137">String</span></span> | <span data-ttu-id="cf605-138">Der Anzeigename der Regel.</span><span class="sxs-lookup"><span data-stu-id="cf605-138">The display name of the rule.</span></span> |
| <span data-ttu-id="cf605-139">Ausnahmen</span><span class="sxs-lookup"><span data-stu-id="cf605-139">exceptions</span></span> | [<span data-ttu-id="cf605-140">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="cf605-140">messageRulePredicates</span></span>](../resources/messagerulepredicates.md) | <span data-ttu-id="cf605-141">Ausnahmebedingungen für die Regel.</span><span class="sxs-lookup"><span data-stu-id="cf605-141">Exception conditions for the rule.</span></span> |
| <span data-ttu-id="cf605-142">isEnabled</span><span class="sxs-lookup"><span data-stu-id="cf605-142">isEnabled</span></span> | <span data-ttu-id="cf605-143">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="cf605-143">Boolean</span></span> | <span data-ttu-id="cf605-144">Gibt an, ob die Regel auf Nachrichten angewendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="cf605-144">Indicates whether the rule is enabled to be applied to messages.</span></span> |
| <span data-ttu-id="cf605-145">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="cf605-145">isReadOnly</span></span> | <span data-ttu-id="cf605-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="cf605-146">Boolean</span></span> | <span data-ttu-id="cf605-147">Gibt an, ob die Regel schreibgeschützt ist und von der Regel-REST-API nicht geändert oder gelöscht werden kann.</span><span class="sxs-lookup"><span data-stu-id="cf605-147">Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.</span></span> |
| <span data-ttu-id="cf605-148">sequence</span><span class="sxs-lookup"><span data-stu-id="cf605-148">sequence</span></span> | <span data-ttu-id="cf605-149">Int32</span><span class="sxs-lookup"><span data-stu-id="cf605-149">Int32</span></span> | <span data-ttu-id="cf605-150">Gibt die Reihenfolge an, in der die Regel zusammen mit anderen Regeln ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="cf605-150">Indicates the order in which the rule is executed, among other rules.</span></span> |


## <a name="response"></a><span data-ttu-id="cf605-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="cf605-151">Response</span></span>
<span data-ttu-id="cf605-152">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [messageRule](../resources/messagerule.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cf605-152">If successful, this method returns a `200 OK` response code and updated [messageRule](../resources/messagerule.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cf605-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cf605-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cf605-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cf605-154">Request</span></span>
<span data-ttu-id="cf605-155">Im folgenden Beispiel werden der Name der Regel sowie die Aktionen, die für diese Regel ausgeführt werden sollen, im [Beispiel](messagerule-get.md#example) in [Regel abrufen](messagerule-get.md) von der Weiterleitung an eine Adresse zur Markierung ihrer Wichtigkeit in „Hoch“ geändert.</span><span class="sxs-lookup"><span data-stu-id="cf605-155">The following example changes the name of the rule, and the actions to be taken for that rule in the [example](messagerule-get.md#example) in [Get rule](messagerule-get.md), from forwarding to an address to marking its importance as high.</span></span> 
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
##### <a name="response"></a><span data-ttu-id="cf605-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="cf605-156">Response</span></span>
<span data-ttu-id="cf605-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cf605-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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