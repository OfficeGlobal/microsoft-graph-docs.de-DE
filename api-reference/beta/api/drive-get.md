---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Laufwerk abrufen
ms.openlocfilehash: 903eb9d5886bf2ec3b7f8672438f01482e754f9b
ms.sourcegitcommit: 37591c2299c80e7675cd2b5f781e1eeeba628a60
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/08/2019
ms.locfileid: "27748591"
---
# <a name="get-drive"></a><span data-ttu-id="d769b-102">Laufwerk abrufen</span><span class="sxs-lookup"><span data-stu-id="d769b-102">Get Drive</span></span>

> <span data-ttu-id="d769b-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d769b-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d769b-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d769b-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d769b-105">Dient zum Abrufen der Eigenschaften und der Beziehungen einer [Drive](../resources/drive.md)-Ressource.</span><span class="sxs-lookup"><span data-stu-id="d769b-105">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="d769b-106">Ein Laufwerk ist der Container auf oberster Ebene für ein Dateisystem, wie z. B. OneDrive oder SharePoint-Dokumentbibliotheken.</span><span class="sxs-lookup"><span data-stu-id="d769b-106">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="d769b-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d769b-107">Permissions</span></span>

<span data-ttu-id="d769b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d769b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d769b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d769b-110">Permission type</span></span>      | <span data-ttu-id="d769b-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d769b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d769b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d769b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d769b-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d769b-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d769b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d769b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d769b-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d769b-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="d769b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d769b-116">Application</span></span> | <span data-ttu-id="d769b-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d769b-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="d769b-118">Abrufen des OneDrive des aktuellen Benutzers</span><span class="sxs-lookup"><span data-stu-id="d769b-118">Get current user's OneDrive</span></span>

<span data-ttu-id="d769b-119">Das Über den `me`-Singleton kann auf das Laufwerk des angemeldeten Benutzers (bei der Verwendung einer delegierten Authentifizierung) zugegriffen werden.</span><span class="sxs-lookup"><span data-stu-id="d769b-119">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="d769b-120">Wenn das OneDrive eines Benutzers nicht bereitgestellt ist, der Benutzer jedoch über eine Lizenz für OneDrive verfügt, wird über diese Anforderung das Laufwerk des Benutzers automatisch bereitgestellt, wenn eine delegierte Authentifizierung verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="d769b-120">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="d769b-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d769b-121">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read" } -->

```http
GET /me/drive
```

## <a name="get-a-users-onedrive"></a><span data-ttu-id="d769b-122">Abrufen des OneDrive eines Benutzers</span><span class="sxs-lookup"><span data-stu-id="d769b-122">Get a user's OneDrive</span></span>

<span data-ttu-id="d769b-123">Damit Sie auf OneDrive oder OneDrive for Business eines Benutzers zugreifen können, muss Ihre App die **drive**-Beziehung in der User-Ressource anfordern.</span><span class="sxs-lookup"><span data-stu-id="d769b-123">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="d769b-124">Wenn das OneDrive eines Benutzers nicht bereitgestellt ist, der Benutzer jedoch über eine Lizenz für OneDrive verfügt, wird über diese Anforderung das Laufwerk des Benutzers automatisch bereitgestellt, wenn eine delegierte Authentifizierung verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="d769b-124">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="d769b-125">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d769b-125">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all" } -->

```http
GET /users/{idOrUserPrincipalName}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="d769b-126">Pfadparameter</span><span class="sxs-lookup"><span data-stu-id="d769b-126">Path parameters</span></span>

| <span data-ttu-id="d769b-127">Parametername</span><span class="sxs-lookup"><span data-stu-id="d769b-127">Parameter name</span></span> | <span data-ttu-id="d769b-128">Wert</span><span class="sxs-lookup"><span data-stu-id="d769b-128">Value</span></span>  | <span data-ttu-id="d769b-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d769b-129">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="d769b-130">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="d769b-130">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="d769b-131">string</span><span class="sxs-lookup"><span data-stu-id="d769b-131">string</span></span> | <span data-ttu-id="d769b-132">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d769b-132">Required.</span></span> <span data-ttu-id="d769b-133">Der Bezeichner für das Benutzerobjekt, dem OneDrive angehört.</span><span class="sxs-lookup"><span data-stu-id="d769b-133">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="d769b-134">Dient zum Abrufen der Dokumentbibliothek, die einer Gruppe zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="d769b-134">Get the document library associated with a group</span></span>

<span data-ttu-id="d769b-135">Für den Zugriff auf die Standarddokumentbibliothek einer **Gruppe** fordert Ihre App die drive-Beziehung in der Gruppe an.</span><span class="sxs-lookup"><span data-stu-id="d769b-135">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="d769b-136">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d769b-136">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all" } -->

```http
GET /groups/{groupId}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="d769b-137">Pfadparameter</span><span class="sxs-lookup"><span data-stu-id="d769b-137">Path parameters</span></span>

| <span data-ttu-id="d769b-138">Parametername</span><span class="sxs-lookup"><span data-stu-id="d769b-138">Parameter name</span></span> | <span data-ttu-id="d769b-139">Wert</span><span class="sxs-lookup"><span data-stu-id="d769b-139">Value</span></span>  | <span data-ttu-id="d769b-140">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d769b-140">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="d769b-141">_groupId_</span><span class="sxs-lookup"><span data-stu-id="d769b-141">_groupId_</span></span>      | <span data-ttu-id="d769b-142">string</span><span class="sxs-lookup"><span data-stu-id="d769b-142">string</span></span> | <span data-ttu-id="d769b-143">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d769b-143">Required.</span></span> <span data-ttu-id="d769b-144">Der Bezeichner für die Gruppe, die die Dokumentbibliothek besitzt.</span><span class="sxs-lookup"><span data-stu-id="d769b-144">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="d769b-145">Abrufen der Dokumentbibliothek für eine Website</span><span class="sxs-lookup"><span data-stu-id="d769b-145">Get the document library for a site</span></span>

<span data-ttu-id="d769b-146">Für den Zugriff auf die Standarddokumentbibliothek einer [Website](../resources/site.md) fordert Ihre App die **drive**-Beziehung auf der Website an.</span><span class="sxs-lookup"><span data-stu-id="d769b-146">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="d769b-147">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d769b-147">HTTP request</span></span>

```http
GET /sites/{siteId}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="d769b-148">Pfadparameter</span><span class="sxs-lookup"><span data-stu-id="d769b-148">Path parameters</span></span>

| <span data-ttu-id="d769b-149">Parametername</span><span class="sxs-lookup"><span data-stu-id="d769b-149">Parameter name</span></span> | <span data-ttu-id="d769b-150">Wert</span><span class="sxs-lookup"><span data-stu-id="d769b-150">Value</span></span>  | <span data-ttu-id="d769b-151">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d769b-151">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="d769b-152">_siteId_</span><span class="sxs-lookup"><span data-stu-id="d769b-152">_siteId_</span></span>       | <span data-ttu-id="d769b-153">string</span><span class="sxs-lookup"><span data-stu-id="d769b-153">string</span></span> | <span data-ttu-id="d769b-154">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d769b-154">Required.</span></span> <span data-ttu-id="d769b-155">Der Bezeichner für die Website, die die Dokumentbibliothek enthält.</span><span class="sxs-lookup"><span data-stu-id="d769b-155">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="d769b-156">Abrufen eines Laufwerks nach ID</span><span class="sxs-lookup"><span data-stu-id="d769b-156">Get a drive by ID</span></span>

<span data-ttu-id="d769b-157">Wenn Sie die eindeutige ID für ein Laufwerk besitzen, können Sie direkt über die Websitesammlung auf oberster Ebene darauf zugreifen.</span><span class="sxs-lookup"><span data-stu-id="d769b-157">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="d769b-158">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d769b-158">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```http
GET /drives/{driveId}
```

### <a name="path-parameters"></a><span data-ttu-id="d769b-159">Pfadparameter</span><span class="sxs-lookup"><span data-stu-id="d769b-159">Path parameters</span></span>

| <span data-ttu-id="d769b-160">Parametername</span><span class="sxs-lookup"><span data-stu-id="d769b-160">Parameter name</span></span> | <span data-ttu-id="d769b-161">Wert</span><span class="sxs-lookup"><span data-stu-id="d769b-161">Value</span></span>  | <span data-ttu-id="d769b-162">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d769b-162">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="d769b-163">_driveId_</span><span class="sxs-lookup"><span data-stu-id="d769b-163">_driveId_</span></span>      | <span data-ttu-id="d769b-164">string</span><span class="sxs-lookup"><span data-stu-id="d769b-164">string</span></span> | <span data-ttu-id="d769b-165">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d769b-165">Required.</span></span> <span data-ttu-id="d769b-166">Dies ist der Bezeichner des angeforderten Laufwerks.</span><span class="sxs-lookup"><span data-stu-id="d769b-166">The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="d769b-167">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="d769b-167">Optional query parameters</span></span>

<span data-ttu-id="d769b-168">Diese Methode unterstützt die [$select-Abfrageparameter] [ odata-query-parameters] zum Modellieren der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d769b-168">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="d769b-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="d769b-169">Response</span></span>

<span data-ttu-id="d769b-170">Diese Methoden gebeneine [Drive-Ressource][drive-resource] für das entsprechende Laufwerk im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d769b-170">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.drive", "truncated": true, "name": ["get-drive-by-id", "get-drive-by-group", "get-drive-by-user", "get-drive-default"] } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "b!t18F8ybsHUq1z3LTz8xvZqP8zaSWjkFNhsME-Fepo75dTf9vQKfeRblBZjoSQrd7",
    "driveType": "business",
    "owner": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "Ryan Gregg"
        }
    },
    "quota": {
        "deleted": 256938,
        "remaining": 1099447353539,
        "state": "normal",
        "total": 1099511627776
    }
}
```

### <a name="error-response-codes"></a><span data-ttu-id="d769b-171">Fehlerantwortcodes</span><span class="sxs-lookup"><span data-stu-id="d769b-171">Error response codes</span></span>

<span data-ttu-id="d769b-172">Wenn das Laufwerk nicht vorhanden ist und nicht automatisch bereitgestellt werden kann (wenn die delegierte Authentifizierung verwendet wird), wird eine `HTTP 404`-Antwort zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d769b-172">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

[drive-resource]: ../resources/drive.md
[odata-query-parameters]: /graph/query-parameters

<!-- {
  "type": "#page.annotation",
  "description": "Get metadata for a OneDrive, OneDrive for Business, or Office 365 group drive",
  "keywords": "drive,onedrive,default drive,group drive",
  "section": "documentation",
  "tocPath": "Drives/Get drive"
} -->
