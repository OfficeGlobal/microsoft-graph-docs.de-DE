# <a name="update-organization"></a><span data-ttu-id="b4ef9-101">Organisation aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b4ef9-101">Update organization</span></span>

<span data-ttu-id="b4ef9-102">Mit dieser API können Sie die Eigenschaften der aktuell authentifizierten Organisation aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="b4ef9-102">Update the properties of the currently authenticated organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4ef9-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b4ef9-103">Permissions</span></span>

<span data-ttu-id="b4ef9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b4ef9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b4ef9-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b4ef9-106">Permission type</span></span> | <span data-ttu-id="b4ef9-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b4ef9-107">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4ef9-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b4ef9-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b4ef9-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b4ef9-109">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b4ef9-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b4ef9-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4ef9-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b4ef9-111">Not supported.</span></span>    |
|<span data-ttu-id="b4ef9-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b4ef9-112">Application</span></span> | <span data-ttu-id="b4ef9-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b4ef9-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4ef9-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b4ef9-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization

```

## <a name="request-headers"></a><span data-ttu-id="b4ef9-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b4ef9-115">Request headers</span></span>

| <span data-ttu-id="b4ef9-116">Name</span><span class="sxs-lookup"><span data-stu-id="b4ef9-116">Name</span></span>       | <span data-ttu-id="b4ef9-117">Typ</span><span class="sxs-lookup"><span data-stu-id="b4ef9-117">Type</span></span> | <span data-ttu-id="b4ef9-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b4ef9-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b4ef9-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4ef9-119">Authorization</span></span>  | <span data-ttu-id="b4ef9-120">string</span><span class="sxs-lookup"><span data-stu-id="b4ef9-120">string</span></span>  | <span data-ttu-id="b4ef9-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b4ef9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b4ef9-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b4ef9-123">Request body</span></span>
<span data-ttu-id="b4ef9-124">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="b4ef9-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="b4ef9-125">Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="b4ef9-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="b4ef9-126">Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="b4ef9-126">For best performance, you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b4ef9-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b4ef9-127">Property</span></span>     | <span data-ttu-id="b4ef9-128">Typ</span><span class="sxs-lookup"><span data-stu-id="b4ef9-128">Type</span></span>   |<span data-ttu-id="b4ef9-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b4ef9-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b4ef9-130">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="b4ef9-130">marketingNotificationEmails</span></span>|<span data-ttu-id="b4ef9-131">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="b4ef9-131">String collection</span></span>|                                        <span data-ttu-id="b4ef9-132">**Hinweis:** Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="b4ef9-132">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="b4ef9-133">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="b4ef9-133">privacyProfile</span></span>|[<span data-ttu-id="b4ef9-134">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="b4ef9-134">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="b4ef9-135">Das Datenschutzprofil einer Organisation ( „statementUrl“ und „contactEmail“ festlegen).</span><span class="sxs-lookup"><span data-stu-id="b4ef9-135">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="b4ef9-136">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="b4ef9-136">securityComplianceNotificationMails</span></span>|<span data-ttu-id="b4ef9-137">String collection</span><span class="sxs-lookup"><span data-stu-id="b4ef9-137">String collection</span></span>||
|<span data-ttu-id="b4ef9-138">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="b4ef9-138">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="b4ef9-139">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="b4ef9-139">String collection</span></span>||
|<span data-ttu-id="b4ef9-140">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="b4ef9-140">technicalNotificationMails</span></span>|<span data-ttu-id="b4ef9-141">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="b4ef9-141">String collection</span></span>|                                        <span data-ttu-id="b4ef9-142">**Hinweis:** Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="b4ef9-142">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="b4ef9-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="b4ef9-143">Response</span></span>

<span data-ttu-id="b4ef9-144">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b4ef9-144">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b4ef9-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b4ef9-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4ef9-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b4ef9-146">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_organization"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization
Content-type: application/json
Content-length: 411

{
  "marketingNotificationEmails" : ["marketing@contoso.com"],
  "privacyProfile" :
    {
      "contactEmail":"alice@contoso.com",
      "statementUrl":"https://contoso.com/privacyStatement"
    },
  "securityComplianceNotificationMails" : ["security@contoso.com"],
  "securityComplianceNotificationPhones" : ["(123) 456-7890"],
  "technicalNotificationMails" : ["tech@contoso.com"]
}
```

### <a name="response"></a><span data-ttu-id="b4ef9-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="b4ef9-147">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
