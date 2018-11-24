# <a name="delete-app-from-team"></a><span data-ttu-id="ebf6d-101">Löschen von app-Teams</span><span class="sxs-lookup"><span data-stu-id="ebf6d-101">Delete app from team</span></span>



<span data-ttu-id="ebf6d-102">Deinstalliert eine [app](../resources/teamsappinstallation.md) aus dem angegebenen [Team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="ebf6d-102">Uninstalls an [app](../resources/teamsappinstallation.md) from the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ebf6d-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ebf6d-103">Permissions</span></span>
<span data-ttu-id="ebf6d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ebf6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ebf6d-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ebf6d-106">Permission type</span></span>      | <span data-ttu-id="ebf6d-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ebf6d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ebf6d-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ebf6d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ebf6d-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebf6d-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ebf6d-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ebf6d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebf6d-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ebf6d-111">Not supported.</span></span>    |
|<span data-ttu-id="ebf6d-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ebf6d-112">Application</span></span> | <span data-ttu-id="ebf6d-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ebf6d-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ebf6d-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ebf6d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ebf6d-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ebf6d-115">Request headers</span></span>
| <span data-ttu-id="ebf6d-116">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ebf6d-116">Header</span></span>       | <span data-ttu-id="ebf6d-117">Wert</span><span class="sxs-lookup"><span data-stu-id="ebf6d-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ebf6d-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="ebf6d-118">Authorization</span></span>  | <span data-ttu-id="ebf6d-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ebf6d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ebf6d-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ebf6d-121">Request body</span></span>
<span data-ttu-id="ebf6d-122">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ebf6d-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ebf6d-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="ebf6d-123">Response</span></span>

<span data-ttu-id="ebf6d-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ebf6d-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebf6d-126">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ebf6d-126">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ebf6d-127">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ebf6d-127">Request</span></span>
<span data-ttu-id="ebf6d-128">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ebf6d-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/installedApps/{id}
```
#### <a name="response"></a><span data-ttu-id="ebf6d-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="ebf6d-129">Response</span></span>
<span data-ttu-id="ebf6d-130">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ebf6d-130">The following is an example of the response.</span></span> <span data-ttu-id="ebf6d-131">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="ebf6d-131">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ebf6d-132">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ebf6d-132">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 204 No Content
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
