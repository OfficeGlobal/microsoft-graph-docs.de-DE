---
title: directoryRole aktivieren
description: Dient zum Aktivieren einer Verzeichnisrolle. Um eine Verzeichnisrolle zu lesen oder ihre Mitglieder zu aktualisieren, muss diese zuerst im Mandanten aktiviert werden. Nur die Unternehmensadministratoren und die impliziten Benutzerverzeichnisrollen sind standardmäßig aktiviert. Um auf Mitglieder zuzugreifen und diese einer anderen Verzeichnisrolle zuzuweisen, müssen Sie diese zuerst mit der entsprechenden Verzeichnisrollenvorlage aktivieren (directoryRoleTemplate).
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 094374dd8aa5d68e1adaad89e9a3b46987bc7c8f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522728"
---
# <a name="activate-directoryrole"></a><span data-ttu-id="f348e-106">directoryRole aktivieren</span><span class="sxs-lookup"><span data-stu-id="f348e-106">Activate directoryRole</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f348e-107">Dient zum Aktivieren einer Verzeichnisrolle.</span><span class="sxs-lookup"><span data-stu-id="f348e-107">Activate a directory role.</span></span> <span data-ttu-id="f348e-108">Um eine Rolle Directory lesen oder deren Member aktualisieren möchten, müssen sie zuerst im Mandanten aktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="f348e-108">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="f348e-109">Nur die Administratoren im Unternehmen und die impliziten Benutzer Directory Rollen sind standardmäßig aktiviert.</span><span class="sxs-lookup"><span data-stu-id="f348e-109">Only the Company Administrators  and the implicit Users directory roles are activated by default.</span></span> <span data-ttu-id="f348e-110">Zugriff auf und Zuweisen von Mitgliedern zu einer anderen Verzeichnis Rolle, müssen Sie zuerst mit der entsprechenden Verzeichnis Rolle-Vorlage ([DirectoryRoleTemplate](../resources/directoryroletemplate.md)) aktivieren.</span><span class="sxs-lookup"><span data-stu-id="f348e-110">To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="f348e-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f348e-111">Permissions</span></span>
<span data-ttu-id="f348e-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f348e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f348e-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f348e-114">Permission type</span></span>      | <span data-ttu-id="f348e-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f348e-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f348e-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f348e-116">Delegated (work or school account)</span></span> | <span data-ttu-id="f348e-117">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f348e-117">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f348e-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f348e-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f348e-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f348e-119">Not supported.</span></span>    |
|<span data-ttu-id="f348e-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f348e-120">Application</span></span> | <span data-ttu-id="f348e-121">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f348e-121">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f348e-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f348e-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="f348e-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f348e-123">Request headers</span></span>
| <span data-ttu-id="f348e-124">Name</span><span class="sxs-lookup"><span data-stu-id="f348e-124">Name</span></span>       | <span data-ttu-id="f348e-125">Typ</span><span class="sxs-lookup"><span data-stu-id="f348e-125">Type</span></span> | <span data-ttu-id="f348e-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f348e-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f348e-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="f348e-127">Authorization</span></span>  | <span data-ttu-id="f348e-128">String</span><span class="sxs-lookup"><span data-stu-id="f348e-128">string</span></span>  | <span data-ttu-id="f348e-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f348e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f348e-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f348e-131">Request body</span></span>
<span data-ttu-id="f348e-132">Geben Sie im Anforderungstext eine JSON-Darstellung des [directoryRole](../resources/directoryrole.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="f348e-132">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="f348e-133">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Aktivieren einer Verzeichnisrolle erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="f348e-133">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="f348e-134">Erforderliche Parameter</span><span class="sxs-lookup"><span data-stu-id="f348e-134">Required parameter</span></span> | <span data-ttu-id="f348e-135">Typ</span><span class="sxs-lookup"><span data-stu-id="f348e-135">Type</span></span> | <span data-ttu-id="f348e-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f348e-136">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="f348e-137">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="f348e-137">roleTemplateId</span></span> | <span data-ttu-id="f348e-138">string</span><span class="sxs-lookup"><span data-stu-id="f348e-138">string</span></span> | <span data-ttu-id="f348e-p105">Die ID der [directoryRoleTemplate](../resources/directoryroletemplate.md), auf der die Rolle basiert. Dies ist die einzige Eigenschaft, die in der Anforderung angegeben werden kann.</span><span class="sxs-lookup"><span data-stu-id="f348e-p105">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on. This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="f348e-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="f348e-141">Response</span></span>

<span data-ttu-id="f348e-142">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [directoryRole](../resources/directoryrole.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f348e-142">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f348e-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f348e-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f348e-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f348e-144">Request</span></span>
<span data-ttu-id="f348e-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f348e-145">Here is an example of the request.</span></span>
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
<span data-ttu-id="f348e-146">Geben Sie im Anforderungstext eine JSON-Darstellung des [directoryRole](../resources/directoryrole.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="f348e-146">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f348e-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="f348e-147">Response</span></span>
<span data-ttu-id="f348e-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f348e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directoryrole-post-directoryroles.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
