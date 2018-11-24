# <a name="outlookuser-supportedtimezones"></a><span data-ttu-id="fd72b-101">outlookUser: supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="fd72b-101">outlookUser: supportedTimeZones</span></span>

<span data-ttu-id="fd72b-102">Abrufen der Liste von Zeitzonen, die für den Benutzer unterstützt werden, wie auf dem Postfachserver des Benutzers konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="fd72b-102">Get the list of time zones that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="fd72b-103">Sie können explizit angeben, dass Zeitzonen im Windows-Zeitzonenformat oder im [IANA-Format (Internet Assigned Numbers Authority)](https://www.iana.org/time-zones) (auch als Olson-Zeitzone bezeichnet) zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="fd72b-103">You can explicitly specify to have time zones returned in the Windows time zone format or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="fd72b-104">Das Windows-Format ist die Standardeinstellung.</span><span class="sxs-lookup"><span data-stu-id="fd72b-104">The Windows format is the default.</span></span>

<span data-ttu-id="fd72b-105">Beim Einrichten eines Outlook-Clients wählt der Benutzer die bevorzugte Zeitzone aus dieser unterstützten Liste aus.</span><span class="sxs-lookup"><span data-stu-id="fd72b-105">When setting up an Outlook client, the user selects the preferred time zone from this supported list.</span></span> <span data-ttu-id="fd72b-106">Sie können anschließend die bevorzugte Zeitzone abrufen, indem Sie [die Postfacheinstellungen des Benutzers abrufen](user_get_mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="fd72b-106">You can subsequently get the preferred time zone by [getting the user's mailbox settings](user_get_mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="fd72b-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fd72b-107">Permissions</span></span>
<span data-ttu-id="fd72b-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fd72b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fd72b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fd72b-110">Permission type</span></span>      | <span data-ttu-id="fd72b-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fd72b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd72b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fd72b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fd72b-113">User.Read, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="fd72b-113">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="fd72b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fd72b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd72b-115">User.Read</span><span class="sxs-lookup"><span data-stu-id="fd72b-115">User.Read</span></span>    |
|<span data-ttu-id="fd72b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fd72b-116">Application</span></span> | <span data-ttu-id="fd72b-117">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="fd72b-117">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fd72b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fd72b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedTimeZones
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones

GET /me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
```

## <a name="function-parameters"></a><span data-ttu-id="fd72b-119">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="fd72b-119">Function parameters</span></span>
| <span data-ttu-id="fd72b-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="fd72b-120">Parameter</span></span>       | <span data-ttu-id="fd72b-121">Typ</span><span class="sxs-lookup"><span data-stu-id="fd72b-121">Type</span></span> | <span data-ttu-id="fd72b-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fd72b-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fd72b-123">TimeZoneStandard</span><span class="sxs-lookup"><span data-stu-id="fd72b-123">TimeZoneStandard</span></span>  | <span data-ttu-id="fd72b-124">timeZoneStandard</span><span class="sxs-lookup"><span data-stu-id="fd72b-124">timeZoneStandard</span></span>  | <span data-ttu-id="fd72b-125">Ein Zeitzonenformat.</span><span class="sxs-lookup"><span data-stu-id="fd72b-125">A time zone format.</span></span> <span data-ttu-id="fd72b-126">Unterstützte Werte sind: `Windows` und `Iana`.</span><span class="sxs-lookup"><span data-stu-id="fd72b-126">Supported values are: `Windows`, and `Iana`.</span></span> <span data-ttu-id="fd72b-127">Optional.</span><span class="sxs-lookup"><span data-stu-id="fd72b-127">Optional.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="fd72b-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fd72b-128">Request headers</span></span>
| <span data-ttu-id="fd72b-129">Name</span><span class="sxs-lookup"><span data-stu-id="fd72b-129">Name</span></span>       | <span data-ttu-id="fd72b-130">Typ</span><span class="sxs-lookup"><span data-stu-id="fd72b-130">Type</span></span> | <span data-ttu-id="fd72b-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fd72b-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fd72b-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd72b-132">Authorization</span></span>  | <span data-ttu-id="fd72b-133">string</span><span class="sxs-lookup"><span data-stu-id="fd72b-133">string</span></span>  | <span data-ttu-id="fd72b-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fd72b-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fd72b-136">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fd72b-136">Request body</span></span>
<span data-ttu-id="fd72b-137">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fd72b-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd72b-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="fd72b-138">Response</span></span>
<span data-ttu-id="fd72b-139">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Sammlung von [timeZoneInformation](../resources/timezoneinformation.md)-Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="fd72b-139">If successful, this method returns `200 OK` response code and a collection of [timeZoneInformation](../resources/timezoneinformation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd72b-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fd72b-140">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="fd72b-141">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="fd72b-141">Request 1</span></span>
<span data-ttu-id="fd72b-142">Im folgenden Beispiel wird der `timeZoneStandard`-Parameter nicht angegeben, und es wird eine Liste unterstützter Zeitzonen abgerufen, die im Windows-Zeitzonenformat dargestellt werden.</span><span class="sxs-lookup"><span data-stu-id="fd72b-142">The following example does not specify the `timeZoneStandard` parameter, and gets the list of supported time zones represented in the Windows time zone format.</span></span> 
<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_default"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/outlook/supportedTimeZones
```

##### <a name="response-1"></a><span data-ttu-id="fd72b-143">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="fd72b-143">Response 1</span></span>
<span data-ttu-id="fd72b-144">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fd72b-144">Here is an example of the response.</span></span> 
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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.timeZoneInformation)",
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

##### <a name="request-2"></a><span data-ttu-id="fd72b-145">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="fd72b-145">Request 2</span></span>
<span data-ttu-id="fd72b-146">Im folgenden Beispiel wird `Iana` für den `TimeZoneStandard`-Parameter angegeben und die Liste der unterstützten Zeitzonen abgerufen, die im IANA-Format dargestellt werden.</span><span class="sxs-lookup"><span data-stu-id="fd72b-146">The following example specifies `Iana` for the `TimeZoneStandard` parameter, and gets the list of supported time zones represented in IANA format.</span></span> 

<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_iana"
} -->

```http
GET https://graph.microsoft.com/v1.0/me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'Iana')
```

##### <a name="response-2"></a><span data-ttu-id="fd72b-147">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="fd72b-147">Response 2</span></span>
<span data-ttu-id="fd72b-148">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fd72b-148">Here is an example of the response.</span></span> 

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.timeZoneInformation)",
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