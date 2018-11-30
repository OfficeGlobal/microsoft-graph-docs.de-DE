---
title: 'outlookUser: supportedTimeZones'
description: Abrufen der Liste von Zeitzonen, die für den Benutzer unterstützt werden, wie auf dem Postfachserver des Benutzers konfiguriert.
ms.openlocfilehash: c5886cc435b482a0acfcd99c65f356efe3a99d59
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058768"
---
# <a name="outlookuser-supportedtimezones"></a><span data-ttu-id="4c7ae-103">outlookUser: supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="4c7ae-103">outlookUser: supportedTimeZones</span></span>

> <span data-ttu-id="4c7ae-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4c7ae-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4c7ae-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4c7ae-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4c7ae-106">Abrufen der Liste von Zeitzonen, die für den Benutzer unterstützt werden, wie auf dem Postfachserver des Benutzers konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="4c7ae-106">Get the list of time zones that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="4c7ae-107">Sie können explizit angeben, dass Zeitzonen im Windows-Zeitzonenformat oder im [IANA-Format (Internet Assigned Numbers Authority)](https://www.iana.org/time-zones) (auch als Olson-Zeitzone bezeichnet) zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="4c7ae-107">You can explicitly specify to have time zones returned in the Windows time zone format or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="4c7ae-108">Das Windows-Format ist die Standardeinstellung.</span><span class="sxs-lookup"><span data-stu-id="4c7ae-108">The Windows format is the default.</span></span>

<span data-ttu-id="4c7ae-109">Beim Einrichten eines Outlook-Clients wählt der Benutzer die bevorzugte Zeitzone aus dieser unterstützten Liste aus.</span><span class="sxs-lookup"><span data-stu-id="4c7ae-109">When setting up an Outlook client, the user selects the preferred time zone from this supported list.</span></span> <span data-ttu-id="4c7ae-110">Sie können anschließend die bevorzugte Zeitzone abrufen, indem Sie [die Postfacheinstellungen des Benutzers abrufen](user-get-mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="4c7ae-110">You can subsequently get the preferred time zone by [getting the user's mailbox settings](user-get-mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="4c7ae-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4c7ae-111">Permissions</span></span>
<span data-ttu-id="4c7ae-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c7ae-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c7ae-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4c7ae-114">Permission type</span></span>      | <span data-ttu-id="4c7ae-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4c7ae-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c7ae-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4c7ae-116">Delegated (work or school account)</span></span> | <span data-ttu-id="4c7ae-117">User.Read, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="4c7ae-117">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="4c7ae-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4c7ae-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c7ae-119">User.Read</span><span class="sxs-lookup"><span data-stu-id="4c7ae-119">User.Read</span></span>    |
|<span data-ttu-id="4c7ae-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4c7ae-120">Application</span></span> | <span data-ttu-id="4c7ae-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4c7ae-121">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c7ae-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4c7ae-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedTimeZones
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones

GET /me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
```

## <a name="function-parameters"></a><span data-ttu-id="4c7ae-123">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="4c7ae-123">Function parameters</span></span>
| <span data-ttu-id="4c7ae-124">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="4c7ae-124">Function parameter</span></span>       | <span data-ttu-id="4c7ae-125">Typ</span><span class="sxs-lookup"><span data-stu-id="4c7ae-125">Type</span></span> | <span data-ttu-id="4c7ae-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4c7ae-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4c7ae-127">TimeZoneStandard</span><span class="sxs-lookup"><span data-stu-id="4c7ae-127">TimeZoneStandard</span></span>  | <span data-ttu-id="4c7ae-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4c7ae-128">String</span></span>  | <span data-ttu-id="4c7ae-129">Ein Zeitzonenformat.</span><span class="sxs-lookup"><span data-stu-id="4c7ae-129">A time zone format.</span></span> <span data-ttu-id="4c7ae-130">Unterstützte Werte sind: `Windows` und `Iana`.</span><span class="sxs-lookup"><span data-stu-id="4c7ae-130">Supported values are: `Windows`, and `Iana`.</span></span> <span data-ttu-id="4c7ae-131">Optional.</span><span class="sxs-lookup"><span data-stu-id="4c7ae-131">Optional.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="4c7ae-132">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4c7ae-132">Request headers</span></span>
| <span data-ttu-id="4c7ae-133">Name</span><span class="sxs-lookup"><span data-stu-id="4c7ae-133">Name</span></span>       | <span data-ttu-id="4c7ae-134">Typ</span><span class="sxs-lookup"><span data-stu-id="4c7ae-134">Type</span></span> | <span data-ttu-id="4c7ae-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4c7ae-135">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4c7ae-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c7ae-136">Authorization</span></span>  | <span data-ttu-id="4c7ae-137">string</span><span class="sxs-lookup"><span data-stu-id="4c7ae-137">string</span></span>  | <span data-ttu-id="4c7ae-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4c7ae-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4c7ae-140">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4c7ae-140">Request body</span></span>
<span data-ttu-id="4c7ae-141">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4c7ae-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c7ae-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="4c7ae-142">Response</span></span>
<span data-ttu-id="4c7ae-143">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Sammlung von [timeZoneInformation](../resources/timezoneinformation.md)-Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="4c7ae-143">If successful, this method returns `200 OK` response code and a collection of [timeZoneInformation](../resources/timezoneinformation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c7ae-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4c7ae-144">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="4c7ae-145">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="4c7ae-145">Request 1</span></span>
<span data-ttu-id="4c7ae-146">Im folgenden Beispiel wird der `timeZoneStandard`-Parameter nicht angegeben, und es wird eine Liste unterstützter Zeitzonen abgerufen, die im Windows-Zeitzonenformat dargestellt werden.</span><span class="sxs-lookup"><span data-stu-id="4c7ae-146">The following example does not specify the `timeZoneStandard` parameter, and gets the list of supported time zones represented in the Windows time zone format.</span></span> 
<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_default"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/supportedTimeZones
```

##### <a name="response-1"></a><span data-ttu-id="4c7ae-147">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="4c7ae-147">Response 1</span></span>
<span data-ttu-id="4c7ae-148">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4c7ae-148">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "name": "user_supportedtimezones_default",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeZoneInformation",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.timeZoneInformation)",
  "value":[
    {
      "alias":"Dateline Standard Time",
      "displayName":"(UTC-12:00) International Date Line West"
    },
    {
      "alias":"Samoa Standard Time",
      "displayName":"(UTC+13:00) Samoa"
    },
    {
       "alias":"UTC-11",
       "displayName":"(UTC-11:00) Coordinated Universal Time-11"
    },
    {
      "alias":"Aleutian Standard Time",
      "displayName":"(UTC-10:00) Aleutian Islands"
    }
  ]
}
```

##### <a name="request-2"></a><span data-ttu-id="4c7ae-149">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="4c7ae-149">Request 2</span></span>
<span data-ttu-id="4c7ae-150">Im folgenden Beispiel wird `Iana` für den `TimeZoneStandard`-Parameter angegeben und die Liste der unterstützten Zeitzonen abgerufen, die im IANA-Format dargestellt werden.</span><span class="sxs-lookup"><span data-stu-id="4c7ae-150">The following example specifies `Iana` for the `TimeZoneStandard` parameter, and gets the list of supported time zones represented in IANA format.</span></span> 

<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_iana"
} -->

```http
GET https://graph.microsoft.com/beta/me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'Iana')
```

##### <a name="response-2"></a><span data-ttu-id="4c7ae-151">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="4c7ae-151">Response 2</span></span>
<span data-ttu-id="4c7ae-152">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4c7ae-152">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "name": "user_supportedtimezones_iana",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeZoneInformation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.timeZoneInformation)",
  "value":[
    {
      "alias":"Etc/GMT+12",
      "displayName":"Etc/GMT+12"
    },
    {
      "alias":"US/Samoa",
      "displayName":"US/Samoa"
    },
    {
      "alias":"Etc/GMT+11",
      "displayName":"Etc/GMT+11"
    },
    {
      "alias":"US/Aleutian",
      "displayName":"US/Aleutian"
    }
  ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: supportedTimeZones",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->