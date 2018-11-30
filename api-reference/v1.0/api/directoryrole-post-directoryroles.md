---
title: directoryRole aktivieren
description: Dient zum Aktivieren einer Verzeichnisrolle. Um eine Verzeichnisrolle zu lesen oder ihre Mitglieder zu aktualisieren, muss diese zuerst im Mandanten aktiviert werden. Nur die Unternehmensadministratoren und die impliziten Benutzerverzeichnisrollen sind standardmäßig aktiviert. Um auf Mitglieder zuzugreifen und diese einer anderen Verzeichnisrolle zuzuweisen, müssen Sie diese zuerst mit der entsprechenden Verzeichnisrollenvorlage aktivieren (directoryRoleTemplate).
ms.openlocfilehash: 2d2f51aab33520c95bda88eab8f98af12af36083
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018998"
---
# <a name="activate-directoryrole"></a><span data-ttu-id="388f8-106">directoryRole aktivieren</span><span class="sxs-lookup"><span data-stu-id="388f8-106">Activate directoryRole</span></span>

<span data-ttu-id="388f8-p102">Dient zum Aktivieren einer Verzeichnisrolle. Um eine Verzeichnisrolle zu lesen oder ihre Mitglieder zu aktualisieren, muss diese zuerst im Mandanten aktiviert werden. Nur die Unternehmensadministratoren und die impliziten Benutzerverzeichnisrollen sind standardmäßig aktiviert. Um auf Mitglieder zuzugreifen und diese einer anderen Verzeichnisrolle zuzuweisen, müssen Sie diese zuerst mit der entsprechenden Verzeichnisrollenvorlage aktivieren ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="388f8-p102">Activate a directory role. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators and the implicit Users directory roles are activated by default. To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="388f8-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="388f8-111">Permissions</span></span>
<span data-ttu-id="388f8-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="388f8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="388f8-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="388f8-114">Permission type</span></span>      | <span data-ttu-id="388f8-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="388f8-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="388f8-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="388f8-116">Delegated (work or school account)</span></span> | <span data-ttu-id="388f8-117">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="388f8-117">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="388f8-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="388f8-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="388f8-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="388f8-119">Not supported.</span></span>    |
|<span data-ttu-id="388f8-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="388f8-120">Application</span></span> | <span data-ttu-id="388f8-121">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="388f8-121">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="388f8-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="388f8-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="388f8-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="388f8-123">Request headers</span></span>
| <span data-ttu-id="388f8-124">Name</span><span class="sxs-lookup"><span data-stu-id="388f8-124">Name</span></span>       | <span data-ttu-id="388f8-125">Typ</span><span class="sxs-lookup"><span data-stu-id="388f8-125">Type</span></span> | <span data-ttu-id="388f8-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="388f8-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="388f8-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="388f8-127">Authorization</span></span>  | <span data-ttu-id="388f8-128">string</span><span class="sxs-lookup"><span data-stu-id="388f8-128">string</span></span>  | <span data-ttu-id="388f8-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="388f8-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="388f8-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="388f8-131">Content-Type</span></span>  | <span data-ttu-id="388f8-132">string</span><span class="sxs-lookup"><span data-stu-id="388f8-132">string</span></span>  | <span data-ttu-id="388f8-133">application/json</span><span class="sxs-lookup"><span data-stu-id="388f8-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="388f8-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="388f8-134">Request body</span></span>
<span data-ttu-id="388f8-135">Geben Sie im Anforderungstext eine JSON-Darstellung des [directoryRole](../resources/directoryrole.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="388f8-135">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="388f8-136">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Aktivieren einer Verzeichnisrolle erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="388f8-136">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="388f8-137">Parameter</span><span class="sxs-lookup"><span data-stu-id="388f8-137">Parameter</span></span> | <span data-ttu-id="388f8-138">Typ</span><span class="sxs-lookup"><span data-stu-id="388f8-138">Type</span></span> | <span data-ttu-id="388f8-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="388f8-139">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="388f8-140">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="388f8-140">roleTemplateId</span></span> | <span data-ttu-id="388f8-141">string</span><span class="sxs-lookup"><span data-stu-id="388f8-141">string</span></span> | <span data-ttu-id="388f8-142">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="388f8-142">Required.</span></span> <span data-ttu-id="388f8-143">Die ID des der [DirectoryRoleTemplate](../resources/directoryroletemplate.md) , die die Rolle basiert.</span><span class="sxs-lookup"><span data-stu-id="388f8-143">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on.</span></span> <span data-ttu-id="388f8-144">Dies ist die einzige Eigenschaft, die in der Anforderung angegeben werden können.</span><span class="sxs-lookup"><span data-stu-id="388f8-144">This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="388f8-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="388f8-145">Response</span></span>

<span data-ttu-id="388f8-146">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [directoryRole](../resources/directoryrole.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="388f8-146">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="388f8-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="388f8-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="388f8-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="388f8-148">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryrole_from_directoryroles"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles
Content-type: application/json

{
  "roleTemplateId": "roleTemplateId-value"
}
```
<span data-ttu-id="388f8-149">Geben Sie im Anforderungstext eine JSON-Darstellung des [directoryRole](../resources/directoryrole.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="388f8-149">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="388f8-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="388f8-150">Response</span></span>
<span data-ttu-id="388f8-p106">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="388f8-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "description": "description-value",
  "displayName": "displayName-value",
  "roleTemplateId": "roleTemplateId-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->