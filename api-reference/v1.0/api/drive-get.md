---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Laufwerk abrufen
ms.openlocfilehash: 67d5dd612073db96ebcc5bf9c19aa004a034243c
ms.sourcegitcommit: 37591c2299c80e7675cd2b5f781e1eeeba628a60
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/08/2019
ms.locfileid: "27748423"
---
# <a name="get-drive"></a><span data-ttu-id="6e779-102">Laufwerk abrufen</span><span class="sxs-lookup"><span data-stu-id="6e779-102">Get Drive</span></span>

<span data-ttu-id="6e779-103">Dient zum Abrufen der Eigenschaften und der Beziehungen einer [Drive](../resources/drive.md)-Ressource.</span><span class="sxs-lookup"><span data-stu-id="6e779-103">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="6e779-104">Ein Laufwerk ist der Container auf oberster Ebene für ein Dateisystem, wie z. B. OneDrive oder SharePoint-Dokumentbibliotheken.</span><span class="sxs-lookup"><span data-stu-id="6e779-104">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e779-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6e779-105">Permissions</span></span>

<span data-ttu-id="6e779-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e779-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e779-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6e779-108">Permission type</span></span>      | <span data-ttu-id="6e779-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6e779-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e779-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6e779-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6e779-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e779-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="6e779-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6e779-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e779-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e779-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="6e779-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6e779-114">Application</span></span> | <span data-ttu-id="6e779-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e779-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="6e779-116">Abrufen des OneDrive des aktuellen Benutzers</span><span class="sxs-lookup"><span data-stu-id="6e779-116">Get current user's OneDrive</span></span>

<span data-ttu-id="6e779-117">Das Über den `me`-Singleton kann auf das Laufwerk des angemeldeten Benutzers (bei der Verwendung einer delegierten Authentifizierung) zugegriffen werden.</span><span class="sxs-lookup"><span data-stu-id="6e779-117">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="6e779-118">Wenn das OneDrive eines Benutzers nicht bereitgestellt ist, der Benutzer jedoch über eine Lizenz für OneDrive verfügt, wird über diese Anforderung das Laufwerk des Benutzers automatisch bereitgestellt, wenn eine delegierte Authentifizierung verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="6e779-118">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="6e779-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6e779-119">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive
```

## <a name="get-a-users-onedrive"></a><span data-ttu-id="6e779-120">Abrufen des OneDrive eines Benutzers</span><span class="sxs-lookup"><span data-stu-id="6e779-120">Get a user's OneDrive</span></span>

<span data-ttu-id="6e779-121">Damit Sie auf OneDrive oder OneDrive for Business eines Benutzers zugreifen können, muss Ihre App die **drive**-Beziehung in der User-Ressource anfordern.</span><span class="sxs-lookup"><span data-stu-id="6e779-121">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="6e779-122">Wenn das OneDrive eines Benutzers nicht bereitgestellt ist, der Benutzer jedoch über eine Lizenz für OneDrive verfügt, wird über diese Anforderung das Laufwerk des Benutzers automatisch bereitgestellt, wenn eine delegierte Authentifizierung verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="6e779-122">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="6e779-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6e779-123">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all", "tags": "service.graph" } -->

```http
GET /users/{idOrUserPrincipalName}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="6e779-124">Pfadparameter</span><span class="sxs-lookup"><span data-stu-id="6e779-124">Path parameters</span></span>

| <span data-ttu-id="6e779-125">Parametername</span><span class="sxs-lookup"><span data-stu-id="6e779-125">Parameter name</span></span> | <span data-ttu-id="6e779-126">Wert</span><span class="sxs-lookup"><span data-stu-id="6e779-126">Value</span></span>  | <span data-ttu-id="6e779-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6e779-127">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="6e779-128">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="6e779-128">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="6e779-129">string</span><span class="sxs-lookup"><span data-stu-id="6e779-129">string</span></span> | <span data-ttu-id="6e779-130">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6e779-130">Required.</span></span> <span data-ttu-id="6e779-131">Der Bezeichner für das Benutzerobjekt, dem OneDrive angehört.</span><span class="sxs-lookup"><span data-stu-id="6e779-131">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="6e779-132">Dient zum Abrufen der Dokumentbibliothek, die einer Gruppe zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="6e779-132">Get the document library associated with a group</span></span>

<span data-ttu-id="6e779-133">Für den Zugriff auf die Standarddokumentbibliothek einer **Gruppe** fordert Ihre App die drive-Beziehung in der Gruppe an.</span><span class="sxs-lookup"><span data-stu-id="6e779-133">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="6e779-134">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6e779-134">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all", "tags": "service.graph" } -->

```http
GET /groups/{groupId}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="6e779-135">Pfadparameter</span><span class="sxs-lookup"><span data-stu-id="6e779-135">Path parameters</span></span>

| <span data-ttu-id="6e779-136">Parametername</span><span class="sxs-lookup"><span data-stu-id="6e779-136">Parameter name</span></span> | <span data-ttu-id="6e779-137">Wert</span><span class="sxs-lookup"><span data-stu-id="6e779-137">Value</span></span>  | <span data-ttu-id="6e779-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6e779-138">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="6e779-139">_groupId_</span><span class="sxs-lookup"><span data-stu-id="6e779-139">_groupId_</span></span>      | <span data-ttu-id="6e779-140">string</span><span class="sxs-lookup"><span data-stu-id="6e779-140">string</span></span> | <span data-ttu-id="6e779-141">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6e779-141">Required.</span></span> <span data-ttu-id="6e779-142">Der Bezeichner für die Gruppe, die die Dokumentbibliothek besitzt.</span><span class="sxs-lookup"><span data-stu-id="6e779-142">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="6e779-143">Abrufen der Dokumentbibliothek für eine Website</span><span class="sxs-lookup"><span data-stu-id="6e779-143">Get the document library for a site</span></span>

<span data-ttu-id="6e779-144">Für den Zugriff auf die Standarddokumentbibliothek einer [Website](../resources/site.md) fordert Ihre App die **drive**-Beziehung auf der Website an.</span><span class="sxs-lookup"><span data-stu-id="6e779-144">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="6e779-145">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6e779-145">HTTP request</span></span>

```http
GET /sites/{siteId}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="6e779-146">Pfadparameter</span><span class="sxs-lookup"><span data-stu-id="6e779-146">Path parameters</span></span>

| <span data-ttu-id="6e779-147">Parametername</span><span class="sxs-lookup"><span data-stu-id="6e779-147">Parameter name</span></span> | <span data-ttu-id="6e779-148">Wert</span><span class="sxs-lookup"><span data-stu-id="6e779-148">Value</span></span>  | <span data-ttu-id="6e779-149">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6e779-149">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="6e779-150">_siteId_</span><span class="sxs-lookup"><span data-stu-id="6e779-150">_siteId_</span></span>       | <span data-ttu-id="6e779-151">string</span><span class="sxs-lookup"><span data-stu-id="6e779-151">string</span></span> | <span data-ttu-id="6e779-152">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6e779-152">Required.</span></span> <span data-ttu-id="6e779-153">Der Bezeichner für die Website, die die Dokumentbibliothek enthält.</span><span class="sxs-lookup"><span data-stu-id="6e779-153">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="6e779-154">Abrufen eines Laufwerks nach ID</span><span class="sxs-lookup"><span data-stu-id="6e779-154">Get a drive by ID</span></span>

<span data-ttu-id="6e779-155">Wenn Sie die eindeutige ID für ein Laufwerk besitzen, können Sie direkt über die Websitesammlung auf oberster Ebene darauf zugreifen.</span><span class="sxs-lookup"><span data-stu-id="6e779-155">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="6e779-156">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6e779-156">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}
```

### <a name="path-parameters"></a><span data-ttu-id="6e779-157">Pfadparameter</span><span class="sxs-lookup"><span data-stu-id="6e779-157">Path parameters</span></span>

| <span data-ttu-id="6e779-158">Parametername</span><span class="sxs-lookup"><span data-stu-id="6e779-158">Parameter name</span></span> | <span data-ttu-id="6e779-159">Wert</span><span class="sxs-lookup"><span data-stu-id="6e779-159">Value</span></span>  | <span data-ttu-id="6e779-160">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6e779-160">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="6e779-161">_driveId_</span><span class="sxs-lookup"><span data-stu-id="6e779-161">_driveId_</span></span>      | <span data-ttu-id="6e779-162">string</span><span class="sxs-lookup"><span data-stu-id="6e779-162">string</span></span> | <span data-ttu-id="6e779-163">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6e779-163">Required.</span></span> <span data-ttu-id="6e779-164">Dies ist der Bezeichner des angeforderten Laufwerks.</span><span class="sxs-lookup"><span data-stu-id="6e779-164">The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="6e779-165">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="6e779-165">Optional query parameters</span></span>

<span data-ttu-id="6e779-166">Diese Methode unterstützt die [$select-Abfrageparameter] [ odata-query-parameters] zum Modellieren der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6e779-166">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="6e779-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="6e779-167">Response</span></span>

<span data-ttu-id="6e779-168">Diese Methoden gebeneine [Drive-Ressource][drive-resource] für das entsprechende Laufwerk im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6e779-168">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

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

### <a name="error-response-codes"></a><span data-ttu-id="6e779-169">Fehlerantwortcodes</span><span class="sxs-lookup"><span data-stu-id="6e779-169">Error response codes</span></span>

<span data-ttu-id="6e779-170">Wenn das Laufwerk nicht vorhanden ist und nicht automatisch bereitgestellt werden kann (wenn die delegierte Authentifizierung verwendet wird), wird eine `HTTP 404`-Antwort zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6e779-170">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

[drive-resource]: ../resources/drive.md
[odata-query-parameters]: /graph/query-parameters

<!-- {
  "type": "#page.annotation",
  "description": "Get metadata for a OneDrive, OneDrive for Business, or Office 365 group drive",
  "keywords": "drive,onedrive,default drive,group drive",
  "section": "documentation",
  "suppressions": [
      "Warning: /api-reference/v1.0/api/drive-get.md:
        Unable to map some markdown elements into schema.
            Unmapped methods:
        get-drive-default, get-drive-by-user, get-drive-by-group, get-drive-by-id
            Unmapped tables:
        Permissions - AuthScopes, Path parameters - PathParameters, Path parameters - PathParameters, Path parameters - PathParameters, Path parameters - PathParameters"
  ],
  "tocPath": "Drives/Get drive"
} -->
