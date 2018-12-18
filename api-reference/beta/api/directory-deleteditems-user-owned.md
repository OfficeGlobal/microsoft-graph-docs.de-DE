---
title: Berechtigungen
description: 'Ruft eine Liste der kürzlich gelöschter Objekte Besitz des angegebenen Benutzers.  '
author: lleonard-msft
ms.openlocfilehash: 5363adb943ac8c240e0f168246f7d17b3addf086
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348482"
---
# <a name="list-deleted-items-owned-by-a-user"></a><span data-ttu-id="5ae75-103">**Gelöschte Listenelemente Besitz eines Benutzers**</span><span class="sxs-lookup"><span data-stu-id="5ae75-103">**List deleted items owned by a user**</span></span>

<span data-ttu-id="5ae75-104">Ruft eine Liste der kürzlich gelöschter Objekte Besitz des angegebenen Benutzers.</span><span class="sxs-lookup"><span data-stu-id="5ae75-104">Retrieves a list of recently deleted items owned by the specified user.</span></span>  

<span data-ttu-id="5ae75-105">Liste gelöschter Elemente Funktionalität ist derzeit nur für Ressourcen der [Gruppe](../resources/group.md) Besitz des Benutzers unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5ae75-105">Currently, list deleted items functionality is supported only for [group](../resources/group.md) resources owned by the user.</span></span>

<span data-ttu-id="5ae75-106">Dies ist eine Service-Aktion, was bedeutet, dass es keine Paginierung unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5ae75-106">This is a service action, which means it does not support pagination.</span></span>  <span data-ttu-id="5ae75-107">Die API gibt bis zu 1.000 Gelöschte Objekte Besitz des Benutzers, sortiert nach ID zurück.</span><span class="sxs-lookup"><span data-stu-id="5ae75-107">The API returns up to 1,000 deleted objects owned by the user, sorted by ID.</span></span>  <span data-ttu-id="5ae75-108">Sollte der Benutzer der Besitzer 1.000 oder mehr Gelöschte Objekte, die API gibt Nothing zurück.</span><span class="sxs-lookup"><span data-stu-id="5ae75-108">Should the user own 1,000 or more deleted objects, the API returns nothing.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ae75-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5ae75-109">Permissions</span></span>

<span data-ttu-id="5ae75-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="5ae75-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

| <span data-ttu-id="5ae75-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5ae75-112">Permission type</span></span> | <span data-ttu-id="5ae75-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5ae75-113">Permissions (from least to most privileged)</span></span> |
| --- | --- |
| <span data-ttu-id="5ae75-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5ae75-114">Delegated (work or school account)</span></span> | <span data-ttu-id="5ae75-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ae75-115">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="5ae75-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5ae75-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="5ae75-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5ae75-117">Not supported.</span></span> |
| <span data-ttu-id="5ae75-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5ae75-118">Application</span></span> | <span data-ttu-id="5ae75-119">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ae75-119">Group.Read.All, Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="5ae75-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5ae75-120">HTTP request</span></span>

``` http
POST /directory/deletedItems/getUserOwnedObjects
```

## <a name="request-headers"></a><span data-ttu-id="5ae75-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5ae75-121">Request headers</span></span>

| <span data-ttu-id="5ae75-122">**Name**</span><span class="sxs-lookup"><span data-stu-id="5ae75-122">**Name**</span></span>      | <span data-ttu-id="5ae75-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="5ae75-123">**Description**</span></span>           |
| ------------- | ------------------------- |
| <span data-ttu-id="5ae75-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ae75-124">Authorization</span></span> | <span data-ttu-id="5ae75-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5ae75-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5ae75-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5ae75-127">Request body</span></span>

```json
{
  "userId":"55ac777c-109e-4022-b58c-470c8fcb6892",
  "type":"group"
}
```

<span data-ttu-id="5ae75-128">Textkörper der Anforderung erfordert die folgenden Parameter:</span><span class="sxs-lookup"><span data-stu-id="5ae75-128">The request body requires the following parameters:</span></span>

| <span data-ttu-id="5ae75-129">Parameter</span><span class="sxs-lookup"><span data-stu-id="5ae75-129">Parameter</span></span>    | <span data-ttu-id="5ae75-130">Typ</span><span class="sxs-lookup"><span data-stu-id="5ae75-130">Type</span></span> |<span data-ttu-id="5ae75-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5ae75-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5ae75-132">userId</span><span class="sxs-lookup"><span data-stu-id="5ae75-132">userId</span></span>|<span data-ttu-id="5ae75-133">String</span><span class="sxs-lookup"><span data-stu-id="5ae75-133">String</span></span>|<span data-ttu-id="5ae75-134">ID des Besitzers.</span><span class="sxs-lookup"><span data-stu-id="5ae75-134">ID of the owner.</span></span>|
|<span data-ttu-id="5ae75-135">type</span><span class="sxs-lookup"><span data-stu-id="5ae75-135">type</span></span>|<span data-ttu-id="5ae75-136">String</span><span class="sxs-lookup"><span data-stu-id="5ae75-136">String</span></span>|<span data-ttu-id="5ae75-137">Art der Objekte zurückgegeben. `Group` ist derzeit der einzige unterstützte Wert.</span><span class="sxs-lookup"><span data-stu-id="5ae75-137">Type of owned objects to return; `Group` is currently the only supported value.</span></span>|

## <a name="response"></a><span data-ttu-id="5ae75-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="5ae75-138">Response</span></span>

<span data-ttu-id="5ae75-139">Zurückgeben der erfolgreiche Anforderungen `200 OK` Antwortcodes; Response-Objekt enthält die Eigenschaften des [Verzeichnisses (Gelöschte Objekte)](../resources/directory.md) .</span><span class="sxs-lookup"><span data-stu-id="5ae75-139">Successful requests return `200 OK` response codes; the response object includes [directory (deleted items)](../resources/directory.md) properties.</span></span>

## <a name="example"></a><span data-ttu-id="5ae75-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5ae75-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5ae75-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5ae75-141">Request</span></span>

<span data-ttu-id="5ae75-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5ae75-142">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/directory/deletedItems/getUserOwnedObjects
Content-type: application/json
```

``` json
{
  "userId":"55ac777c-109e-4022-b58c-470c8fcb6892",
  "type":"Group"
}
```

###### <a name="response"></a><span data-ttu-id="5ae75-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="5ae75-143">Response</span></span>

<span data-ttu-id="5ae75-144">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5ae75-144">Here is an example of the response.</span></span> <span data-ttu-id="5ae75-145">Hinweis: Dieses Antwortobjekt der Kürze halber werden möglicherweise abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="5ae75-145">Note: This response object may be truncated for brevity.</span></span> <span data-ttu-id="5ae75-146">Alle unterstützte Eigenschaften werden von tatsächlichen Anrufe zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5ae75-146">All supported properties are returned from actual calls.</span></span>

``` http
HTTP/1.1 200
Content-type: application/json
Content-length: 1249

{
"value": [
          {
              "@odata.type": "#microsoft.graph.group",
              "id": "bfa7033a-7367-4644-85f5-95aaf385cbd7",
              "deletedDateTime": "2018-04-01T12:34:56Z",
              "classification": null,
              "createdDateTime": "2017-03-22T12:39:16Z",
              "description": null,
              "displayName": "Test",
              "groupTypes": [
                  "Unified"
              ],
              "mail": "Test@contoso.com",
              "mailEnabled": true,
              "mailNickname": "Test",
              "membershipRule": null,
              "membershipRuleProcessingState": null,
              "preferredDataLocation": null,
              "preferredLanguage": null,
              "proxyAddresses": [
                  "SMTP:Test@contoso.com"
              ],
              "renewedDateTime": "2017-09-22T22:30:39Z",
              "securityEnabled": false,
              "theme": null,
              "visibility": "Public"
          } 
        ]
 }
```


