---
title: 'Gruppe: ValidateProperties'
description: Überprüfen Sie, ob eine Office 365-Gruppe Display Name oder die e-Mail-Spitzname naming Richtlinien entspricht. Clients können mithilfe der API bestimmen, ob ein Anzeigename oder e-Mail-Spitzname ist gültig, bevor Sie versuchen, eine Office 365-Gruppe zu **Aktualisieren** . Verwenden Sie zum Überprüfen von Eigenschaften vor dem Erstellen einer Gruppe, die ValidateProperties-Funktion für Directory-Objekte.
ms.openlocfilehash: d7f2767908e6cbf9116bec769a1abc32731e4758
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058945"
---
# <a name="group-validateproperties"></a><span data-ttu-id="6f351-105">Gruppe: ValidateProperties</span><span class="sxs-lookup"><span data-stu-id="6f351-105">group: validateProperties</span></span>

<span data-ttu-id="6f351-106">Überprüfen Sie, ob eine Office 365-Gruppe Display Name oder die e-Mail-Spitzname naming Richtlinien entspricht.</span><span class="sxs-lookup"><span data-stu-id="6f351-106">Validate if an Office 365 group's display name or mail nickname complies with naming policies.</span></span> <span data-ttu-id="6f351-107">Clients können mithilfe der API bestimmen, ob ein Anzeigename oder e-Mail-Spitzname ist gültig, bevor Sie versuchen, eine Office 365-Gruppe zu **Aktualisieren** .</span><span class="sxs-lookup"><span data-stu-id="6f351-107">Clients can use the API to determine if a display name or mail nickname is valid before trying to **update** an Office 365 group.</span></span> <span data-ttu-id="6f351-108">Überprüfen vor dem Erstellen einer Gruppe von Eigenschaften, verwenden Sie die [ValidateProperties-Funktion](directoryobject-validateproperties.md) für Directory-Objekte.</span><span class="sxs-lookup"><span data-stu-id="6f351-108">For validating properties before creating a group, use the [validateProperties function](directoryobject-validateproperties.md) for directory objects.</span></span>

<span data-ttu-id="6f351-109">Für die Namen und e-Mail-Spitzname Anzeigeeigenschaften werden die folgenden Überprüfungen ausgeführt:</span><span class="sxs-lookup"><span data-stu-id="6f351-109">The following validations are performed for the display name and mail nickname properties:</span></span> 
1. <span data-ttu-id="6f351-110">Überprüfen Sie das Präfix und Suffix Richtlinie zum Benennen</span><span class="sxs-lookup"><span data-stu-id="6f351-110">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="6f351-111">Überprüfen Sie die benutzerdefinierten gesperrten Wörter-Richtlinie</span><span class="sxs-lookup"><span data-stu-id="6f351-111">Validate the custom banned words policy</span></span>

<span data-ttu-id="6f351-112">Diese API zurückgegeben mit ersten Fehler.</span><span class="sxs-lookup"><span data-stu-id="6f351-112">This API returns with the first failure encountered.</span></span> <span data-ttu-id="6f351-113">Wenn mehrere Überprüfungen eine oder mehrere Eigenschaften ein Fehler auftritt, wird nur die-Eigenschaft mit den ersten Validierungsfehler zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6f351-113">If one or more properties fail multiple validations, only the property with the first validation failure is returned.</span></span> <span data-ttu-id="6f351-114">Sie können jedoch überprüft e-Mail-Spitznamen und den Anzeigenamen und eine Auflistung von Validierungsfehlern empfangen, wenn Sie nur das Präfix und Suffix Richtlinie zum Benennen überprüfen.</span><span class="sxs-lookup"><span data-stu-id="6f351-114">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f351-115">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6f351-115">Permissions</span></span>

<span data-ttu-id="6f351-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f351-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f351-118">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6f351-118">Permission type</span></span>      | <span data-ttu-id="6f351-119">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6f351-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f351-120">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6f351-120">Delegated (work or school account)</span></span> | <span data-ttu-id="6f351-121">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f351-121">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6f351-122">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6f351-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f351-123">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6f351-123">Not supported.</span></span>    |
|<span data-ttu-id="6f351-124">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6f351-124">Application</span></span> | <span data-ttu-id="6f351-125">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f351-125">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f351-126">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6f351-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /groups/<id>/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="6f351-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6f351-127">Request headers</span></span>

| <span data-ttu-id="6f351-128">Name</span><span class="sxs-lookup"><span data-stu-id="6f351-128">Name</span></span>           | <span data-ttu-id="6f351-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6f351-129">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="6f351-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f351-130">Authorization</span></span>  | <span data-ttu-id="6f351-131">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="6f351-131">Bearer {code}</span></span>    |
| <span data-ttu-id="6f351-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6f351-132">Content-Type</span></span>   | <span data-ttu-id="6f351-133">application/json</span><span class="sxs-lookup"><span data-stu-id="6f351-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="6f351-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6f351-134">Request body</span></span>

<span data-ttu-id="6f351-135">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="6f351-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6f351-136">Parameter</span><span class="sxs-lookup"><span data-stu-id="6f351-136">Parameter</span></span>    | <span data-ttu-id="6f351-137">Typ</span><span class="sxs-lookup"><span data-stu-id="6f351-137">Type</span></span>   |<span data-ttu-id="6f351-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6f351-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6f351-139">displayName</span><span class="sxs-lookup"><span data-stu-id="6f351-139">displayName</span></span>|<span data-ttu-id="6f351-140">String</span><span class="sxs-lookup"><span data-stu-id="6f351-140">String</span></span>| <span data-ttu-id="6f351-141">Der Anzeigename der Gruppe zu überprüfen.</span><span class="sxs-lookup"><span data-stu-id="6f351-141">The display name of the group to validate.</span></span> <span data-ttu-id="6f351-142">Die Eigenschaft ist nicht einzeln erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6f351-142">The property is not individually required.</span></span> <span data-ttu-id="6f351-143">Mindestens eine Eigenschaft (DisplayName oder MailNickname) ist jedoch erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6f351-143">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="6f351-144">mailNickname</span><span class="sxs-lookup"><span data-stu-id="6f351-144">mailNickname</span></span>|<span data-ttu-id="6f351-145">String</span><span class="sxs-lookup"><span data-stu-id="6f351-145">String</span></span>| <span data-ttu-id="6f351-146">Die e-Mail-Spitzname der Gruppe zu überprüfen.</span><span class="sxs-lookup"><span data-stu-id="6f351-146">The mail nickname of the group to validate.</span></span> <span data-ttu-id="6f351-147">Die Eigenschaft ist nicht einzeln erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6f351-147">The property is not individually required.</span></span> <span data-ttu-id="6f351-148">Mindestens eine Eigenschaft (DisplayName oder MailNickname) ist jedoch erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6f351-148">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="6f351-149">onBehalfOfUserId</span><span class="sxs-lookup"><span data-stu-id="6f351-149">onBehalfOfUserId</span></span>|<span data-ttu-id="6f351-150">Guid</span><span class="sxs-lookup"><span data-stu-id="6f351-150">Guid</span></span>| <span data-ttu-id="6f351-151">Die Objekt-ID des Benutzers zum imitieren beim Aufrufen der API.</span><span class="sxs-lookup"><span data-stu-id="6f351-151">The object ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="6f351-152">Die Überprüfungsergebnisse werden für die OnBehalfOfUserId Attribute und Rollen.</span><span class="sxs-lookup"><span data-stu-id="6f351-152">The validation results are for the onBehalfOfUserId's attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="6f351-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="6f351-153">Response</span></span>
<span data-ttu-id="6f351-154">Bei erfolgreicher und es liegen keine Validierungsfehler, die Methode gibt `204 No Content` Antwortcode.</span><span class="sxs-lookup"><span data-stu-id="6f351-154">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="6f351-155">Es gibt keine Suchzeichenfolge im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6f351-155">It does not return anything in the response body.</span></span>

<span data-ttu-id="6f351-156">Wenn die Anforderung ungültig ist, gibt die Methode `400 Bad Request` Antwortcode.</span><span class="sxs-lookup"><span data-stu-id="6f351-156">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="6f351-157">Eine Fehlermeldung mit Details über die ungültige Anforderung wird in der Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6f351-157">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="6f351-158">Wenn ein Gültigkeitsprüfungsfehler vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="6f351-158">If there is a validation error.</span></span> <span data-ttu-id="6f351-159">Gibt die Methode `422 Unprocessable Entity` Antwortcode.</span><span class="sxs-lookup"><span data-stu-id="6f351-159">The method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="6f351-160">In den Antworttext wird eine Fehlermeldung angezeigt und eine Auflistung von Fehlerdetails zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6f351-160">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6f351-161">Beispiele</span><span class="sxs-lookup"><span data-stu-id="6f351-161">Examples</span></span>

<span data-ttu-id="6f351-162">Dies ist ein Beispiel für eine Anforderung erfolgreicher Überprüfung.</span><span class="sxs-lookup"><span data-stu-id="6f351-162">This is an example of a successful validation request.</span></span>

### <a name="request"></a><span data-ttu-id="6f351-163">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6f351-163">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "group_validateproperties"
}-->
``` http
POST https://graph.microsoft.com/beta/groups/{id}/validateProperties
Content-type: application/json
Content-length: 132

{
  "displayName": "Myprefix_test_mysuffix",
  "mailNickname": "Myprefix_test_mysuffix",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```

### <a name="response"></a><span data-ttu-id="6f351-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="6f351-164">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="6f351-165">Dies ist ein Beispiel für eine Anforderung mit Überprüfungsfehlern.</span><span class="sxs-lookup"><span data-stu-id="6f351-165">This is an example of a request with validation errors.</span></span>

### <a name="request"></a><span data-ttu-id="6f351-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6f351-166">Request</span></span>
``` http
POST https://graph.microsoft.com/beta/groups/{id}/validateProperties
Content-type: application/json
Content-length: 128

{
  "displayName": "MyPrefix_test_mysuffix",
  "mailNickname": "MyPrefix_test_mysuffix"
}
```

### <a name="response"></a><span data-ttu-id="6f351-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="6f351-167">Response</span></span>
```http
HTTP/1.1 422
Content-type: application/json
Content-length: 223

{
  "error": {
    "code": "Request_UnprocessableEntity",
    "message": "The values provided contain one or more validation errors.",
    "innerError": {
      "request-id": "id-value",
      "date": "date-value"
    },
    "details": [
      {
        "target": "mailNickname",
        "code": "PropertyConflict",
        "message": "Another object with the same value for property mailNickname already exists."
      }
    ]
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: validateProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
