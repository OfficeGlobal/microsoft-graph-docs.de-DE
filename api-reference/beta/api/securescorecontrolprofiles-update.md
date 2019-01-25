---
title: Update secureScoreControlProfiles
description: Aktualisieren einer bearbeitbaren SecureScoreControlProfiles-Eigenschaft in eine integrierte Lösung verschiedene Eigenschaften, wie AssignedTo oder TenantNote ändern.
localization_priority: Normal
ms.openlocfilehash: 711fd29e906822def0a5f4b5fbca13a1d73732d6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510953"
---
# <a name="update-securescorecontrolprofiles"></a><span data-ttu-id="39f29-103">Update secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="39f29-103">Update secureScoreControlProfiles</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39f29-104">Aktualisieren einer bearbeitbaren **SecureScoreControlProfiles** -Eigenschaft in eine integrierte Lösung verschiedene Eigenschaften, wie **AssignedTo** oder **TenantNote**ändern.</span><span class="sxs-lookup"><span data-stu-id="39f29-104">Update an editable **secureScoreControlProfiles** property within any integrated solution to change various properties, such as **assignedTo** or **tenantNote**.</span></span>

## <a name="permissions"></a><span data-ttu-id="39f29-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="39f29-105">Permissions</span></span>

<span data-ttu-id="39f29-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39f29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39f29-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="39f29-108">Permission type</span></span>      | <span data-ttu-id="39f29-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="39f29-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="39f29-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="39f29-110">Delegated (work or school account)</span></span> |   <span data-ttu-id="39f29-111">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39f29-111">SecurityEvents.ReadWrite.All.</span></span>  |
|<span data-ttu-id="39f29-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="39f29-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="39f29-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="39f29-113">Not supported.</span></span>  |
|<span data-ttu-id="39f29-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="39f29-114">Application</span></span> | <span data-ttu-id="39f29-115">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39f29-115">SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="39f29-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="39f29-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/secureScoreControlProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="39f29-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="39f29-117">Request headers</span></span>

| <span data-ttu-id="39f29-118">Name</span><span class="sxs-lookup"><span data-stu-id="39f29-118">Name</span></span>       | <span data-ttu-id="39f29-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="39f29-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="39f29-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="39f29-120">Authorization</span></span>  | <span data-ttu-id="39f29-p102">Bearer {code}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="39f29-p102">Bearer {code}. Required.</span></span>|
|<span data-ttu-id="39f29-123">Prefer</span><span class="sxs-lookup"><span data-stu-id="39f29-123">Prefer</span></span> | <span data-ttu-id="39f29-124">zurückgeben = Darstellung.</span><span class="sxs-lookup"><span data-stu-id="39f29-124">return=representation.</span></span> |

## <a name="request-body"></a><span data-ttu-id="39f29-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="39f29-125">Request body</span></span>

<span data-ttu-id="39f29-126">Geben Sie im Textkörper Anforderung eine JSON-Darstellung der Werte für die entsprechenden Felder, die aktualisiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="39f29-126">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="39f29-127">In der folgenden Tabelle werden die Felder, die für eine SecureScoreControlProfile aktualisiert werden können.</span><span class="sxs-lookup"><span data-stu-id="39f29-127">The following table lists the fields that can be updated for a secureScoreControlProfile.</span></span> <span data-ttu-id="39f29-128">Die Werte für vorhandene Eigenschaften, die nicht im Textkörper Anforderung enthalten sind, werden nicht geändert.</span><span class="sxs-lookup"><span data-stu-id="39f29-128">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="39f29-129">Geben Sie aus Gründen der Leistung vorhandene Werte, die nicht geändert wurden, nicht an.</span><span class="sxs-lookup"><span data-stu-id="39f29-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="39f29-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="39f29-130">Property</span></span>   | <span data-ttu-id="39f29-131">Typ</span><span class="sxs-lookup"><span data-stu-id="39f29-131">Type</span></span> |<span data-ttu-id="39f29-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="39f29-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="39f29-133">assignedTo</span><span class="sxs-lookup"><span data-stu-id="39f29-133">assignedTo</span></span>|<span data-ttu-id="39f29-134">String</span><span class="sxs-lookup"><span data-stu-id="39f29-134">String</span></span>|<span data-ttu-id="39f29-135">Name des der Analyst das Steuerelement wird für die Ursachenanalyse, Implementierung und-Wartung zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="39f29-135">Name of the analyst the control is assigned to for triage, implementation, or remediation.</span></span>|
|<span data-ttu-id="39f29-136">tenantNote</span><span class="sxs-lookup"><span data-stu-id="39f29-136">tenantNote</span></span>|<span data-ttu-id="39f29-137">String</span><span class="sxs-lookup"><span data-stu-id="39f29-137">String</span></span>|<span data-ttu-id="39f29-138">Analyst von Kommentaren auf das Steuerelement (für Kunden Steuerelement Management).</span><span class="sxs-lookup"><span data-stu-id="39f29-138">Analyst comments on the control (for customer control management).</span></span>|
|<span data-ttu-id="39f29-139">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="39f29-139">controlStateUpdates</span></span>| <span data-ttu-id="39f29-140">String</span><span class="sxs-lookup"><span data-stu-id="39f29-140">String</span></span>|<span data-ttu-id="39f29-141">Analyst gesteuerte Einstellung für das Steuerelement.</span><span class="sxs-lookup"><span data-stu-id="39f29-141">Analyst driven setting on the control.</span></span> <span data-ttu-id="39f29-142">Mögliche Werte sind: `ignore`, `thirdParty` und `reviewed`.</span><span class="sxs-lookup"><span data-stu-id="39f29-142">Possible values are: `ignore`, `thirdParty`, `reviewed`.</span></span>|


## <a name="response"></a><span data-ttu-id="39f29-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="39f29-143">Response</span></span>

<span data-ttu-id="39f29-144">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="39f29-144">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="39f29-145">Wenn der optionale Anforderungsheader verwendet wird, gibt die Methode eine `200 OK` Antwortcode und der aktualisierten [SecureScoreControlProfiles](../resources/securescorecontrolprofiles.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="39f29-145">If the optional request header is used, the method returns a `200 OK` response code and the updated [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39f29-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="39f29-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="39f29-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="39f29-147">Request</span></span>

<span data-ttu-id="39f29-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="39f29-148">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_update"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/secureScoreControlProfiles/AdminMFA
Content-type: application/json

{
  "assignedTo": "assignedTo-value",
  "controlStateUpdates": "controlStateUpdates-value",
  "tenantNote": "tenantNote-value"
}
```

### <a name="response"></a><span data-ttu-id="39f29-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="39f29-149">Response</span></span>

<span data-ttu-id="39f29-150">Es folgt ein Beispiel für eine erfolgreiche Antwort.</span><span class="sxs-lookup"><span data-stu-id="39f29-150">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfiles"
} -->

```http
HTTP/1.1 204 No Content
```




<!--
{
  "type": "#page.annotation",
  "description": "Update secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/securescorecontrolprofiles-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
