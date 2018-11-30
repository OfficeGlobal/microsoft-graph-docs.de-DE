---
title: Arbeiten mit SharePoint-Websites in Microsoft Graph
description: 'Die SharePoint-API in Microsoft Graph unterstützt die folgenden wesentlichen Szenarios:'
ms.openlocfilehash: e7150f5b437358b3ddb484640463b2f92d5416eb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064990"
---
# <a name="working-with-sharepoint-sites-in-microsoft-graph"></a><span data-ttu-id="21f0d-103">Arbeiten mit SharePoint-Websites in Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="21f0d-103">Working with SharePoint sites in Microsoft Graph</span></span>

<span data-ttu-id="21f0d-104">Die SharePoint-API in Microsoft Graph unterstützt die folgenden wesentlichen Szenarios:</span><span class="sxs-lookup"><span data-stu-id="21f0d-104">The SharePoint API in Microsoft Graph supports the following core scenarios:</span></span>

* <span data-ttu-id="21f0d-105">Zugriff auf SharePoint-**Websites**, **-Listen** und **-Laufwerke** (Dokumentbibliotheken)</span><span class="sxs-lookup"><span data-stu-id="21f0d-105">Access to SharePoint **sites**, **lists**, and **drives** (document libraries)</span></span>
* <span data-ttu-id="21f0d-106">Schreibgeschützte Unterstützung für **Website**-Ressourcen (keine Möglichkeit zum Erstellen neuer Websites)</span><span class="sxs-lookup"><span data-stu-id="21f0d-106">Read-only support for **site** resources (no ability to create new sites)</span></span>
* <span data-ttu-id="21f0d-107">Lese-/ Schreibzugriff-Unterstützung für **-Listen**, **listItems** und **driveItems**</span><span class="sxs-lookup"><span data-stu-id="21f0d-107">Read-write support for **lists**, **listItems**, and **driveItems**</span></span>
* <span data-ttu-id="21f0d-108">Adressierung von Ressourcen nach SharePoint-ID, URL oder relativem Pfad</span><span class="sxs-lookup"><span data-stu-id="21f0d-108">Address resources by SharePoint ID, URL, or relative path</span></span>

<span data-ttu-id="21f0d-109">Die SharePoint-API macht drei wichtige Ressourcentypen verfügbar:</span><span class="sxs-lookup"><span data-stu-id="21f0d-109">The SharePoint API exposes three major resource types:</span></span>

* <span data-ttu-id="21f0d-110">[Site](site.md) _ (Objekt auf oberster Ebene)_</span><span class="sxs-lookup"><span data-stu-id="21f0d-110">[Site](site.md) _(top-level object)_</span></span>
* [<span data-ttu-id="21f0d-111">List</span><span class="sxs-lookup"><span data-stu-id="21f0d-111">List</span></span>](list.md)
* [<span data-ttu-id="21f0d-112">ListItem</span><span class="sxs-lookup"><span data-stu-id="21f0d-112">ListItem</span></span>](listitem.md)

<span data-ttu-id="21f0d-113">Es folgt ein Beispiel für eine listItem-Ressource:</span><span class="sxs-lookup"><span data-stu-id="21f0d-113">The following is an example of a listItem resource.</span></span>

```json
{
  "fields": {
    "Title": "Access card",
    "Employee": "Ryan Gregg",
    "EmployeeId": "10",
    "CardSerial": "01235492",
    "Alias": "RGregg",
    "ID": 1,
    "ContentType": "Item",
    "Modified": "2016-09-19T23:15:25-07:00",
    "Created": "2016-09-19T23:15:25-07:00"
  },
  "createdBy": {
    "user": {
      "id": "b757fdcb-0271-4807-b243-504139e4ba04",
      "displayName": "Ryan Gregg"
    }
  },
  "createdDateTime": "2016-09-20T06:15:25Z",
  "eTag": "48e941c3-9515-4c48-9760-c07c90c79d48,1",
  "id": "4",
  "lastModifiedBy": {
    "user": {
      "id": "b757fdcb-0271-4807-b243-504139e4ba04",
      "displayName": "Ryan Gregg"
    }
  },
  "lastModifiedDateTime": "2016-09-20T06:15:25Z",
}
```

<span data-ttu-id="21f0d-114">Ressourcen legen Daten auf drei verschiedene Arten offen:</span><span class="sxs-lookup"><span data-stu-id="21f0d-114">Resources expose data in three different ways:</span></span>

* <span data-ttu-id="21f0d-115">_Eigenschaften_ (wie **id** und **name**) legen einfache Werte offen.</span><span class="sxs-lookup"><span data-stu-id="21f0d-115">_Properties_ (like **id** and **name**) expose simple values.</span></span>
* <span data-ttu-id="21f0d-116">_Facets_ (wie **fields** und **createdBy**) legen komplexe Werte offen.</span><span class="sxs-lookup"><span data-stu-id="21f0d-116">_Facets_ (like **fields** and **createdBy**) expose complex values.</span></span>
* <span data-ttu-id="21f0d-117">_References_ (wie **items**) verweisen auf Sammlungen anderer Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="21f0d-117">_References_ (like **items**) point to collections of other resources.</span></span>

<span data-ttu-id="21f0d-118">Sie können Sie Referenzen in der URL mit dem _expand_-Abfrageparameter erweitern, z. B. `?expand=fields`.</span><span class="sxs-lookup"><span data-stu-id="21f0d-118">You can expand references in your URL with the _expand_ query parameter; for example, `?expand=fields`.</span></span>
<span data-ttu-id="21f0d-119">Sie können bestimmte Eigenschaften und Facets mit dem _select_ Abfrageparameter abrufen, z. B. `?select=id,name`.</span><span class="sxs-lookup"><span data-stu-id="21f0d-119">You can request specific properties and facets with the _select_ query parameter; for example, `?select=id,name`.</span></span>
<span data-ttu-id="21f0d-120">Standardmäßig werden die meisten Eigenschaften und Facets zurückgegeben, wohingegen alle Referenzen ausgeblendet werden.</span><span class="sxs-lookup"><span data-stu-id="21f0d-120">By default, most properties and facets are returned while all references are hidden.</span></span>
<span data-ttu-id="21f0d-121">Aus Leistungsgründen wird empfohlen, dass Sie _select_ und _expand_ nur für die Daten angeben, an denen Sie interessiert sind.</span><span class="sxs-lookup"><span data-stu-id="21f0d-121">For efficiency, we recommend that you specify _select_ and _expand_ to only return the data you care about.</span></span>

## <a name="sharepoint-api-root-resources"></a><span data-ttu-id="21f0d-122">SharePoint-API-Stammressourcen</span><span class="sxs-lookup"><span data-stu-id="21f0d-122">SharePoint API root resources</span></span>

<span data-ttu-id="21f0d-123">Die folgenden Beispiele sind relativ zu `https://graph.microsoft.com/beta`.</span><span class="sxs-lookup"><span data-stu-id="21f0d-123">The following examples are relative to `https://graph.microsoft.com/beta`.</span></span>

| <span data-ttu-id="21f0d-124">Pfad</span><span class="sxs-lookup"><span data-stu-id="21f0d-124">Path</span></span>                                   | <span data-ttu-id="21f0d-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="21f0d-125">Description</span></span>
|:---------------------------------------|:------------------------------------
| <span data-ttu-id="21f0d-126">/sites/root</span><span class="sxs-lookup"><span data-stu-id="21f0d-126">/sites/root</span></span>                            | <span data-ttu-id="21f0d-127">Standardmäßige [Website][] der Organisation</span><span class="sxs-lookup"><span data-stu-id="21f0d-127">Organization's default [site][].</span></span>
| <span data-ttu-id="21f0d-128">/sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="21f0d-128">/sites/{site-id}</span></span>                       | <span data-ttu-id="21f0d-129">Zugriff auf eine bestimmte [Website][] anhand ihrer ID</span><span class="sxs-lookup"><span data-stu-id="21f0d-129">Access a specific [site][] by its ID.</span></span>
| <span data-ttu-id="21f0d-130">/sites/{site-id}/drive</span><span class="sxs-lookup"><span data-stu-id="21f0d-130">/sites/{site-id}/drive</span></span>                 | <span data-ttu-id="21f0d-131">Zugriff auf das standardmäßige [Laufwerk](drive.md) (Dokumentbibliothek) für die angegebene [Website][]</span><span class="sxs-lookup"><span data-stu-id="21f0d-131">Access the default [drive](drive.md) (document library) for the given [site][].</span></span>
| <span data-ttu-id="21f0d-132">/sites/{site-id}/drives</span><span class="sxs-lookup"><span data-stu-id="21f0d-132">/sites/{site-id}/drives</span></span>                | <span data-ttu-id="21f0d-133">Aufzählung der [Laufwerke](drive.md) (Dokumentbibliotheken) unter der [Website][]</span><span class="sxs-lookup"><span data-stu-id="21f0d-133">Enumerate the [drives](drive.md) (document libraries) under the [site][].</span></span>
| <span data-ttu-id="21f0d-134">/sites/{site-id}/sites</span><span class="sxs-lookup"><span data-stu-id="21f0d-134">/sites/{site-id}/sites</span></span>                 | <span data-ttu-id="21f0d-135">Aufzählung der Unterwebsites unter der [site][]</span><span class="sxs-lookup"><span data-stu-id="21f0d-135">Enumerate the sub-sites under the [site][].</span></span>
| <span data-ttu-id="21f0d-136">/sites/{site-id}/lists</span><span class="sxs-lookup"><span data-stu-id="21f0d-136">/sites/{site-id}/lists</span></span>                 | <span data-ttu-id="21f0d-137">Aufzählung der [lists](list.md) unter der [site](site.md)</span><span class="sxs-lookup"><span data-stu-id="21f0d-137">Enumerate the [lists](list.md) under the [site](site.md).</span></span>
| <span data-ttu-id="21f0d-138">/sites/{site-id}/lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="21f0d-138">/sites/{site-id}/lists/{list-id}/items</span></span> | <span data-ttu-id="21f0d-139">Aufzählung der [listItems](listitem.md) unter der [list](list.md)</span><span class="sxs-lookup"><span data-stu-id="21f0d-139">Enumerate the [listItems](listitem.md) under the [list](list.md).</span></span>
| <span data-ttu-id="21f0d-140">/groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="21f0d-140">/groups/{group-id}/sites/root</span></span>          | <span data-ttu-id="21f0d-141">Zugriff auf die Teamweb[site][] einer Gruppe</span><span class="sxs-lookup"><span data-stu-id="21f0d-141">Access a group's team [site][].</span></span>

<span data-ttu-id="21f0d-p102">Websites können auch anhand des Pfads adressiert werden, indem der SharePoint-Hostname gefolgt von einem Doppelpunkt und dem relativen Pfad zur Website verwendet wird. Sie können optional wieder zur Adressierung des Ressourcenmodells übergehen, indem Sie einen Doppelpunkt am Ende einfügen.</span><span class="sxs-lookup"><span data-stu-id="21f0d-p102">Sites can also be addressed by path by using the SharePoint hostname, followed by a colon and the relative path to the site. You can optionally transition back to addressing the resource model by putting another colon at the end.</span></span>

| <span data-ttu-id="21f0d-144">Pfad</span><span class="sxs-lookup"><span data-stu-id="21f0d-144">Path</span></span>                                           | <span data-ttu-id="21f0d-145">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="21f0d-145">Description</span></span>
|:-----------------------------------------------|:-----------------------------------
| <span data-ttu-id="21f0d-146">/sites/contoso.sharepoint.com:/teams/hr</span><span class="sxs-lookup"><span data-stu-id="21f0d-146">/sites/contoso.sharepoint.com:/teams/hr</span></span>        | <span data-ttu-id="21f0d-147">Die Website zugeordnethttps://contoso.sharepoint.com/teams/hr</span><span class="sxs-lookup"><span data-stu-id="21f0d-147">The site associated with https://contoso.sharepoint.com/teams/hr</span></span>
| <span data-ttu-id="21f0d-148">/sites/contoso.sharepoint.com:/teams/hr:/drive</span><span class="sxs-lookup"><span data-stu-id="21f0d-148">/sites/contoso.sharepoint.com:/teams/hr:/drive</span></span> | <span data-ttu-id="21f0d-149">Zugriff auf das standardmäßige [Laufwerk](drive.md) für diese Website</span><span class="sxs-lookup"><span data-stu-id="21f0d-149">Access the default [drive](drive.md) for this site.</span></span>

## <a name="note-for-existing-sharepoint-developers"></a><span data-ttu-id="21f0d-150">Hinweis für bestehende SharePoint-Entwickler</span><span class="sxs-lookup"><span data-stu-id="21f0d-150">Note for existing SharePoint developers</span></span>

<span data-ttu-id="21f0d-p103">Zwischen der Microsoft Graph-SharePoint-API und den CSOM-APIs bestehen einige wesentliche Unterschiede. Die [site][]-Ressource ist `SPWeb` zugeordnet. Die Stammweb[site][] (`SPWeb`) in einer Websitesammlung verfügt über ein [siteCollection](sitecollection.md)-Facet, das Informationen über `SPSite` enthält. Da IDs für Websites nur innerhalb einer Websitesammlung eindeutig sind, müssen zur Adressierung einer Website nach ID sowohl die Websitesammlungs-ID als auch die Website-ID angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="21f0d-p103">The Microsoft Graph SharePoint API has a few key differences with the CSOM APIs. The [site][] resource maps to `SPWeb`. The root [site][] (`SPWeb`) in a site collection has a [siteCollection](sitecollection.md) facet, which contains information about the `SPSite`. Because IDs for sites are only unique within their site collection, addressing a site by ID requires providing both the site collection identifier and the site identifier.</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{hostname},{spsite-id},{spweb-id}/
```
<span data-ttu-id="21f0d-155">Eine URL, die nur mit dem Hostnamen gebildet wird, verweist auf die Stammwebsite (`SPWeb`) in der Standard-Websitesammlung.</span><span class="sxs-lookup"><span data-stu-id="21f0d-155">A URL constructed with only the hostname will point to the root site (`SPWeb`) in the default site collection.</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{hostname}
```

<span data-ttu-id="21f0d-156">Eine URL, die nur mit dem Hostnamen und der Websitesammlungs-ID (`SPSite`) gebildet wird, verweist auf die Stammwebsite (`SPWeb`) in der angegebenen Websitesammlung.</span><span class="sxs-lookup"><span data-stu-id="21f0d-156">A URL constructed with only the hostname and siteCollection (`SPSite`) ID will point to the root site (`SPWeb`) in the given site collection.</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{hostname},{spsite-id}
```

[site]: site.md
[list]: list.md
[drive]: drive.md
[siteCollection]: sitecollection.md

<!-- {
  "type": "#page.annotation",
  "description": "Getting started programming with the SharePoint API",
  "keywords": "getting started sharepoint rest api programming C# ios android rest http",
  "section": "documentation",
  "tocPath": "Getting Started",
  "tocIndex": -100
} -->
