# <a name="create-team"></a><span data-ttu-id="c7d2c-101">Erstellen von Teams</span><span class="sxs-lookup"><span data-stu-id="c7d2c-101">Create team</span></span>



<span data-ttu-id="c7d2c-102">Erstellen Sie ein neues [Team](../resources/team.md) unter einer [Gruppe](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="c7d2c-102">Create a new [team](../resources/team.md) under a [group](../resources/group.md).</span></span>

<span data-ttu-id="c7d2c-103">Um ein Team zu erstellen, muss die Gruppe einen mindestens einen Besitzer haben.</span><span class="sxs-lookup"><span data-stu-id="c7d2c-103">In order to create a team, the group must have a least one owner.</span></span>

<span data-ttu-id="c7d2c-104">Wenn die Gruppe vor weniger als 15 Minuten erstellt wurde, kann der erstellen teamanruf an einen Code 404-Fehler aufgrund von Replikation Verzögerungen auftreten.</span><span class="sxs-lookup"><span data-stu-id="c7d2c-104">If the group was created less than 15 minutes ago, it's possible for the Create team call to fail with a 404 error code due to replication delays.</span></span> <span data-ttu-id="c7d2c-105">Das empfohlene Muster liegt, um den Aufruf der Create-Team drei Mal mit einer Verzögerung von 10 Sekunden zwischen aufrufen.</span><span class="sxs-lookup"><span data-stu-id="c7d2c-105">The recommended pattern is to retry the Create team call three times, with a 10 second delay between calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7d2c-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c7d2c-106">Permissions</span></span>

<span data-ttu-id="c7d2c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c7d2c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c7d2c-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c7d2c-109">Permission type</span></span>      | <span data-ttu-id="c7d2c-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c7d2c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7d2c-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c7d2c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c7d2c-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7d2c-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c7d2c-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c7d2c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7d2c-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c7d2c-114">Not supported.</span></span>    |
|<span data-ttu-id="c7d2c-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c7d2c-115">Application</span></span> | <span data-ttu-id="c7d2c-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7d2c-116">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7d2c-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c7d2c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /groups/{id}/team
```

## <a name="request-headers"></a><span data-ttu-id="c7d2c-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c7d2c-118">Request headers</span></span>

| <span data-ttu-id="c7d2c-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c7d2c-119">Header</span></span>       | <span data-ttu-id="c7d2c-120">Wert</span><span class="sxs-lookup"><span data-stu-id="c7d2c-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c7d2c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7d2c-121">Authorization</span></span>  | <span data-ttu-id="c7d2c-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c7d2c-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c7d2c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c7d2c-124">Content-Type</span></span>  | <span data-ttu-id="c7d2c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c7d2c-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c7d2c-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c7d2c-126">Request body</span></span>

<span data-ttu-id="c7d2c-127">Geben Sie im Textkörper Anforderung eine JSON-Darstellung eines [Team](../resources/team.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c7d2c-127">In the request body, supply a JSON representation of a [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c7d2c-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="c7d2c-128">Response</span></span>

<span data-ttu-id="c7d2c-129">Wenn diese Methode erfolgreich ist, zurückgeben soll eine `201 Created` Antwortcode und ein [Team](../resources/team.md) -Objekt aus der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c7d2c-129">If successful, this method should return a `201 Created` response code and a [team](../resources/team.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7d2c-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c7d2c-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c7d2c-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c7d2c-131">Request</span></span>

<span data-ttu-id="c7d2c-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c7d2c-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_team"
}-->
```http
PUT https://graph.microsoft.com/v1.0/groups/{id}/team
Content-type: application/json

{  
  "memberSettings": {
    "allowCreateUpdateChannels": true
  },
  "messagingSettings": {
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true
  },
  "funSettings": {
    "allowGiphy": true,
    "giphyContentRating": "strict"
  }
}
```

#### <a name="response"></a><span data-ttu-id="c7d2c-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="c7d2c-133">Response</span></span>

<span data-ttu-id="c7d2c-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c7d2c-134">The following is an example of the response.</span></span> 

><span data-ttu-id="c7d2c-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="c7d2c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 401

{
  "memberSettings": {
    "allowCreateUpdateChannels": true,
    "allowDeleteChannels": true,
    "allowAddRemoveApps": true,
    "allowCreateUpdateRemoveTabs": true,
    "allowCreateUpdateRemoveConnectors": true    
  },
  "guestSettings": {
    "allowCreateUpdateChannels": true,
    "allowDeleteChannels": true 
  },
  "messagingSettings": {
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true,
    "allowOwnerDeleteMessages": true,
    "allowTeamMentions": true,
    "allowChannelMentions": true    
  },
  "funSettings": {
    "allowGiphy": true,
    "giphyContentRating": "strict",
    "allowStickersAndMemes": true,
    "allowCustomMemes": true
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a><span data-ttu-id="c7d2c-137">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="c7d2c-137">See also</span></span>

- [<span data-ttu-id="c7d2c-138">Erstellen einer Gruppe mit einem team</span><span class="sxs-lookup"><span data-stu-id="c7d2c-138">Creating a group with a team</span></span>](../../../concepts/teams-create-group-and-team.md)
