---
title: Arbeiten mit Dateien in Microsoft Graph
description: Microsoft Graph können Sie eine app erstellen, die mit Dateien über OneDrive, OneDrive für Unternehmen und SharePoint-Dokumentbibliotheken stellt eine Verbindung her.
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 89798778fff0297ffce607d1546a177dd90d357e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918021"
---
# <a name="working-with-files-in-microsoft-graph"></a><span data-ttu-id="68691-103">Arbeiten mit Dateien in Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="68691-103">Working with files in Microsoft Graph</span></span>

<span data-ttu-id="68691-104">Microsoft Graph können Sie eine app erstellen, die mit Dateien über OneDrive, OneDrive für Unternehmen und SharePoint-Dokumentbibliotheken stellt eine Verbindung her.</span><span class="sxs-lookup"><span data-stu-id="68691-104">You can use Microsoft Graph to create an app that connects with files across OneDrive, OneDrive for Business, and SharePoint document libraries.</span></span>
<span data-ttu-id="68691-105">Mit Microsoft Graph können Sie eine Vielzahl von Erfahrungen mit Dateien, die Sie in Office 365 einfach Speichern von Benutzerdokumenten für komplexe Dateifreigabe Szenarien erstellen.</span><span class="sxs-lookup"><span data-stu-id="68691-105">With Microsoft Graph, you can build a variety of experiences with files stored in Office 365, from simply storing user documents to complex file-sharing scenarios.</span></span>

<span data-ttu-id="68691-106">Microsoft Graph legt zwei Ressourcentypen für die Arbeit mit Dateien Offen:</span><span class="sxs-lookup"><span data-stu-id="68691-106">Microsoft Graph exposes two resource types for working with files:</span></span>

* <span data-ttu-id="68691-107">[Drive](drive.md): Stellt einen logischen Container von Dateien wie z. B. eine Dokumentbibliothek oder OneDrive eines Benutzers dar.</span><span class="sxs-lookup"><span data-stu-id="68691-107">[Drive](drive.md) - Represents a logical container of files, like a document library or a user's OneDrive.</span></span>
* <span data-ttu-id="68691-108">[DriveItem](driveitem.md): Stellt ein Element innerhalb eines Laufwerks dar, wie z. B. ein Dokument, ein Foto, ein Video oder einen Ordner.</span><span class="sxs-lookup"><span data-stu-id="68691-108">[DriveItem](driveitem.md) - Represents an item within a drive, like a document, photo, video, or folder.</span></span>

<span data-ttu-id="68691-p102">Die meisten Interaktionen mit Dateien finden über Interaktionen mit **DriveItem**-Ressourcen statt. Es folgt ein Beispiel für eine DriveItem-Ressource:</span><span class="sxs-lookup"><span data-stu-id="68691-p102">Most of the interaction with files occurs through interaction with **DriveItem** resources. The following is an example of a DriveItem resource:</span></span>

```json
{
  "@content.downloadUrl":"https://public-sn3302.files.1drv.com/y2pcT7OaUEExF7EHOlpTjCE55mIUoiX7H3sx1ff6I-nP35XUTBqZlnkh9FJhWb_pf9sZ7LEpEchvDznIbQig0hWBeidpwFkOqSKCwQylisarN6T0ecAeMvantizBUzM2PA1",
  "createdDateTime": "2016-09-16T03:37:04.72Z",
  "cTag": "aYzpENDY0OEYwNkM5MUQ5RDNEITU0OTI3LjI1Ng",
  "eTag": "aRDQ2NDhGMDZDOTFEOUQzRCE1NDkyNy4w",
  "id":"D4648F06C91D9D3D!54927",
  "lastModifiedBy": {
    "user": {
      "displayName": "Daron Spektor",
      "id": "d4648f06c91d9d3d"
    }
  },
  "name":"BritishShorthair.jpg",
  "size":35212,
  "image":{
    "height":398,
    "width":273
  },
  "file": {
    "hashes":{
      "sha1Hash":"wmgPQ6jrSeMX7JP1XmstQEGM2fc="
    }
  }
}
```

<span data-ttu-id="68691-111">**Drive**- und **DriveItem**-Ressourcen legen Daten auf drei verschiedene Arten offen:</span><span class="sxs-lookup"><span data-stu-id="68691-111">**Drive** and **DriveItem** resources expose data in three different ways:</span></span>

* <span data-ttu-id="68691-112">_Eigenschaften_ (wie **id** und **name**) legen einfache Werte (Zeichenfolgen, Zahlen, boolesche Werte) offen.</span><span class="sxs-lookup"><span data-stu-id="68691-112">_Properties_ (like **id** and **name**) expose simple values (strings, numbers, Booleans).</span></span>
* <span data-ttu-id="68691-p103">_Facets_ (wie **file** und **photo**) legen komplexe Werte offen. Vorhandene **file**- oder **folder**-Facets geben Verhaltensweisen und Eigenschaften eines **DriveItem** an.</span><span class="sxs-lookup"><span data-stu-id="68691-p103">_Facets_ (like **file** and **photo**) expose complex values. The presence of **file** or **folder** facets indicates behaviors and properties of a **DriveItem**.</span></span>
* <span data-ttu-id="68691-115">_Referenzen_ (wie **children** und **thumbnails**) verweisen auf Sammlungen anderer Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="68691-115">_References_ (like **children** and **thumbnails**) point to collections of other resources.</span></span>

## <a name="commonly-accessed-resources"></a><span data-ttu-id="68691-116">Häufig verwendete Ressourcen</span><span class="sxs-lookup"><span data-stu-id="68691-116">Commonly accessed resources</span></span>

<span data-ttu-id="68691-117">Die meisten API-Anforderungen für Dateiinteraktionen verwenden eine der folgenden grundlegenden Ressourcen für den Zugriff auf **Drive** oder **DriveItem**.</span><span class="sxs-lookup"><span data-stu-id="68691-117">Most API requests for file interactions will use one of these base resources to access a **Drive** or **DriveItem**.</span></span>

| <span data-ttu-id="68691-118">Pfad</span><span class="sxs-lookup"><span data-stu-id="68691-118">Path</span></span>                               | <span data-ttu-id="68691-119">Ressource</span><span class="sxs-lookup"><span data-stu-id="68691-119">Resource</span></span>
|------------------------------------|-----------------------------------------
| `/me/drive`                        | <span data-ttu-id="68691-120">OneDrive eines Benutzers</span><span class="sxs-lookup"><span data-stu-id="68691-120">User's OneDrive</span></span>
| `/me/drives`                       | <span data-ttu-id="68691-121">Listet die für den Benutzer verfügbaren OneDrive-Ressourcen auf.</span><span class="sxs-lookup"><span data-stu-id="68691-121">Enumerate OneDrive resources available to the user.</span></span>
| `/drives/{drive-id}`               | <span data-ttu-id="68691-122">Greift auf ein bestimmtes **Drive** über die Laufwerks-ID zu.</span><span class="sxs-lookup"><span data-stu-id="68691-122">Access a specific **Drive** by the drive's ID.</span></span>
| `/drives/{drive-id}/root/children` | <span data-ttu-id="68691-123">Listet die **DriveItem**-Ressourcen in der Root eines spezifischen **Drive** auf.</span><span class="sxs-lookup"><span data-stu-id="68691-123">Enumerate the **DriveItem** resources in the root of a specific **Drive**.</span></span>
| `/me/drive/items/{item-id}`        | <span data-ttu-id="68691-124">Greift auf ein **DriveItem** auf dem OneDrive des Benutzers über die eindeutige ID zu.</span><span class="sxs-lookup"><span data-stu-id="68691-124">Access a **DriveItem** in the user's OneDrive by its unique ID.</span></span>
| `/me/drive/special/{special-id}`   | <span data-ttu-id="68691-125">Greift auf einen bestimmten (benannten) Ordner auf dem OneDrive des Benutzers über seinen bekannten Namen zu.</span><span class="sxs-lookup"><span data-stu-id="68691-125">Access a special (named) folder in the user's OneDrive by its known name.</span></span>
| `/users/{user-id}/drive`           | <span data-ttu-id="68691-126">Greift auf das OneDrive eines anderen Benutzers mithilfe der eindeutigen ID des Benutzers zu.</span><span class="sxs-lookup"><span data-stu-id="68691-126">Access another user's OneDrive by using the user's unique ID.</span></span>
| `/groups/{group-id}/drive`         | <span data-ttu-id="68691-127">Greift auf die Standarddokumentbibliothek für eine Gruppe mithilfe der eindeutigen ID der Gruppe zu.</span><span class="sxs-lookup"><span data-stu-id="68691-127">Access the default document library for a group by the group's unique ID.</span></span>
| `/shares/{share-id}`               | <span data-ttu-id="68691-128">Greift auf ein **DriveItem** über seine **SharedId** oder eine Freigabe-URL zu.</span><span class="sxs-lookup"><span data-stu-id="68691-128">Access a **DriveItem** by its **sharedId** or sharing URL.</span></span>
| `/sites/{site-id}/drive`           | <span data-ttu-id="68691-129">Zugriff auf die Standardeinstellung **Laufwerk** (Dokumentbibliothek) für die angegebene [SharePoint][] - [Website][]</span><span class="sxs-lookup"><span data-stu-id="68691-129">Access the default **Drive** (document library) for the given [SharePoint][] [site][]</span></span>
| `/sites/{site-id}/drives`          | <span data-ttu-id="68691-130">Auflisten der **Laufwerke** (Dokumentbibliotheken) unter der angegebenen [SharePoint][] - [Website][]</span><span class="sxs-lookup"><span data-stu-id="68691-130">Enumerate the **Drives** (document libraries) under the given [SharePoint][] [site][]</span></span>

<span data-ttu-id="68691-p104">Zusätzlich zur Adressierung eines **DriveItem** innerhalb eines **Drive** durch eine eindeutige ID kann die App ein **DriveItem** auch über einen relativen Pfad von einer bekannten Ressource adressieren. Zur Adressierung über einen Pfad wird das Doppelpunktzeichen (`:`) für das Escape des relativen Pfads verwendet. Diese Tabelle enthält ein Beispiel für unterschiedliche Methoden für die Verwendung des Doppelpunkts zur Adressierung eines Elements nach Pfad.</span><span class="sxs-lookup"><span data-stu-id="68691-p104">In addition to addressing a **DriveItem** within a **Drive** by unique ID, your app can also address a **DriveItem** by relative path from a known resource. To address using a path, the colon (`:`) character is used to escape the relative path. This table provides an example of different ways to use the colon character to address an item by path.</span></span>

| <span data-ttu-id="68691-134">Pfad</span><span class="sxs-lookup"><span data-stu-id="68691-134">Path</span></span> | <span data-ttu-id="68691-135">Ressource</span><span class="sxs-lookup"><span data-stu-id="68691-135">Resource</span></span> |
|---|---|
| `/me/drive/root:/path/to/file` | <span data-ttu-id="68691-136">Greift auf ein **DriveItem** über den Pfad relativ zum OneDrive-Stammordner des Benutzers zu.</span><span class="sxs-lookup"><span data-stu-id="68691-136">Access a **DriveItem** by path relative to the user's OneDrive root folder.</span></span> |
| `/me/drive/items/{item-id}:/path/to/file` | <span data-ttu-id="68691-137">Greift auf ein **DriveItem** über einen Pfad relativ zu einem anderen Element zu (einem **DriveItem** mit einem **folder**-Facet).</span><span class="sxs-lookup"><span data-stu-id="68691-137">Access a **DriveItem** by path relative to another item (a **DriveItem** with a **folder** facet).</span></span> |
| `/me/drive/root:/path/to/folder:/children` | <span data-ttu-id="68691-138">Listet die untergeordneten Elemente eines **DriveItem** über einen Pfad relativ zum Stammordner des OneDrive des Benutzers auf.</span><span class="sxs-lookup"><span data-stu-id="68691-138">List the children of a **DriveItem** by path relative to the root of the user's OneDrive.</span></span> |
| `/me/drive/items/{item-id}:/path/to/folder:/children` | <span data-ttu-id="68691-139">Listet die untergeordneten Elemente eines **DriveItem** über einen Pfad relativ zu einem anderen Element auf.</span><span class="sxs-lookup"><span data-stu-id="68691-139">List the children of a **DriveItem** by path relative to another item.</span></span> |

## <a name="drive-resource"></a><span data-ttu-id="68691-140">Drive-Ressource</span><span class="sxs-lookup"><span data-stu-id="68691-140">Drive resource</span></span>

<span data-ttu-id="68691-141">[Laufwerk Ressource](drive.md) ist das Objekt der obersten Ebene innerhalb eines Benutzers OneDrive oder einer [SharePoint][] -Dokumentbibliothek.</span><span class="sxs-lookup"><span data-stu-id="68691-141">The [Drive resource](drive.md) is the top-level object within a user's OneDrive or a [SharePoint][] document library.</span></span>
<span data-ttu-id="68691-142">Fast alle Dateivorgänge beginnen damit, dass eine bestimmte Drive-Ressource  adressiert wird.</span><span class="sxs-lookup"><span data-stu-id="68691-142">Nearly all files operations will start by addressing a specific drive resource.</span></span>

<span data-ttu-id="68691-143">Eine Drive-Ressource kann entweder von der eindeutigen ID des Laufwerks oder von dem Standardlaufwerk eines [Benutzers](user.md), einer [Gruppe](group.md), oder einer Organisation adressiert werden.</span><span class="sxs-lookup"><span data-stu-id="68691-143">A drive resource can be addressed either by the drive's unique ID or by the default drive for a [User](user.md), [Group](group.md), or organization.</span></span> 

## <a name="driveitem-resource"></a><span data-ttu-id="68691-144">DriveItem-Ressource</span><span class="sxs-lookup"><span data-stu-id="68691-144">DriveItem resource</span></span>

<span data-ttu-id="68691-p106">[DriveItems](driveitem.md) sind die Objekte innerhalb des Laufwerks-Dateisystems. Der Zugriff darauf erfolgt über ihre **id** unter Verwendung der `/items/{item-id}`-Syntax oder den Dateisystempfad unter Verwendung der`/root:/path/to/item/`-Syntax.</span><span class="sxs-lookup"><span data-stu-id="68691-p106">[DriveItems](driveitem.md) are the objects inside a drive's file system. They can be accessed by their **id** by using `/items/{item-id}` syntax, or by their file system path using the `/root:/path/to/item/` syntax.</span></span>

<span data-ttu-id="68691-147">DriveItems verfügen _Facets_, die Daten zu den Identitäten und Funktionen der Elemente bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="68691-147">DriveItems have _facets_ that provide data about the item's identity and capabilities.</span></span>

<span data-ttu-id="68691-148">DriveItems mit einem **folder**-Facet fungieren als Container von Elementen und enthalten einen **children**-Verweis, der auf eine Sammlung von Elementen unter dem Ordner zeigt.</span><span class="sxs-lookup"><span data-stu-id="68691-148">DriveItems with a **folder** facet act as containers of items, and have a **children** reference, which points to a collection of items under the folder.</span></span>

## <a name="shared-folders-and-remote-items"></a><span data-ttu-id="68691-149">Freigegebene Ordner und Remoteelemente</span><span class="sxs-lookup"><span data-stu-id="68691-149">Shared folders and remote items</span></span>

<span data-ttu-id="68691-p107">Persönliche OneDrive-Benutzer können ein oder mehrere freigegebene Elemente von einem anderen Laufwerk zu ihrem eigenen OneDrive hinzufügen. Diese freigegebenen Elemente werden als **DriveItem** in der **children**-Sammlung mit einem [remoteItem](remoteitem.md)-Facet angezeigt.</span><span class="sxs-lookup"><span data-stu-id="68691-p107">OneDrive personal users can add one or more shared items from another drive to their own OneDrive. These shared items appear as a **DriveItem** in the **children** collection with a [remoteItem](remoteitem.md) facet.</span></span>

<span data-ttu-id="68691-152">Weitere Informationen zum Arbeiten mit freigegebenen Ordnern und Remoteelementen finden Sie unter [Remoteelemente und freigegebene Ordner](remoteitem.md).</span><span class="sxs-lookup"><span data-stu-id="68691-152">For more information about working with shared folders and remote items, see [Remote items and shared folders](remoteitem.md).</span></span>   

## <a name="sharing-and-permissions"></a><span data-ttu-id="68691-153">Freigabe und Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="68691-153">Sharing and permissions</span></span>

<span data-ttu-id="68691-p108">Eine der am häufigsten verwendeten Aktionen für OneDrive und SharePoint-Dokumentbibliotheken besteht im Freigeben von Inhalten für andere Personen. Über Microsoft Graph kann Ihre App [Freigabelinks](../api/driveitem-createlink.md) erstellen, [Genehmigungen hinzufügen und Einladungen an Elemente eines Laufwerks senden](../api/driveitem-invite.md).</span><span class="sxs-lookup"><span data-stu-id="68691-p108">One of the most common actions for OneDrive and SharePoint document libraries is sharing content with other people. Microsoft Graph allows your app to create [sharing links](../api/driveitem-createlink.md), [add permissions and send invitations](../api/driveitem-invite.md) to items in a drive.</span></span>

<span data-ttu-id="68691-156">Microsoft Graph bietet der App auch eine Möglichkeit, [Zugriff auf freigegebene Inhalte](../api/shares-get.md) direkt über einen Freigabelinks zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="68691-156">Microsoft Graph also provides a way for your app to [access shared content](../api/shares-get.md) directly from a sharing link.</span></span>

[SharePoint]: sharepoint.md
[site]: site.md
