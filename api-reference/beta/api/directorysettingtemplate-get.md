---
title: Abrufen einer Directory Einstellung-Vorlage
description: Verzeichnis Einstellung Vorlage stellt eine Vorlage der Einstellungen aus denen Einstellungen innerhalb einer mandantenstruktur erstellt werden können. Dieser Vorgang ermöglicht das Abrufen der Eigenschaften des DirectorySettingTemplate-Objekts, einschließlich der verfügbaren Einstellungen und Standardwerte.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c097d9919a52cde8559ead338f433b27a1e3e73d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529978"
---
# <a name="get-a-directory-setting-template"></a><span data-ttu-id="0bed7-104">Abrufen einer Directory Einstellung-Vorlage</span><span class="sxs-lookup"><span data-stu-id="0bed7-104">Get a directory setting template</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0bed7-105">Verzeichnis Einstellung Vorlage stellt eine Vorlage der Einstellungen aus denen Einstellungen innerhalb einer mandantenstruktur erstellt werden können.</span><span class="sxs-lookup"><span data-stu-id="0bed7-105">A directory setting template represents a template of settings from which settings may be created within a tenant.</span></span> <span data-ttu-id="0bed7-106">Dieser Vorgang ermöglicht das Abrufen der Eigenschaften des DirectorySettingTemplate-Objekts, einschließlich der verfügbaren Einstellungen und Standardwerte.</span><span class="sxs-lookup"><span data-stu-id="0bed7-106">This operation allows retrieval of the properties of the directorySettingTemplate object, including the available settings and their defaults.</span></span>

> <span data-ttu-id="0bed7-107">**Hinweis**: die Version /beta diese API ist nur auf Gruppen angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="0bed7-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="0bed7-108">Die /v1.0 Version dieser API wurde zum *Abrufen von GroupSettingTemplate*umbenannt.</span><span class="sxs-lookup"><span data-stu-id="0bed7-108">The /v1.0 version of this API has been renamed to *Get groupSettingTemplate*.</span></span>

## <a name="permissions"></a><span data-ttu-id="0bed7-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0bed7-109">Permissions</span></span>
<span data-ttu-id="0bed7-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0bed7-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0bed7-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0bed7-112">Permission type</span></span>      | <span data-ttu-id="0bed7-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0bed7-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0bed7-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0bed7-114">Delegated (work or school account)</span></span> | <span data-ttu-id="0bed7-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0bed7-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0bed7-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0bed7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0bed7-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0bed7-117">Not supported.</span></span>    |
|<span data-ttu-id="0bed7-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0bed7-118">Application</span></span> | <span data-ttu-id="0bed7-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bed7-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0bed7-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0bed7-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directorySettingTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0bed7-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="0bed7-121">Optional query parameters</span></span>
<span data-ttu-id="0bed7-122">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0bed7-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0bed7-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0bed7-123">Request headers</span></span>
| <span data-ttu-id="0bed7-124">Name</span><span class="sxs-lookup"><span data-stu-id="0bed7-124">Name</span></span>      |<span data-ttu-id="0bed7-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0bed7-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0bed7-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="0bed7-126">Authorization</span></span>  | <span data-ttu-id="0bed7-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0bed7-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bed7-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0bed7-129">Request body</span></span>
<span data-ttu-id="0bed7-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0bed7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0bed7-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="0bed7-131">Response</span></span>

<span data-ttu-id="0bed7-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [DirectorySettingTemplate](../resources/directorysettingtemplate.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="0bed7-132">If successful, this method returns a `200 OK` response code and [directorySettingTemplate](../resources/directorysettingtemplate.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0bed7-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0bed7-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0bed7-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0bed7-134">Request</span></span>
<span data-ttu-id="0bed7-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0bed7-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplate"
}-->
```http
GET https://graph.microsoft.com/beta/directorySettingTemplates/{id}
```
##### <a name="response"></a><span data-ttu-id="0bed7-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="0bed7-136">Response</span></span>
<span data-ttu-id="0bed7-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0bed7-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySettingTemplate"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 270

{
  "id": "id-value",
  "displayName": "displayName-value",
  "description": "description-value",
  "values": [
    {
      "name": "name-value",
      "type": "type-value",
      "defaultValue": "defaultValue-value",
      "description": "description-value"
    }
  ],
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get directorySettingTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directorysettingtemplate-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
