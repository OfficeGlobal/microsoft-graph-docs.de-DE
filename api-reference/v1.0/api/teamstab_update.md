# <a name="update-tab"></a><span data-ttu-id="97fb8-101">Registerkarte "Aktualisieren"</span><span class="sxs-lookup"><span data-stu-id="97fb8-101">Update tab</span></span>



<span data-ttu-id="97fb8-102">Aktualisieren Sie die Eigenschaften der angegebenen [Registerkarte](../resources/teamstab.md). Dies kann so konfigurieren Sie den Inhalt der Registerkarte verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="97fb8-102">Update the properties of the specified [tab](../resources/teamstab.md). This can be used to configure the content of the tab.</span></span>

## <a name="permissions"></a><span data-ttu-id="97fb8-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="97fb8-103">Permissions</span></span>
<span data-ttu-id="97fb8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="97fb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="97fb8-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="97fb8-106">Permission type</span></span>      | <span data-ttu-id="97fb8-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="97fb8-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97fb8-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="97fb8-108">Delegated (work or school account)</span></span> | <span data-ttu-id="97fb8-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97fb8-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="97fb8-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="97fb8-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97fb8-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="97fb8-111">Not supported.</span></span>    |
|<span data-ttu-id="97fb8-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="97fb8-112">Application</span></span>                            | <span data-ttu-id="97fb8-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97fb8-113">Group.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="97fb8-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="97fb8-114">HTTP request</span></span>
```http
PATCH /teams/{id}/channels/{id}/tabs/{id}
```
## <a name="request-headers"></a><span data-ttu-id="97fb8-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="97fb8-115">Request headers</span></span>
| <span data-ttu-id="97fb8-116">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="97fb8-116">Header</span></span>       | <span data-ttu-id="97fb8-117">Wert</span><span class="sxs-lookup"><span data-stu-id="97fb8-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="97fb8-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="97fb8-118">Authorization</span></span>  | <span data-ttu-id="97fb8-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="97fb8-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="97fb8-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="97fb8-121">Content-Type</span></span>  | <span data-ttu-id="97fb8-122">application/json</span><span class="sxs-lookup"><span data-stu-id="97fb8-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="97fb8-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="97fb8-123">Request body</span></span>
<span data-ttu-id="97fb8-124">Geben Sie im Textkörper Anforderung eine JSON-Darstellung der [Tab](../resources/teamstab.md) -Objekt.</span><span class="sxs-lookup"><span data-stu-id="97fb8-124">In the request body, supply a JSON representation of [tab](../resources/teamstab.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="97fb8-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="97fb8-125">Response</span></span>

<span data-ttu-id="97fb8-126">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="97fb8-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="97fb8-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="97fb8-127">Example</span></span>
#### <a name="request"></a><span data-ttu-id="97fb8-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="97fb8-128">Request</span></span>
<span data-ttu-id="97fb8-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="97fb8-129">The following is an example of the request.</span></span>
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
Content-type: application/json
Content-length: 211

{
  "name": "My Contoso Tab - updated"
}
```
#### <a name="response"></a><span data-ttu-id="97fb8-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="97fb8-130">Response</span></span>
```http
HTTP/1.1 200 Success
Content-type: application/json

{
  "id": "tabId",
  "name": "My Contoso Tab - updated",
  "teamsAppId": "06805b9e-77e3-4b93-ac81-525eb87513b8",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  },
  "sortOrderIndex": 20,
  "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3afd736d46-51ed-4c0b-9b23-e67ca354bb24?label=my%20%contoso%to%tab"
}
```

## <a name="see-also"></a><span data-ttu-id="97fb8-131">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="97fb8-131">See also</span></span>

[<span data-ttu-id="97fb8-132">Konfigurieren der integrierten Registerkartentypen</span><span class="sxs-lookup"><span data-stu-id="97fb8-132">Configuring the built-in tab types</span></span>](../../../concepts/teams-configuring-builtin-tabs.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tab in channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
