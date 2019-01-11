---
title: Abrufen einer Directory Einstellung-Vorlage
description: Verzeichnis Einstellung Vorlage stellt eine Vorlage der Einstellungen aus denen Einstellungen innerhalb einer mandantenstruktur erstellt werden können. Dieser Vorgang ermöglicht das Abrufen der Eigenschaften des DirectorySettingTemplate-Objekts, einschließlich der verfügbaren Einstellungen und Standardwerte.
localization_priority: Normal
ms.openlocfilehash: 55312fd4d7e2a77821dc7ad18ca3f67bded261df
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888172"
---
# <a name="get-a-directory-setting-template"></a><span data-ttu-id="a732f-104">Abrufen einer Directory Einstellung-Vorlage</span><span class="sxs-lookup"><span data-stu-id="a732f-104">Get a directory setting template</span></span>

> <span data-ttu-id="a732f-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a732f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a732f-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a732f-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a732f-107">Verzeichnis Einstellung Vorlage stellt eine Vorlage der Einstellungen aus denen Einstellungen innerhalb einer mandantenstruktur erstellt werden können.</span><span class="sxs-lookup"><span data-stu-id="a732f-107">A directory setting template represents a template of settings from which settings may be created within a tenant.</span></span> <span data-ttu-id="a732f-108">Dieser Vorgang ermöglicht das Abrufen der Eigenschaften des DirectorySettingTemplate-Objekts, einschließlich der verfügbaren Einstellungen und Standardwerte.</span><span class="sxs-lookup"><span data-stu-id="a732f-108">This operation allows retrieval of the properties of the directorySettingTemplate object, including the available settings and their defaults.</span></span>

> <span data-ttu-id="a732f-109">**Hinweis**: die Version /beta diese API ist nur auf Gruppen angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="a732f-109">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="a732f-110">Die /v1.0 Version dieser API wurde zum *Abrufen von GroupSettingTemplate*umbenannt.</span><span class="sxs-lookup"><span data-stu-id="a732f-110">The /v1.0 version of this API has been renamed to *Get groupSettingTemplate*.</span></span>

## <a name="permissions"></a><span data-ttu-id="a732f-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a732f-111">Permissions</span></span>
<span data-ttu-id="a732f-p105">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a732f-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a732f-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a732f-114">Permission type</span></span>      | <span data-ttu-id="a732f-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a732f-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a732f-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a732f-116">Delegated (work or school account)</span></span> | <span data-ttu-id="a732f-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a732f-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a732f-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a732f-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a732f-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a732f-119">Not supported.</span></span>    |
|<span data-ttu-id="a732f-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a732f-120">Application</span></span> | <span data-ttu-id="a732f-121">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a732f-121">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a732f-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a732f-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directorySettingTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a732f-123">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a732f-123">Optional query parameters</span></span>
<span data-ttu-id="a732f-124">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a732f-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a732f-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a732f-125">Request headers</span></span>
| <span data-ttu-id="a732f-126">Name</span><span class="sxs-lookup"><span data-stu-id="a732f-126">Name</span></span>      |<span data-ttu-id="a732f-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a732f-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a732f-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="a732f-128">Authorization</span></span>  | <span data-ttu-id="a732f-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a732f-p106">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a732f-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a732f-131">Request body</span></span>
<span data-ttu-id="a732f-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a732f-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a732f-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="a732f-133">Response</span></span>

<span data-ttu-id="a732f-134">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [DirectorySettingTemplate](../resources/directorysettingtemplate.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="a732f-134">If successful, this method returns a `200 OK` response code and [directorySettingTemplate](../resources/directorysettingtemplate.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a732f-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a732f-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a732f-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a732f-136">Request</span></span>
<span data-ttu-id="a732f-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a732f-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplate"
}-->
```http
GET https://graph.microsoft.com/beta/directorySettingTemplates/{id}
```
##### <a name="response"></a><span data-ttu-id="a732f-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="a732f-138">Response</span></span>
<span data-ttu-id="a732f-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a732f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get directorySettingTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
