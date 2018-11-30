---
title: SecureScoreControlProfiles aktualisieren
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
ms.openlocfilehash: afbfcd1889c55dd53241ff8d796bb3ab492b2acf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058136"
---
# <a name="update-securescorecontrolprofiles"></a><span data-ttu-id="916d1-104">SecureScoreControlProfiles aktualisieren</span><span class="sxs-lookup"><span data-stu-id="916d1-104">Update secureScoreControlProfiles</span></span>

 > <span data-ttu-id="916d1-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="916d1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="916d1-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="916d1-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="916d1-107">Aktualisieren einer bearbeitbaren **SecureScoreControlProfiles** -Eigenschaft in eine integrierte Lösung verschiedene Eigenschaften, wie **AssignedTo** oder **TenantNote**ändern.</span><span class="sxs-lookup"><span data-stu-id="916d1-107">Update an editable **secureScoreControlProfiles** property within any integrated solution to change various properties, such as **assignedTo** or **tenantNote**.</span></span>

## <a name="permissions"></a><span data-ttu-id="916d1-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="916d1-108">Permissions</span></span>

<span data-ttu-id="916d1-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="916d1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="916d1-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="916d1-111">Permission type</span></span>      | <span data-ttu-id="916d1-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="916d1-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="916d1-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="916d1-113">Delegated (work or school account)</span></span> |   <span data-ttu-id="916d1-114">SecurityEvents.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="916d1-114">SecurityEvents.ReadWrite.All.</span></span>  |
|<span data-ttu-id="916d1-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="916d1-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="916d1-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="916d1-116">Not supported.</span></span>  |
|<span data-ttu-id="916d1-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="916d1-117">Application</span></span> | <span data-ttu-id="916d1-118">SecurityEvents.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="916d1-118">SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="916d1-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="916d1-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/secureScoreControlProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="916d1-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="916d1-120">Request headers</span></span>

| <span data-ttu-id="916d1-121">Name</span><span class="sxs-lookup"><span data-stu-id="916d1-121">Name</span></span>       | <span data-ttu-id="916d1-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="916d1-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="916d1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="916d1-123">Authorization</span></span>  | <span data-ttu-id="916d1-p104">Bearer {code}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="916d1-p104">Bearer {code}. Required.</span></span>|
|<span data-ttu-id="916d1-126">Prefer</span><span class="sxs-lookup"><span data-stu-id="916d1-126">Prefer</span></span> | <span data-ttu-id="916d1-127">zurückgeben = Darstellung.</span><span class="sxs-lookup"><span data-stu-id="916d1-127">return=representation.</span></span> |

## <a name="request-body"></a><span data-ttu-id="916d1-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="916d1-128">Request body</span></span>

<span data-ttu-id="916d1-129">Geben Sie im Textkörper Anforderung eine JSON-Darstellung der Werte für die entsprechenden Felder, die aktualisiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="916d1-129">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="916d1-130">In der folgenden Tabelle werden die Felder, die für eine SecureScoreControlProfile aktualisiert werden können.</span><span class="sxs-lookup"><span data-stu-id="916d1-130">The following table lists the fields that can be updated for a secureScoreControlProfile.</span></span> <span data-ttu-id="916d1-131">Die Werte für vorhandene Eigenschaften, die nicht im Textkörper Anforderung enthalten sind, werden nicht geändert.</span><span class="sxs-lookup"><span data-stu-id="916d1-131">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="916d1-132">Geben Sie aus Gründen der Leistung vorhandene Werte, die nicht geändert wurden, nicht an.</span><span class="sxs-lookup"><span data-stu-id="916d1-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="916d1-133">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="916d1-133">Property</span></span>   | <span data-ttu-id="916d1-134">Typ</span><span class="sxs-lookup"><span data-stu-id="916d1-134">Type</span></span> |<span data-ttu-id="916d1-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="916d1-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="916d1-136">assignedTo</span><span class="sxs-lookup"><span data-stu-id="916d1-136">assignedTo</span></span>|<span data-ttu-id="916d1-137">String</span><span class="sxs-lookup"><span data-stu-id="916d1-137">String</span></span>|<span data-ttu-id="916d1-138">Name des der Analyst das Steuerelement wird für die Ursachenanalyse, Implementierung und-Wartung zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="916d1-138">Name of the analyst the control is assigned to for triage, implementation, or remediation.</span></span>|
|<span data-ttu-id="916d1-139">tenantNote</span><span class="sxs-lookup"><span data-stu-id="916d1-139">tenantNote</span></span>|<span data-ttu-id="916d1-140">String</span><span class="sxs-lookup"><span data-stu-id="916d1-140">String</span></span>|<span data-ttu-id="916d1-141">Analyst von Kommentaren auf das Steuerelement (für Kunden Steuerelement Management).</span><span class="sxs-lookup"><span data-stu-id="916d1-141">Analyst comments on the control (for customer control management).</span></span>|
|<span data-ttu-id="916d1-142">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="916d1-142">controlStateUpdates</span></span>| <span data-ttu-id="916d1-143">String</span><span class="sxs-lookup"><span data-stu-id="916d1-143">String</span></span>|<span data-ttu-id="916d1-144">Analyst gesteuerte Einstellung für das Steuerelement.</span><span class="sxs-lookup"><span data-stu-id="916d1-144">Analyst driven setting on the control.</span></span> <span data-ttu-id="916d1-145">Mögliche Werte sind: `ignore`, `thirdParty` und `reviewed`.</span><span class="sxs-lookup"><span data-stu-id="916d1-145">Possible values are: `ignore`, `thirdParty`, `reviewed`.</span></span>|


## <a name="response"></a><span data-ttu-id="916d1-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="916d1-146">Response</span></span>

<span data-ttu-id="916d1-147">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="916d1-147">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="916d1-148">Wenn der optionale Anforderungsheader verwendet wird, gibt die Methode eine `200 OK` Antwortcode und der aktualisierten [SecureScoreControlProfiles](../resources/securescorecontrolprofiles.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="916d1-148">If the optional request header is used, the method returns a `200 OK` response code and the updated [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="916d1-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="916d1-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="916d1-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="916d1-150">Request</span></span>

<span data-ttu-id="916d1-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="916d1-151">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="916d1-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="916d1-152">Response</span></span>

<span data-ttu-id="916d1-153">Es folgt ein Beispiel für eine erfolgreiche Antwort.</span><span class="sxs-lookup"><span data-stu-id="916d1-153">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfiles"
} -->

```http
HTTP/1.1 204 No Content
```




<!-- {
  "type": "#page.annotation",
  "description": "Update secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
