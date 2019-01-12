---
title: directoryRole aktivieren
description: Dient zum Aktivieren einer Verzeichnisrolle. Um eine Verzeichnisrolle zu lesen oder ihre Mitglieder zu aktualisieren, muss diese zuerst im Mandanten aktiviert werden. Nur die Unternehmensadministratoren und die impliziten Benutzerverzeichnisrollen sind standardmäßig aktiviert. Um auf Mitglieder zuzugreifen und diese einer anderen Verzeichnisrolle zuzuweisen, müssen Sie diese zuerst mit der entsprechenden Verzeichnisrollenvorlage aktivieren (directoryRoleTemplate).
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5d127580c0a4851c5a991ccc0646007ddf1298a5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924916"
---
# <a name="activate-directoryrole"></a><span data-ttu-id="194e1-106">directoryRole aktivieren</span><span class="sxs-lookup"><span data-stu-id="194e1-106">Activate directoryRole</span></span>

<span data-ttu-id="194e1-p102">Dient zum Aktivieren einer Verzeichnisrolle. Um eine Verzeichnisrolle zu lesen oder ihre Mitglieder zu aktualisieren, muss diese zuerst im Mandanten aktiviert werden. Nur die Unternehmensadministratoren und die impliziten Benutzerverzeichnisrollen sind standardmäßig aktiviert. Um auf Mitglieder zuzugreifen und diese einer anderen Verzeichnisrolle zuzuweisen, müssen Sie diese zuerst mit der entsprechenden Verzeichnisrollenvorlage aktivieren ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="194e1-p102">Activate a directory role. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators and the implicit Users directory roles are activated by default. To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="194e1-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="194e1-111">Permissions</span></span>
<span data-ttu-id="194e1-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="194e1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="194e1-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="194e1-114">Permission type</span></span>      | <span data-ttu-id="194e1-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="194e1-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="194e1-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="194e1-116">Delegated (work or school account)</span></span> | <span data-ttu-id="194e1-117">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="194e1-117">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="194e1-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="194e1-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="194e1-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="194e1-119">Not supported.</span></span>    |
|<span data-ttu-id="194e1-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="194e1-120">Application</span></span> | <span data-ttu-id="194e1-121">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="194e1-121">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="194e1-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="194e1-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="194e1-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="194e1-123">Request headers</span></span>
| <span data-ttu-id="194e1-124">Name</span><span class="sxs-lookup"><span data-stu-id="194e1-124">Name</span></span>       | <span data-ttu-id="194e1-125">Typ</span><span class="sxs-lookup"><span data-stu-id="194e1-125">Type</span></span> | <span data-ttu-id="194e1-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="194e1-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="194e1-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="194e1-127">Authorization</span></span>  | <span data-ttu-id="194e1-128">string</span><span class="sxs-lookup"><span data-stu-id="194e1-128">string</span></span>  | <span data-ttu-id="194e1-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="194e1-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="194e1-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="194e1-131">Content-Type</span></span>  | <span data-ttu-id="194e1-132">string</span><span class="sxs-lookup"><span data-stu-id="194e1-132">string</span></span>  | <span data-ttu-id="194e1-133">application/json</span><span class="sxs-lookup"><span data-stu-id="194e1-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="194e1-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="194e1-134">Request body</span></span>
<span data-ttu-id="194e1-135">Geben Sie im Anforderungstext eine JSON-Darstellung des [directoryRole](../resources/directoryrole.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="194e1-135">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="194e1-136">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Aktivieren einer Verzeichnisrolle erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="194e1-136">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="194e1-137">Parameter</span><span class="sxs-lookup"><span data-stu-id="194e1-137">Parameter</span></span> | <span data-ttu-id="194e1-138">Typ</span><span class="sxs-lookup"><span data-stu-id="194e1-138">Type</span></span> | <span data-ttu-id="194e1-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="194e1-139">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="194e1-140">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="194e1-140">roleTemplateId</span></span> | <span data-ttu-id="194e1-141">string</span><span class="sxs-lookup"><span data-stu-id="194e1-141">string</span></span> | <span data-ttu-id="194e1-142">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="194e1-142">Required.</span></span> <span data-ttu-id="194e1-143">Die ID des der [DirectoryRoleTemplate](../resources/directoryroletemplate.md) , die die Rolle basiert.</span><span class="sxs-lookup"><span data-stu-id="194e1-143">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on.</span></span> <span data-ttu-id="194e1-144">Dies ist die einzige Eigenschaft, die in der Anforderung angegeben werden können.</span><span class="sxs-lookup"><span data-stu-id="194e1-144">This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="194e1-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="194e1-145">Response</span></span>

<span data-ttu-id="194e1-146">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [directoryRole](../resources/directoryrole.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="194e1-146">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="194e1-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="194e1-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="194e1-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="194e1-148">Request</span></span>

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
<span data-ttu-id="194e1-149">Geben Sie im Anforderungstext eine JSON-Darstellung des [directoryRole](../resources/directoryrole.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="194e1-149">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="194e1-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="194e1-150">Response</span></span>
<span data-ttu-id="194e1-p106">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="194e1-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
