# <a name="list-deleted-items-owned-by-a-user"></a><span data-ttu-id="b1e11-101">**Gelöschte Listenelemente im Besitz eines Benutzers**</span><span class="sxs-lookup"><span data-stu-id="b1e11-101">Added **List deleted items owned by a user** action to directory (deleted items) resource</span></span>

<span data-ttu-id="b1e11-102">Durchsucht eine Liste kürzlich gelöschter Objekte in Besitz des angegebenen Benutzers.</span><span class="sxs-lookup"><span data-stu-id="b1e11-102">Retrieves a list of recently deleted items owned by the specified user.</span></span>  

<span data-ttu-id="b1e11-103">Zurzeit wird die Funktion der Liste gelöschter Elemente nur für [Gruppen-](../resources/group.md)Ressourcen im Besitz des Benutzers unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b1e11-103">Currently, list deleted items functionality is supported only for [group](../resources/group.md) resources owned by the user.</span></span>

<span data-ttu-id="b1e11-104">Dies ist eine Dienst-Aktion, was bedeutet, dass sie keine Paginierung unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b1e11-104">This is a service action, which means it does not support pagination.</span></span>  <span data-ttu-id="b1e11-105">Die API gibt bis zu 1.000 Gelöschte Objekte im Besitz des Benutzers, sortiert nach ID zurück.</span><span class="sxs-lookup"><span data-stu-id="b1e11-105">The API returns up to 1,000 deleted objects owned by the user, sorted by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1e11-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b1e11-106">Permissions</span></span>

<span data-ttu-id="b1e11-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](https://developer.microsoft.com/en-us/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="b1e11-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/en-us/graph/docs/concepts/permissions_reference).</span></span>

| <span data-ttu-id="b1e11-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b1e11-109">Permission type</span></span> | <span data-ttu-id="b1e11-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b1e11-110">Permissions (from least to most privileged)</span></span> |
| --- | --- |
| <span data-ttu-id="b1e11-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b1e11-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b1e11-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1e11-112">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="b1e11-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b1e11-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b1e11-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b1e11-114">Not supported.</span></span> |
| <span data-ttu-id="b1e11-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b1e11-115">Application</span></span> | <span data-ttu-id="b1e11-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1e11-116">Group.Read.All, Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="b1e11-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b1e11-117">HTTP request</span></span>

``` http
POST /directory/deletedItems/getUserOwnedObjects
```

## <a name="request-headers"></a><span data-ttu-id="b1e11-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b1e11-118">Request headers</span></span>

| <span data-ttu-id="b1e11-119">Name</span><span class="sxs-lookup"><span data-stu-id="b1e11-119">Name</span></span>          | <span data-ttu-id="b1e11-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b1e11-120">Description</span></span>               |
| ------------- | ------------------------- |
| <span data-ttu-id="b1e11-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="b1e11-121">Authorization</span></span> | <span data-ttu-id="b1e11-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b1e11-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b1e11-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b1e11-124">Request body</span></span>

```json
{
  "userId":"{id}",
  "type":"Group"
}
```

<span data-ttu-id="b1e11-125">Der Textkörper der Anforderung erfordert die folgenden Parameter:</span><span class="sxs-lookup"><span data-stu-id="b1e11-125">The request body requires the following parameters:</span></span>

| <span data-ttu-id="b1e11-126">Parameter</span><span class="sxs-lookup"><span data-stu-id="b1e11-126">Parameter</span></span>    | <span data-ttu-id="b1e11-127">Typ</span><span class="sxs-lookup"><span data-stu-id="b1e11-127">Type</span></span> |<span data-ttu-id="b1e11-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b1e11-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b1e11-129">userId</span><span class="sxs-lookup"><span data-stu-id="b1e11-129">userId</span></span>|<span data-ttu-id="b1e11-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b1e11-130">String</span></span>|<span data-ttu-id="b1e11-131">ID des Eigentümers.</span><span class="sxs-lookup"><span data-stu-id="b1e11-131">ID of the owner.</span></span>|
|<span data-ttu-id="b1e11-132">Typ</span><span class="sxs-lookup"><span data-stu-id="b1e11-132">type</span></span>|<span data-ttu-id="b1e11-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b1e11-133">String</span></span>|<span data-ttu-id="b1e11-134">Bei der Art der zurückzugebenden Objekte ist `Group` derzeit der einzige unterstützte Wert.</span><span class="sxs-lookup"><span data-stu-id="b1e11-134">Type of owned objects to return; `Group` is currently the only supported value.</span></span>|


## <a name="response"></a><span data-ttu-id="b1e11-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="b1e11-135">Response</span></span>

<span data-ttu-id="b1e11-136">Erfolgreiche Anforderungen geben `200 OK` Antwortcodes zurück; das Antwort-Objekt enthält die Eigenschaften des [Verzeichnisses (Gelöschte Objekte)](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="b1e11-136">Successful requests return `200 OK` response codes; the response object includes [directory (deleted items)](../resources/directory.md) properties.</span></span>

## <a name="example"></a><span data-ttu-id="b1e11-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b1e11-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b1e11-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b1e11-138">Request</span></span>

<span data-ttu-id="b1e11-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b1e11-139">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/directory/deletedItems/getUserOwnedObjects
Content-type: application/json
```

``` json
{
  "userId":"55ac777c-109e-4022-b58c-470c8fcb6892",
  "type":"group"
}
```

###### <a name="response"></a><span data-ttu-id="b1e11-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="b1e11-140">Response</span></span>

<span data-ttu-id="b1e11-141">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b1e11-141">Here is an example of the response.</span></span> <span data-ttu-id="b1e11-142">Hinweis: Dieses Antwortobjekt kann der Kürze halber möglicherweise abgeschnitten werden.</span><span class="sxs-lookup"><span data-stu-id="b1e11-142">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b1e11-143">Alle unterstützte Eigenschaften werden von tatsächlichen Anrufen zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b1e11-143">All supported properties are returned from actual calls.</span></span>

``` http
HTTP/1.1 200
Content-type: application/json
Content-length: 1249

{
"value": [
          {
              "@odata.type": "#microsoft.graph.group",
              "id": "bfa7033a-7367-4644-85f5-95aaf385cbd7",
              "deletedDateTime": 2018-04-01T12:39:16Z,
              "classification": null,
              "createdDateTime": "2017-03-22T12:39:16Z",
              "description": null,
              "displayName": "Test",
              "groupTypes": [
                  "Unified"
              ],
              "mail": "Test@contoso.com",
              "mailEnabled": true,
              "mailNickname": "Test",
              "membershipRule": null,
              "membershipRuleProcessingState": null,
              "preferredDataLocation": null,
              "preferredLanguage": null,
              "proxyAddresses": [
                  "SMTP:Test@contoso.com"
              ],
              "renewedDateTime": "2017-09-22T22:30:39Z",
              "securityEnabled": false,
              "theme": null,
              "visibility": "Public"
          } 
        ]
 }
```


