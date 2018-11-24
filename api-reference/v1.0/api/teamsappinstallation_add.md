# <a name="add-app-to-team"></a><span data-ttu-id="e21cf-101">Team app hinzufügen</span><span class="sxs-lookup"><span data-stu-id="e21cf-101">Add app to team</span></span>



<span data-ttu-id="e21cf-102">Installiert das angegebene [Team](../resources/team.md)einer [app](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="e21cf-102">Installs an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e21cf-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e21cf-103">Permissions</span></span>
<span data-ttu-id="e21cf-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e21cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e21cf-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e21cf-106">Permission type</span></span>      | <span data-ttu-id="e21cf-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e21cf-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e21cf-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e21cf-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e21cf-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e21cf-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e21cf-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e21cf-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e21cf-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e21cf-111">Not supported.</span></span>    |
|<span data-ttu-id="e21cf-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e21cf-112">Application</span></span> | <span data-ttu-id="e21cf-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e21cf-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e21cf-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e21cf-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="e21cf-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e21cf-115">Request headers</span></span>
| <span data-ttu-id="e21cf-116">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e21cf-116">Header</span></span>       | <span data-ttu-id="e21cf-117">Wert</span><span class="sxs-lookup"><span data-stu-id="e21cf-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e21cf-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="e21cf-118">Authorization</span></span>  | <span data-ttu-id="e21cf-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e21cf-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e21cf-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e21cf-121">Request body</span></span>

| <span data-ttu-id="e21cf-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e21cf-122">Property</span></span>     | <span data-ttu-id="e21cf-123">Typ</span><span class="sxs-lookup"><span data-stu-id="e21cf-123">Type</span></span>   |<span data-ttu-id="e21cf-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e21cf-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e21cf-125">teamsApp</span><span class="sxs-lookup"><span data-stu-id="e21cf-125">teamsApp</span></span>| [<span data-ttu-id="e21cf-126">teamsApp</span><span class="sxs-lookup"><span data-stu-id="e21cf-126">teamsApp</span></span>](../resources/teamsapp.md) |<span data-ttu-id="e21cf-127">Die app hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="e21cf-127">The app to add.</span></span>|


## <a name="response"></a><span data-ttu-id="e21cf-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="e21cf-128">Response</span></span>

<span data-ttu-id="e21cf-129">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e21cf-129">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e21cf-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e21cf-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="e21cf-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e21cf-131">Request</span></span>
<span data-ttu-id="e21cf-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e21cf-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/installedApps
{
   "teamsApp@odata.bind":"https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```
#### <a name="response"></a><span data-ttu-id="e21cf-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="e21cf-133">Response</span></span>
<span data-ttu-id="e21cf-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e21cf-134">The following is an example of the response.</span></span> <span data-ttu-id="e21cf-135">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="e21cf-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e21cf-136">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e21cf-136">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a><span data-ttu-id="e21cf-137">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="e21cf-137">See also</span></span>

