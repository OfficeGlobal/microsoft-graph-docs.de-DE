---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Spezielle Ordner abgerufen
ms.openlocfilehash: 758d46b8237ecd2ce94d4e3a270a188300817fcf
ms.sourcegitcommit: 37591c2299c80e7675cd2b5f781e1eeeba628a60
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/08/2019
ms.locfileid: "27748255"
---
# <a name="get-a-special-folder-by-name"></a><span data-ttu-id="f5141-102">Speziellen Ordner nach Name abrufen</span><span class="sxs-lookup"><span data-stu-id="f5141-102">Get a special folder by name</span></span>

<span data-ttu-id="f5141-103">Verwenden Sie spezielle Auflistung, um auf einen speziellen Ordner basierend auf dem Namen zuzugreifen.</span><span class="sxs-lookup"><span data-stu-id="f5141-103">Use the special collection to access a special folder by name.</span></span>

<span data-ttu-id="f5141-p101">Spezielle Ordner bieten einfache Aliase für den Zugriff auf bekannte Ordner in OneDrive, ohne dass der Ordner anhand des Pfads nachgeschlagen werden muss (wofür eine Lokalisierung erforderlich wäre) oder anhand einer ID auf den Ordner verwiesen werden muss. Wenn ein spezieller Ordner umbenannt oder an eine andere Position innerhalb des Laufwerks verschoben wird, kann mit dieser Syntax weiterhin nach diesem Ordner gesucht werden.</span><span class="sxs-lookup"><span data-stu-id="f5141-p101">Special folders provide simple aliases to access well-known folders in OneDrive without the need to look up the folder by path (which would require localization), or reference the folder with an ID. If a special folder is renamed or moved to another location within the drive, this syntax will continue to find that folder.</span></span>

<span data-ttu-id="f5141-p102">Spezielle Ordner werden automatisch erstellt, wenn eine Anwendung das erste Mal versucht, einen Ordner zu schreiben, wenn noch keiner vorhanden ist. Wenn ein Benutzer einen speziellen Ordner löscht, wird dieser neu erstellt, wenn erneut in den Ordner geschrieben wird.</span><span class="sxs-lookup"><span data-stu-id="f5141-p102">Special folders are automatically created the first time an application attempts to write to one, if it doesn't already exist. If a user deletes one, it is recreated when written to again.</span></span>

> <span data-ttu-id="f5141-108">**Hinweis:**  Wenn Sie nur über Leseberechtigungen verfügen und einen speziellen Ordner anfordern, der nicht vorhanden ist, wird ein `403 Forbidden`-Fehler angezeigt.</span><span class="sxs-lookup"><span data-stu-id="f5141-108">**Note:**  If you have read-only permissions and request a special folder that doesn't exist, you'll receive a `403 Forbidden` error.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5141-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f5141-109">Permissions</span></span>

<span data-ttu-id="f5141-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5141-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="f5141-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f5141-112">Permission type</span></span>             |                                           <span data-ttu-id="f5141-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f5141-113">Permissions (from least to most privileged)</span></span>                                            |
| :------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="f5141-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f5141-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="f5141-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5141-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>                            |
| <span data-ttu-id="f5141-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f5141-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5141-117">Files.ReadWrite.AppFolder, Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5141-117">Files.ReadWrite.AppFolder, Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |
| <span data-ttu-id="f5141-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f5141-118">Application</span></span>                            | <span data-ttu-id="f5141-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5141-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>                                                         |

## <a name="http-request"></a><span data-ttu-id="f5141-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f5141-120">HTTP Request</span></span>

<!-- { "blockType": "request", "name": "get-special-folder", "scopes": "files.read" } -->

```http
GET /me/drive/special/{name}
```

### <a name="special-folder-names"></a><span data-ttu-id="f5141-121">Namen für spezielle Ordner</span><span class="sxs-lookup"><span data-stu-id="f5141-121">Special folder names</span></span>

<span data-ttu-id="f5141-122">Im Folgenden sind Namen für spezielle Ordner aufgelistet, die in OneDrive und OneDrive for Business zur Verfügung stehen.</span><span class="sxs-lookup"><span data-stu-id="f5141-122">The follow special folder names are available in OneDrive and OneDrive for Business.</span></span>

| <span data-ttu-id="f5141-123">Name</span><span class="sxs-lookup"><span data-stu-id="f5141-123">Name</span></span>        | <span data-ttu-id="f5141-124">Ordner-ID</span><span class="sxs-lookup"><span data-stu-id="f5141-124">Folder id</span></span>    | <span data-ttu-id="f5141-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f5141-125">Description</span></span>                                                              |
|:------------|:-------------|:-------------------------------------------------------------------------|
| <span data-ttu-id="f5141-126">Dokumente</span><span class="sxs-lookup"><span data-stu-id="f5141-126">Documents</span></span>   | `documents`  | <span data-ttu-id="f5141-127">Der Ordner „Dokumente“.</span><span class="sxs-lookup"><span data-stu-id="f5141-127">The Documents folder.</span></span>                                                    |
| <span data-ttu-id="f5141-128">Fotos</span><span class="sxs-lookup"><span data-stu-id="f5141-128">Photos</span></span>      | `photos`     | <span data-ttu-id="f5141-129">Der Ordner „Fotos“.</span><span class="sxs-lookup"><span data-stu-id="f5141-129">The Photos folder.</span></span>                                                       |
| <span data-ttu-id="f5141-130">Eigene Aufnahmen</span><span class="sxs-lookup"><span data-stu-id="f5141-130">Camera Roll</span></span> | `cameraroll` | <span data-ttu-id="f5141-131">Der Sicherungsordner für Eigene Aufnahmen.</span><span class="sxs-lookup"><span data-stu-id="f5141-131">The Camera Roll Backup folder.</span></span>                                           |
| <span data-ttu-id="f5141-132">Anwendungsstamm</span><span class="sxs-lookup"><span data-stu-id="f5141-132">App Root</span></span>    | `approot`    | <span data-ttu-id="f5141-p104">Der persönliche Ordner der Anwendung. In der Regel unter `/Apps/{Application Name}`</span><span class="sxs-lookup"><span data-stu-id="f5141-p104">The application's personal folder. Usually in `/Apps/{Application Name}`</span></span> |
| <span data-ttu-id="f5141-135">Musik</span><span class="sxs-lookup"><span data-stu-id="f5141-135">Music</span></span>       | `music`      | <span data-ttu-id="f5141-136">Der Ordner „Musik“.</span><span class="sxs-lookup"><span data-stu-id="f5141-136">The Music folder.</span></span>                                                        |


### <a name="optional-query-parameters"></a><span data-ttu-id="f5141-137">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f5141-137">Optional query parameters</span></span>

<span data-ttu-id="f5141-138">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) von `$expand` und `$select` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f5141-138">This method supports the `$expand` and `$select` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="f5141-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="f5141-139">Response</span></span>

<span data-ttu-id="f5141-140">Die Methode gibt den Antwortcode `200 OK` und das aktualisierte [driveItem](../resources/driveitem.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f5141-140">This method returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) object in the response body.</span></span>

<span data-ttu-id="f5141-141">Sie können diese Methode der Adressierung eines speziellen Ordners mit dem zusätzlichen Aufruf der Eigenschaften oder Beziehungen auf das DriveItem anwenden.</span><span class="sxs-lookup"><span data-stu-id="f5141-141">You can use this method of addressing a special folder inline with additional calls to properties or relationships on the driveItem.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "0123456789abc",
  "name": "Documents",
  "eTag": "012345819293.1",
  "specialFolder": {
    "name": "documents"
  }
}
```

## <a name="get-children-of-a-special-folder"></a><span data-ttu-id="f5141-142">Abrufen der untergeordneten Elemente eines speziellen Ordners</span><span class="sxs-lookup"><span data-stu-id="f5141-142">Get children of a special folder</span></span>

<span data-ttu-id="f5141-143">Um die untergeordneten Elemente eines speziellen Ordners anzufordern, können Sie die `children`-Sammlung anfordern oder die Option [expand](/graph/query-parameters) verwenden, um die Sammlung untergeordneter Elemente zu erweitern.</span><span class="sxs-lookup"><span data-stu-id="f5141-143">To request the children of a special folder, you can request the `children` collection or use the [expand](/graph/query-parameters) option to expand the children collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="f5141-144">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f5141-144">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-special-children", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/special/{special-folder-name}/children
```

### <a name="response"></a><span data-ttu-id="f5141-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="f5141-145">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "isCollection": true, "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {"name": "myfile.jpg", "size": 2048 },
    {"name": "Documents", "folder": { "childCount": 4} },
    {"name": "Photos", "folder": { "childCount": 203} },
    {"name": "my sheet(1).xlsx", "size": 197 }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="f5141-146">Hinweise</span><span class="sxs-lookup"><span data-stu-id="f5141-146">Remarks</span></span>

> <span data-ttu-id="f5141-147">**Hinweis:** DriveItems mit der `specialFolder`-Facette geben an, dass das Element ein spezieller Ordner ist und der Zugriff über die `special`-Sammlung erfolgen kann.</span><span class="sxs-lookup"><span data-stu-id="f5141-147">**Note:** DriveItems with the `specialFolder` facet indicate the item is a special folder and can be accessed via the `special` collection.</span></span>

<span data-ttu-id="f5141-148">Wenn Ihre App über Leseberechtigungen verfügt, schläft die Anforderung zum Abrufen eines speziellen Ordners oder der untergeordneten Elemente eines speziellen Ordners mit dem Fehler `404 Not Found` oder `403 Forbidden` fehl, wenn der spezielle Ordner nicht bereits vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="f5141-148">If your app has read-only permissions, the request to get a special folder or the children of a special folder may fail with a `404 Not Found` or a `403 Forbidden` error if the special folder does not already exist.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Access known folders in OneDrive through the special folder collection",
  "keywords": "known folders",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Special folders"
} -->
