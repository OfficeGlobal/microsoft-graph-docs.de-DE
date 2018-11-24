# <a name="add-tab-to-channel"></a><span data-ttu-id="215be-101">Registerkarte Channel hinzufügen</span><span class="sxs-lookup"><span data-stu-id="215be-101">Add tab to channel</span></span>



<span data-ttu-id="215be-102">Fügt (Pins) einer [Registerkarte](../resources/teamstab.md) an den angegebenen [DDE-Kanal](../resources/channel.md) in einem [Team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="215be-102">Adds (pins) a [tab](../resources/teamstab.md) to the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> <span data-ttu-id="215be-103">Die entsprechende app muss bereits [im Team installiert](../api/teamsappinstallation_add.md)sein.</span><span class="sxs-lookup"><span data-stu-id="215be-103">The corresponding app must already be [installed in the team](../api/teamsappinstallation_add.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="215be-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="215be-104">Permissions</span></span>
<span data-ttu-id="215be-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="215be-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="215be-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="215be-107">Permission type</span></span>      | <span data-ttu-id="215be-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="215be-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="215be-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="215be-109">Delegated (work or school account)</span></span> | <span data-ttu-id="215be-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="215be-110">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="215be-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="215be-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="215be-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="215be-112">Not supported.</span></span>    |
| <span data-ttu-id="215be-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="215be-113">Application</span></span>                            | <span data-ttu-id="215be-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="215be-114">Group.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="215be-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="215be-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/tabs
```

## <a name="request-headers"></a><span data-ttu-id="215be-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="215be-116">Request headers</span></span>
| <span data-ttu-id="215be-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="215be-117">Header</span></span>       | <span data-ttu-id="215be-118">Wert</span><span class="sxs-lookup"><span data-stu-id="215be-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="215be-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="215be-119">Authorization</span></span>  | <span data-ttu-id="215be-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="215be-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="215be-122">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="215be-122">Request body</span></span>

<span data-ttu-id="215be-123">Ein [TeamsTab](../resources/teamstab.md).</span><span class="sxs-lookup"><span data-stu-id="215be-123">A [teamsTab](../resources/teamstab.md).</span></span>

## <a name="response"></a><span data-ttu-id="215be-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="215be-124">Response</span></span>

<span data-ttu-id="215be-125">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `201 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="215be-125">If successful, this method returns a `201 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="215be-126">Beispiel</span><span class="sxs-lookup"><span data-stu-id="215be-126">Example</span></span>

#### <a name="request"></a><span data-ttu-id="215be-127">Anforderung</span><span class="sxs-lookup"><span data-stu-id="215be-127">Request</span></span>

<span data-ttu-id="215be-128">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="215be-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs
{
  "name": "My Contoso Tab",
  "teamsApp@odata.bind" : "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  }
}
```

#### <a name="response"></a><span data-ttu-id="215be-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="215be-129">Response</span></span>

<span data-ttu-id="215be-130">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="215be-130">The following is an example of the response.</span></span> <span data-ttu-id="215be-131">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="215be-131">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="215be-132">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="215be-132">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "794f0e4e-4d10-4bb5-9079-3a465a629eff",
  "name": "My Contoso Tab",
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

## <a name="see-also"></a><span data-ttu-id="215be-133">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="215be-133">See also</span></span>

[<span data-ttu-id="215be-134">Konfigurieren der integrierten Registerkartentypen</span><span class="sxs-lookup"><span data-stu-id="215be-134">Configuring the built-in tab types</span></span>](../../../concepts/teams-configuring-builtin-tabs.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Add tab to channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
