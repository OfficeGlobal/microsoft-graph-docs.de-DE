---
title: directoryRole aktivieren
description: Dient zum Aktivieren einer Verzeichnisrolle. Um eine Rolle Directory lesen oder deren Member aktualisieren möchten, müssen sie zuerst im Mandanten aktiviert werden. Nur die Administratoren im Unternehmen und die impliziten Benutzer Directory Rollen sind standardmäßig aktiviert. Zugriff auf und Zuweisen von Mitgliedern zu einer anderen Verzeichnis Rolle, müssen Sie zuerst mit der entsprechenden Verzeichnis Rolle-Vorlage (DirectoryRoleTemplate) aktivieren.
ms.openlocfilehash: 2a81bedaf4998e44825abc5e2cf0a93ec8708f96
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060569"
---
# <a name="activate-directoryrole"></a><span data-ttu-id="9f5a1-106">directoryRole aktivieren</span><span class="sxs-lookup"><span data-stu-id="9f5a1-106">Activate directoryRole</span></span>

> <span data-ttu-id="9f5a1-107">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9f5a1-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f5a1-108">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9f5a1-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9f5a1-109">Dient zum Aktivieren einer Verzeichnisrolle.</span><span class="sxs-lookup"><span data-stu-id="9f5a1-109">Activate a directory role.</span></span> <span data-ttu-id="9f5a1-110">Um eine Rolle Directory lesen oder deren Member aktualisieren möchten, müssen sie zuerst im Mandanten aktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="9f5a1-110">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="9f5a1-111">Nur die Administratoren im Unternehmen und die impliziten Benutzer Directory Rollen sind standardmäßig aktiviert.</span><span class="sxs-lookup"><span data-stu-id="9f5a1-111">Only the Company Administrators  and the implicit Users directory roles are activated by default.</span></span> <span data-ttu-id="9f5a1-112">Zugriff auf und Zuweisen von Mitgliedern zu einer anderen Verzeichnis Rolle, müssen Sie zuerst mit der entsprechenden Verzeichnis Rolle-Vorlage ([DirectoryRoleTemplate](../resources/directoryroletemplate.md)) aktivieren.</span><span class="sxs-lookup"><span data-stu-id="9f5a1-112">To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="9f5a1-113">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9f5a1-113">Permissions</span></span>
<span data-ttu-id="9f5a1-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f5a1-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f5a1-116">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9f5a1-116">Permission type</span></span>      | <span data-ttu-id="9f5a1-117">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9f5a1-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f5a1-118">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9f5a1-118">Delegated (work or school account)</span></span> | <span data-ttu-id="9f5a1-119">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9f5a1-119">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9f5a1-120">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9f5a1-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f5a1-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9f5a1-121">Not supported.</span></span>    |
|<span data-ttu-id="9f5a1-122">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9f5a1-122">Application</span></span> | <span data-ttu-id="9f5a1-123">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f5a1-123">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f5a1-124">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9f5a1-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="9f5a1-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9f5a1-125">Request headers</span></span>
| <span data-ttu-id="9f5a1-126">Name</span><span class="sxs-lookup"><span data-stu-id="9f5a1-126">Name</span></span>       | <span data-ttu-id="9f5a1-127">Typ</span><span class="sxs-lookup"><span data-stu-id="9f5a1-127">Type</span></span> | <span data-ttu-id="9f5a1-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9f5a1-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9f5a1-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f5a1-129">Authorization</span></span>  | <span data-ttu-id="9f5a1-130">string</span><span class="sxs-lookup"><span data-stu-id="9f5a1-130">string</span></span>  | <span data-ttu-id="9f5a1-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9f5a1-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9f5a1-133">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9f5a1-133">Request body</span></span>
<span data-ttu-id="9f5a1-134">Geben Sie im Anforderungstext eine JSON-Darstellung des [directoryRole](../resources/directoryrole.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="9f5a1-134">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="9f5a1-135">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Aktivieren einer Verzeichnisrolle erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="9f5a1-135">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="9f5a1-136">Erforderliche Parameter</span><span class="sxs-lookup"><span data-stu-id="9f5a1-136">Required parameter</span></span> | <span data-ttu-id="9f5a1-137">Typ</span><span class="sxs-lookup"><span data-stu-id="9f5a1-137">Type</span></span> | <span data-ttu-id="9f5a1-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9f5a1-138">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="9f5a1-139">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="9f5a1-139">roleTemplateId</span></span> | <span data-ttu-id="9f5a1-140">string</span><span class="sxs-lookup"><span data-stu-id="9f5a1-140">string</span></span> | <span data-ttu-id="9f5a1-p106">Die ID der [directoryRoleTemplate](../resources/directoryroletemplate.md), auf der die Rolle basiert. Dies ist die einzige Eigenschaft, die in der Anforderung angegeben werden kann.</span><span class="sxs-lookup"><span data-stu-id="9f5a1-p106">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on. This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="9f5a1-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="9f5a1-143">Response</span></span>

<span data-ttu-id="9f5a1-144">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [directoryRole](../resources/directoryrole.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9f5a1-144">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f5a1-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9f5a1-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9f5a1-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9f5a1-146">Request</span></span>
<span data-ttu-id="9f5a1-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9f5a1-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryrole_from_directoryroles"
}-->
```http
POST https://graph.microsoft.com/beta/directoryRoles
Content-type: application/json
Content-length: 153

{
  "description": "description-value",
  "displayName": "displayName-value",
  "roleTemplateId": "roleTemplateId-value"
}
```
<span data-ttu-id="9f5a1-148">Geben Sie im Anforderungstext eine JSON-Darstellung des [directoryRole](../resources/directoryrole.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="9f5a1-148">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="9f5a1-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="9f5a1-149">Response</span></span>
<span data-ttu-id="9f5a1-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9f5a1-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 175

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