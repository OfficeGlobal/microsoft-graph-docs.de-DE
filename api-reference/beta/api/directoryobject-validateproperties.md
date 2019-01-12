---
title: 'DirectoryObject: ValidateProperties'
description: Überprüfen Sie, ob eine Office 365-Gruppe Display Name oder die e-Mail-Spitzname naming Richtlinien entspricht.  Clients können mithilfe der API bestimmen, ob ein Anzeigename oder e-Mail-Spitzname ist gültig, bevor Sie versuchen, eine Office 365-Gruppe zu **Erstellen** . Verwenden Sie zum Überprüfen von Eigenschaften einer vorhandenen Gruppe, die ValidateProperties-Funktion für Gruppen.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 515acb022150d091e7dcbbdecc1fb1adef849a88
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921318"
---
# <a name="directoryobject-validateproperties"></a><span data-ttu-id="c4479-105">DirectoryObject: ValidateProperties</span><span class="sxs-lookup"><span data-stu-id="c4479-105">directoryObject: validateProperties</span></span>

<span data-ttu-id="c4479-106">Überprüfen Sie, ob eine Office 365-Gruppe Display Name oder die e-Mail-Spitzname naming Richtlinien entspricht.</span><span class="sxs-lookup"><span data-stu-id="c4479-106">Validate if an Office 365 group's display name or mail nickname complies with naming policies.</span></span>  <span data-ttu-id="c4479-107">Clients können mithilfe der API bestimmen, ob ein Anzeigename oder e-Mail-Spitzname ist gültig, bevor Sie versuchen, eine Office 365-Gruppe zu **Erstellen** .</span><span class="sxs-lookup"><span data-stu-id="c4479-107">Clients can use the API to determine if a display name or mail nickname is valid before trying to **create** an Office 365 group.</span></span> <span data-ttu-id="c4479-108">Zum Überprüfen von Eigenschaften einer vorhandenen Gruppe, verwenden Sie die [Funktion ValidateProperties](group-validateproperties.md) für Gruppen.</span><span class="sxs-lookup"><span data-stu-id="c4479-108">For validating properties of an existing group, use the [validateProperties function](group-validateproperties.md) for groups.</span></span>

<span data-ttu-id="c4479-109">Für die Namen und e-Mail-Spitzname Anzeigeeigenschaften werden die folgenden Überprüfungen ausgeführt:</span><span class="sxs-lookup"><span data-stu-id="c4479-109">The following validations are performed for the display name and mail nickname properties:</span></span> 
1. <span data-ttu-id="c4479-110">Überprüfen Sie das Präfix und Suffix Richtlinie zum Benennen</span><span class="sxs-lookup"><span data-stu-id="c4479-110">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="c4479-111">Überprüfen Sie die benutzerdefinierten gesperrten Wörter-Richtlinie</span><span class="sxs-lookup"><span data-stu-id="c4479-111">Validate the custom banned words policy</span></span>
3. <span data-ttu-id="c4479-112">Überprüfen Sie die e-Mail-Nachricht Spitzname eindeutig ist.</span><span class="sxs-lookup"><span data-stu-id="c4479-112">Validate the mail nickname is unique</span></span>

<span data-ttu-id="c4479-113">Diese API zurückgegeben mit ersten Fehler.</span><span class="sxs-lookup"><span data-stu-id="c4479-113">This API returns with the first failure encountered.</span></span> <span data-ttu-id="c4479-114">Wenn mehrere Überprüfungen eine oder mehrere Eigenschaften ein Fehler auftritt, wird nur die-Eigenschaft mit den ersten Validierungsfehler zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c4479-114">If one or more properties fail multiple validations, only the property with the first validation failure is returned.</span></span> <span data-ttu-id="c4479-115">Sie können jedoch überprüft e-Mail-Spitznamen und den Anzeigenamen und eine Auflistung von Validierungsfehlern empfangen, wenn Sie nur das Präfix und Suffix Richtlinie zum Benennen überprüfen.</span><span class="sxs-lookup"><span data-stu-id="c4479-115">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4479-116">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c4479-116">Prerequisites</span></span>

<span data-ttu-id="c4479-117">Die folgende **Berechtigung** ist erforderlich, um diese API ausführen: *Group.Read.All*</span><span class="sxs-lookup"><span data-stu-id="c4479-117">The following **permission** is required to execute this API: *Group.Read.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="c4479-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c4479-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /directoryObjects/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="c4479-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c4479-119">Request headers</span></span>

| <span data-ttu-id="c4479-120">Name</span><span class="sxs-lookup"><span data-stu-id="c4479-120">Name</span></span>           | <span data-ttu-id="c4479-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c4479-121">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="c4479-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4479-122">Authorization</span></span>  | <span data-ttu-id="c4479-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c4479-123">Bearer {code}</span></span>    |
| <span data-ttu-id="c4479-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c4479-124">Content-Type</span></span>   | <span data-ttu-id="c4479-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c4479-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c4479-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c4479-126">Request body</span></span>
<span data-ttu-id="c4479-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="c4479-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c4479-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="c4479-128">Parameter</span></span>    | <span data-ttu-id="c4479-129">Typ</span><span class="sxs-lookup"><span data-stu-id="c4479-129">Type</span></span>   |<span data-ttu-id="c4479-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c4479-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c4479-131">entityType</span><span class="sxs-lookup"><span data-stu-id="c4479-131">entityType</span></span>|<span data-ttu-id="c4479-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c4479-132">String</span></span>| <span data-ttu-id="c4479-133">`Group`ist der einzige unterstützte Entitätstyp an.</span><span class="sxs-lookup"><span data-stu-id="c4479-133">`Group` is the only supported entity type.</span></span> |
|<span data-ttu-id="c4479-134">displayName</span><span class="sxs-lookup"><span data-stu-id="c4479-134">displayName</span></span>|<span data-ttu-id="c4479-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c4479-135">String</span></span>| <span data-ttu-id="c4479-136">Der Anzeigename der Gruppe zu überprüfen.</span><span class="sxs-lookup"><span data-stu-id="c4479-136">The display name of the group to validate.</span></span> <span data-ttu-id="c4479-137">Die Eigenschaft ist nicht einzeln erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c4479-137">The property is not individually required.</span></span> <span data-ttu-id="c4479-138">Mindestens eine Eigenschaft (DisplayName oder MailNickname) ist jedoch erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c4479-138">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="c4479-139">mailNickname</span><span class="sxs-lookup"><span data-stu-id="c4479-139">mailNickname</span></span>|<span data-ttu-id="c4479-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c4479-140">String</span></span>| <span data-ttu-id="c4479-141">Die e-Mail-Spitzname der Gruppe zu überprüfen.</span><span class="sxs-lookup"><span data-stu-id="c4479-141">The mail nickname of the group to validate.</span></span> <span data-ttu-id="c4479-142">Die Eigenschaft ist nicht einzeln erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c4479-142">The property is not individually required.</span></span> <span data-ttu-id="c4479-143">Mindestens eine Eigenschaft (DisplayName oder MailNickname) ist jedoch erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c4479-143">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="c4479-144">onBehalfOfUserId</span><span class="sxs-lookup"><span data-stu-id="c4479-144">onBehalfOfUserId</span></span>|<span data-ttu-id="c4479-145">Guid</span><span class="sxs-lookup"><span data-stu-id="c4479-145">Guid</span></span>| <span data-ttu-id="c4479-146">Die Objekt-ID des Benutzers zum imitieren beim Aufrufen der API.</span><span class="sxs-lookup"><span data-stu-id="c4479-146">The object ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="c4479-147">Die Überprüfungsergebnisse werden für die OnBehalfOfUserId Attribute und Rollen.</span><span class="sxs-lookup"><span data-stu-id="c4479-147">The validation results are for the onBehalfOfUserId's attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="c4479-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="c4479-148">Response</span></span>

<span data-ttu-id="c4479-149">Bei erfolgreicher und es liegen keine Validierungsfehler, die Methode gibt `204 No Content` Antwortcode.</span><span class="sxs-lookup"><span data-stu-id="c4479-149">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="c4479-150">Es gibt keine Suchzeichenfolge im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c4479-150">It does not return anything in the response body.</span></span>

<span data-ttu-id="c4479-151">Wenn die Anforderung ungültig ist, gibt die Methode `400 Bad Request` Antwortcode.</span><span class="sxs-lookup"><span data-stu-id="c4479-151">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="c4479-152">Eine Fehlermeldung mit Details über die ungültige Anforderung wird in der Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c4479-152">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="c4479-153">Wenn ein Gültigkeitsprüfungsfehler vorhanden ist, gibt die Methode `422 Unprocessable Entity` Antwortcode.</span><span class="sxs-lookup"><span data-stu-id="c4479-153">If there is a validation error, the method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="c4479-154">In den Antworttext wird eine Fehlermeldung angezeigt und eine Auflistung von Fehlerdetails zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c4479-154">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c4479-155">Beispiele</span><span class="sxs-lookup"><span data-stu-id="c4479-155">Examples</span></span>

<span data-ttu-id="c4479-156">Dies ist ein Beispiel für eine Anforderung erfolgreicher Überprüfung.</span><span class="sxs-lookup"><span data-stu-id="c4479-156">This is an example of a successful validation request.</span></span>

### <a name="request"></a><span data-ttu-id="c4479-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c4479-157">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "directoryobject_validateproperties"
}-->
``` http
POST https://graph.microsoft.com/directoryObjects/validateProperties
Content-type: application/json
Content-length: 164

{
  "entityType": "Group",
  "displayName": "Myprefix_test_mysuffix",
  "mailNickname": "Myprefix_test_mysuffix",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```

### <a name="response"></a><span data-ttu-id="c4479-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="c4479-158">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="c4479-159">Dies ist ein Beispiel für eine Anforderung mit Überprüfungsfehlern.</span><span class="sxs-lookup"><span data-stu-id="c4479-159">This is an example of a request with validation errors.</span></span>

### <a name="request"></a><span data-ttu-id="c4479-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c4479-160">Request</span></span>
```http
POST https://graph.microsoft.com/directoryObjects/validateProperties
Content-type: application/json
Content-length: 164

{
  "entityType": "Group",
  "displayName": "test",
  "mailNickname": "test",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```

### <a name="response"></a><span data-ttu-id="c4479-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="c4479-161">Response</span></span>
```http
HTTP/1.1 422 
Content-Type: application/json

{
  "error": {
    "code": "Request_UnprocessableEntity",
    "message": "The values provided contain one or more validation errors.",
    "innerError": {
      "request-id": "request-id-value",
      "date": "date-value"
    },
    "details": [
      {
        "target": "displayName",
        "code": "MissingPrefixSuffix",
        "message": "Property mailNickname is missing a required prefix/suffix per your organization's Group naming requirements.",
        "prefix": "Myprefix_",
        "suffix": "_mysuffix"
      },
      {
        "target": "mailNickname",
        "code": "MissingPrefixSuffix",
        "message": "Property mailNickname is missing a required prefix/suffix per your organization's Group naming requirements.",
        "prefix": "Myprefix_",
        "suffix": "_mysuffix"
      }
    ]
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: validateProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
