# <a name="update-grouplifecyclepolicy"></a><span data-ttu-id="622fd-101">Aktualisieren von groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="622fd-101">Update groupLifecyclePolicy</span></span>

<span data-ttu-id="622fd-102">Aktualisieren Sie die Eigenschaften eines groupLifecyclePolicy[groupLifecyclePolicy-Ressourcentyp](../resources/grouplifecyclepolicy.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="622fd-102">Update the properties of a groupLifecyclePolicy[groupLifecyclePolicy resource type](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="622fd-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="622fd-103">Permissions</span></span>

<span data-ttu-id="622fd-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="622fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>
 
|<span data-ttu-id="622fd-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="622fd-106">Permission type</span></span>      | <span data-ttu-id="622fd-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="622fd-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="622fd-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="622fd-108">Delegated (work or school account)</span></span> | <span data-ttu-id="622fd-109">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="622fd-109">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="622fd-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="622fd-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="622fd-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="622fd-111">Not supported.</span></span>    |
|<span data-ttu-id="622fd-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="622fd-112">Application</span></span> | <span data-ttu-id="622fd-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="622fd-113">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="622fd-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="622fd-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groupLifecyclePolicies/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="622fd-115">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="622fd-115">Optional request headers</span></span>
| <span data-ttu-id="622fd-116">Name</span><span class="sxs-lookup"><span data-stu-id="622fd-116">Name</span></span> | <span data-ttu-id="622fd-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="622fd-117">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="622fd-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="622fd-118">Authorization</span></span> | <span data-ttu-id="622fd-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="622fd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="622fd-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="622fd-121">Content-Type</span></span>  | <span data-ttu-id="622fd-122">application/json</span><span class="sxs-lookup"><span data-stu-id="622fd-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="622fd-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="622fd-123">Request body</span></span>

<span data-ttu-id="622fd-124">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="622fd-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="622fd-125">Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="622fd-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="622fd-126">Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="622fd-126">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="622fd-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="622fd-127">Property</span></span> | <span data-ttu-id="622fd-128">Typ</span><span class="sxs-lookup"><span data-stu-id="622fd-128">Type</span></span> | <span data-ttu-id="622fd-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="622fd-129">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="622fd-130">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="622fd-130">alternateNotificationEmails</span></span>|<span data-ttu-id="622fd-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="622fd-131">String</span></span>| <span data-ttu-id="622fd-132">Liste der E-Mail-Adressen, an die Benachrichtigungen für Gruppen ohne Besitzer gesendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="622fd-132">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="622fd-133">Mehrere E-Mail-Adressen können durch ein Semikolon voneinander getrennt definiert werden.</span><span class="sxs-lookup"><span data-stu-id="622fd-133">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="622fd-134">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="622fd-134">groupLifetimeInDays</span></span>|<span data-ttu-id="622fd-135">Int32</span><span class="sxs-lookup"><span data-stu-id="622fd-135">Int32</span></span>| <span data-ttu-id="622fd-136">Anzahl von Tagen, bis eine Gruppe abläuft und verlängert werden muss.</span><span class="sxs-lookup"><span data-stu-id="622fd-136">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="622fd-137">Sobald die Gruppe verlängert wurde, wird der Ablaufzeitraum für die Gruppe um die Anzahl der definierten Tage verlängert.</span><span class="sxs-lookup"><span data-stu-id="622fd-137">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="622fd-138">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="622fd-138">managedGroupTypes</span></span>|<span data-ttu-id="622fd-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="622fd-139">String</span></span>| <span data-ttu-id="622fd-140">Der Gruppentyp, für den die Ablaufrichtlinie gilt.</span><span class="sxs-lookup"><span data-stu-id="622fd-140">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="622fd-141">Mögliche Werte sind **Alle**, **Ausgewählte** oder **Keine**.</span><span class="sxs-lookup"><span data-stu-id="622fd-141">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="response"></a><span data-ttu-id="622fd-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="622fd-142">Response</span></span>

<span data-ttu-id="622fd-143">Wenn erfolgreich ausgeführt, gibt diese Methode den Antwortcode `200 OK` und ein aktualisiertes [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="622fd-143">If successful, this method returns a `200 OK` response code and updated [Chart](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="622fd-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="622fd-144">Example</span></span>

##### <a name="request"></a><span data-ttu-id="622fd-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="622fd-145">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_grouplifecyclepolicy"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}
Content-type: application/json
Content-length: 125

{
  "groupLifetimeInDays": 180,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
##### <a name="response"></a><span data-ttu-id="622fd-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="622fd-146">Response</span></span>
<span data-ttu-id="622fd-147">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="622fd-147">Note: The response object shown here may be truncated for brevity.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 146

{
  "id": "id-value",
  "groupLifetimeInDays": 180,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->