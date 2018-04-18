# <a name="permanently-delete-item"></a><span data-ttu-id="f5fba-101">Element endgültig löschen</span><span class="sxs-lookup"><span data-stu-id="f5fba-101">Permanently delete item</span></span>

<span data-ttu-id="f5fba-102">Dauerhaftes Löschen eines Elements aus dem Ordner [Gelöschte Elemente](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="f5fba-102">Permanently deletes an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="f5fba-103">Die Funktion für gelöschte Elemente wird derzeit nur für die Ressourcen [group](../resources/group.md) und [user](../resources/user.md) unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f5fba-103">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="f5fba-104">Sie können ein Element aus den gelöschten Elementen dauerhaft löschen.</span><span class="sxs-lookup"><span data-stu-id="f5fba-104">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="f5fba-105">Aber nachdem ein Element dauerhaft gelöscht wurde, **kann es nicht** wiederhergestellt werden.</span><span class="sxs-lookup"><span data-stu-id="f5fba-105">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5fba-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f5fba-106">Permissions</span></span>
<span data-ttu-id="f5fba-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f5fba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

### <a name="for-users"></a><span data-ttu-id="f5fba-109">Für Benutzer:</span><span class="sxs-lookup"><span data-stu-id="f5fba-109">For users:</span></span>

|<span data-ttu-id="f5fba-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f5fba-110">Permission type</span></span>      | <span data-ttu-id="f5fba-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f5fba-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5fba-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f5fba-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f5fba-113">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f5fba-113">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="f5fba-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f5fba-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5fba-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f5fba-115">Not supported.</span></span> |
|<span data-ttu-id="f5fba-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f5fba-116">Application</span></span> | <span data-ttu-id="f5fba-117">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5fba-117">User.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="f5fba-118">Für Gruppen:</span><span class="sxs-lookup"><span data-stu-id="f5fba-118">For groups:</span></span>

|<span data-ttu-id="f5fba-119">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f5fba-119">Permission type</span></span>      | <span data-ttu-id="f5fba-120">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f5fba-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5fba-121">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f5fba-121">Delegated (work or school account)</span></span> | <span data-ttu-id="f5fba-122">Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f5fba-122">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="f5fba-123">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f5fba-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5fba-124">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f5fba-124">Not supported.</span></span>    |
|<span data-ttu-id="f5fba-125">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f5fba-125">Application</span></span> | <span data-ttu-id="f5fba-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5fba-126">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5fba-127">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f5fba-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deleteditems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f5fba-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f5fba-128">Request headers</span></span>
| <span data-ttu-id="f5fba-129">Name</span><span class="sxs-lookup"><span data-stu-id="f5fba-129">Name</span></span>       | <span data-ttu-id="f5fba-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f5fba-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f5fba-131">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="f5fba-131">Authorization</span></span>  | <span data-ttu-id="f5fba-132">Bearer&lt;code&gt; *erforderlich*</span><span class="sxs-lookup"><span data-stu-id="f5fba-132">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="f5fba-133">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f5fba-133">Accept</span></span>  | <span data-ttu-id="f5fba-134">application/json</span><span class="sxs-lookup"><span data-stu-id="f5fba-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f5fba-135">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f5fba-135">Request body</span></span>
<span data-ttu-id="f5fba-136">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f5fba-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5fba-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="f5fba-137">Response</span></span>

<span data-ttu-id="f5fba-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f5fba-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5fba-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f5fba-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f5fba-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f5fba-141">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
##### <a name="response"></a><span data-ttu-id="f5fba-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="f5fba-142">Response</span></span>
<span data-ttu-id="f5fba-p104">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f5fba-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->