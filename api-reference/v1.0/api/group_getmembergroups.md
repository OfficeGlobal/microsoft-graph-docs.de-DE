# <a name="group-getmembergroups"></a><span data-ttu-id="cb07a-101">group: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="cb07a-101">group: getMemberGroups</span></span>

<span data-ttu-id="cb07a-p101">Gibt alle Gruppen zurück, bei denen die Gruppe Mitglied ist von. Die Überprüfung ist transitiv; im Gegensatz zum Lesen der Navigationseigenschaft [Mitglied](../api/group_list_memberof.md), die nur die Gruppen zurückgibt, deren direktes Mitglied die Gruppe ist.</span><span class="sxs-lookup"><span data-stu-id="cb07a-p101">Return all the groups that the specified group is a member of. The check is transitive, unlike reading the [memberOf](../api/group_list_memberof.md) navigation property, which returns only the groups that the group is a direct member of.</span></span>

<span data-ttu-id="cb07a-p102">Diese Funktion unterstützt Office 365 und andere Typen von Gruppen, die in Azure AD bereitgestellt werden. Die maximale Anzahl von Gruppen, die jede Anfrage zurückgeben kann, ist 2046. Beachten Sie, dass Office 365-Gruppen keine Gruppen enthalten können. Die Mitgliedschaft in einer Office 365-Gruppe ist also immer direkt.</span><span class="sxs-lookup"><span data-stu-id="cb07a-p102">This function supports Office 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb07a-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cb07a-108">Permissions</span></span>

<span data-ttu-id="cb07a-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cb07a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="cb07a-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cb07a-111">Permission type</span></span>                        | <span data-ttu-id="cb07a-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cb07a-112">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="cb07a-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cb07a-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="cb07a-114">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cb07a-114">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="cb07a-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cb07a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb07a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cb07a-116">Not supported.</span></span>                                                                              |
| <span data-ttu-id="cb07a-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cb07a-117">Application</span></span>                            | <span data-ttu-id="cb07a-118">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb07a-118">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

> <span data-ttu-id="cb07a-119">**Hinweis:** Diese API erfordert derzeit die Berechtigung `Directory.Read.All` oder höher.</span><span class="sxs-lookup"><span data-stu-id="cb07a-119">Note: This API currently requires the Directory.Read.All permission or higher.</span></span> <span data-ttu-id="cb07a-120">Bei der Berechtigung `Group.Read.All` wird ein Fehler ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="cb07a-120">Using the Group.Read.All permission will return an error.</span></span> <span data-ttu-id="cb07a-121">Dies ist ein bekanntes Problem.</span><span class="sxs-lookup"><span data-stu-id="cb07a-121">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="cb07a-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cb07a-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/getMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="cb07a-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cb07a-123">Request headers</span></span>

| <span data-ttu-id="cb07a-124">Name</span><span class="sxs-lookup"><span data-stu-id="cb07a-124">Name</span></span>          | <span data-ttu-id="cb07a-125">Typ</span><span class="sxs-lookup"><span data-stu-id="cb07a-125">Type</span></span>   | <span data-ttu-id="cb07a-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cb07a-126">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="cb07a-127">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="cb07a-127">Authorization</span></span> | <span data-ttu-id="cb07a-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cb07a-128">string</span></span> | <span data-ttu-id="cb07a-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cb07a-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cb07a-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cb07a-131">Request body</span></span>

<span data-ttu-id="cb07a-132">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="cb07a-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cb07a-133">Parameter</span><span class="sxs-lookup"><span data-stu-id="cb07a-133">Parameter</span></span>           | <span data-ttu-id="cb07a-134">Typ</span><span class="sxs-lookup"><span data-stu-id="cb07a-134">Type</span></span>    | <span data-ttu-id="cb07a-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cb07a-135">Description</span></span>                                                                           |
| :------------------ | :------ | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="cb07a-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="cb07a-136">securityEnabledOnly</span></span> | <span data-ttu-id="cb07a-137">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cb07a-137">Boolean</span></span> | <span data-ttu-id="cb07a-p106">Festgelegt auf **false**. Die Option, dass nur Gruppen mit aktivierter Sicherheit zurückgegeben werden, wird nur für Benutzer unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cb07a-p106">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span> |

## <a name="response"></a><span data-ttu-id="cb07a-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="cb07a-140">Response</span></span>

<span data-ttu-id="cb07a-141">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Zeichenfolgensammlung im Antworttext zurückgegeben, der die IDs der Gruppen enthält, von denen die Gruppe ein Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="cb07a-141">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="cb07a-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cb07a-142">Example</span></span>

#### <a name="request"></a><span data-ttu-id="cb07a-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cb07a-143">Request</span></span>

<span data-ttu-id="cb07a-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cb07a-144">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "group_getmembergroups"
}-->

```http
POST https://graph.microsoft.com/v1.0/groups/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```

#### <a name="response"></a><span data-ttu-id="cb07a-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="cb07a-145">Response</span></span>

<span data-ttu-id="cb07a-146">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cb07a-146">The following is an example of the response.</span></span>

> <span data-ttu-id="cb07a-p107">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="cb07a-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "group: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
