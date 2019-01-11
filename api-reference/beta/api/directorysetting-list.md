---
title: Verzeichnis listeneinstellungen
description: Abrufen einer Liste der Einstellung Verzeichnisobjekte.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 73756c81f19643fedcec0faa5f43125a7c389b35
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833411"
---
# <a name="list-directory-settings"></a><span data-ttu-id="f20d6-103">Verzeichnis listeneinstellungen</span><span class="sxs-lookup"><span data-stu-id="f20d6-103">List directory settings</span></span>

> <span data-ttu-id="f20d6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f20d6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f20d6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f20d6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f20d6-106">Abrufen einer Liste der Einstellung Verzeichnisobjekte.</span><span class="sxs-lookup"><span data-stu-id="f20d6-106">Retrieve a list of directory setting objects.</span></span>

> <span data-ttu-id="f20d6-107">**Hinweis**: die Version /beta diese API ist nur auf Gruppen angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="f20d6-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="f20d6-108">Die Version /v1.0 dieser API wurde in der *Liste GroupSettings*umbenannt.</span><span class="sxs-lookup"><span data-stu-id="f20d6-108">The /v1.0 version of this API has been renamed to *List groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="f20d6-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f20d6-109">Permissions</span></span>
<span data-ttu-id="f20d6-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f20d6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f20d6-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f20d6-112">Permission type</span></span>      | <span data-ttu-id="f20d6-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f20d6-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f20d6-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f20d6-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f20d6-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f20d6-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f20d6-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f20d6-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f20d6-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f20d6-117">Not supported.</span></span>    |
|<span data-ttu-id="f20d6-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f20d6-118">Application</span></span> | <span data-ttu-id="f20d6-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f20d6-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f20d6-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f20d6-120">HTTP request</span></span>
<span data-ttu-id="f20d6-121"><!-- { "blockType": "ignored" } -->Auflisten der gesamte Mandanten oder eine Gruppe von Einstellungen</span><span class="sxs-lookup"><span data-stu-id="f20d6-121"><!-- { "blockType": "ignored" } --> List tenant-wide or group settings</span></span>
```http
GET /settings
GET /group/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f20d6-122">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f20d6-122">Optional query parameters</span></span>
<span data-ttu-id="f20d6-123">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f20d6-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f20d6-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f20d6-124">Request headers</span></span>
| <span data-ttu-id="f20d6-125">Name</span><span class="sxs-lookup"><span data-stu-id="f20d6-125">Name</span></span>      |<span data-ttu-id="f20d6-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f20d6-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f20d6-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="f20d6-127">Authorization</span></span>  | <span data-ttu-id="f20d6-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f20d6-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f20d6-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f20d6-130">Request body</span></span>
<span data-ttu-id="f20d6-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f20d6-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f20d6-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="f20d6-132">Response</span></span>

<span data-ttu-id="f20d6-133">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [Verzeichnisberechtigungen](../resources/directorysetting.md) .</span><span class="sxs-lookup"><span data-stu-id="f20d6-133">If successful, this method returns a `200 OK` response code and collection of [directorySetting](../resources/directorysetting.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f20d6-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f20d6-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f20d6-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f20d6-135">Request</span></span>
<span data-ttu-id="f20d6-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f20d6-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_settings"
}-->
```http
GET https://graph.microsoft.com/beta/settings
```
##### <a name="response"></a><span data-ttu-id="f20d6-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="f20d6-137">Response</span></span>
<span data-ttu-id="f20d6-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f20d6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySetting",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
    {
      "id": "id-value",
      "displayName": "displayName-value",
      "settingTemplateId": "settingTemplateId-value",
      "values": [
        {
          "name": "name-value",
          "value": "value-value"
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
