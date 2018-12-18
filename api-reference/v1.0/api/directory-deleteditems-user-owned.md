---
title: Berechtigungen
description: 'Ruft eine Liste der kürzlich gelöschter Objekte Besitz des angegebenen Benutzers.  '
author: lleonard-msft
ms.openlocfilehash: 9ce487d957f4bdaa2684d00865aeac7ea293ad67
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351170"
---
# <a name="list-deleted-items-owned-by-a-user"></a><span data-ttu-id="bfd21-103">**Gelöschte Listenelemente Besitz eines Benutzers**</span><span class="sxs-lookup"><span data-stu-id="bfd21-103">**List deleted items owned by a user**</span></span>

<span data-ttu-id="bfd21-104">Ruft eine Liste der kürzlich gelöschter Objekte Besitz des angegebenen Benutzers.</span><span class="sxs-lookup"><span data-stu-id="bfd21-104">Retrieves a list of recently deleted items owned by the specified user.</span></span>  

<span data-ttu-id="bfd21-105">Liste gelöschter Elemente Funktionalität ist derzeit nur für Ressourcen der [Gruppe](../resources/group.md) Besitz des Benutzers unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bfd21-105">Currently, list deleted items functionality is supported only for [group](../resources/group.md) resources owned by the user.</span></span>

<span data-ttu-id="bfd21-106">Dies ist eine Service-Aktion, was bedeutet, dass es keine Paginierung unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bfd21-106">This is a service action, which means it does not support pagination.</span></span>  <span data-ttu-id="bfd21-107">Die API gibt bis zu 1.000 Gelöschte Objekte Besitz des Benutzers, sortiert nach ID zurück.</span><span class="sxs-lookup"><span data-stu-id="bfd21-107">The API returns up to 1,000 deleted objects owned by the user, sorted by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="bfd21-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bfd21-108">Permissions</span></span>

<span data-ttu-id="bfd21-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="bfd21-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

| <span data-ttu-id="bfd21-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bfd21-111">Permission type</span></span> | <span data-ttu-id="bfd21-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bfd21-112">Permissions (from least to most privileged)</span></span> |
| --- | --- |
| <span data-ttu-id="bfd21-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bfd21-113">Delegated (work or school account)</span></span> | <span data-ttu-id="bfd21-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfd21-114">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="bfd21-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bfd21-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="bfd21-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bfd21-116">Not supported.</span></span> |
| <span data-ttu-id="bfd21-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bfd21-117">Application</span></span> | <span data-ttu-id="bfd21-118">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfd21-118">Group.Read.All, Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="bfd21-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bfd21-119">HTTP request</span></span>

``` http
POST /directory/deletedItems/getUserOwnedObjects
```

## <a name="request-headers"></a><span data-ttu-id="bfd21-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bfd21-120">Request headers</span></span>

| <span data-ttu-id="bfd21-121">Name</span><span class="sxs-lookup"><span data-stu-id="bfd21-121">Name</span></span>          | <span data-ttu-id="bfd21-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bfd21-122">Description</span></span>               |
| ------------- | ------------------------- |
| <span data-ttu-id="bfd21-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bfd21-123">Authorization</span></span> | <span data-ttu-id="bfd21-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bfd21-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bfd21-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bfd21-126">Request body</span></span>

```json
{
  "userId":"{id}",
  "type":"Group"
}
```

<span data-ttu-id="bfd21-127">Textkörper der Anforderung erfordert die folgenden Parameter:</span><span class="sxs-lookup"><span data-stu-id="bfd21-127">The request body requires the following parameters:</span></span>

| <span data-ttu-id="bfd21-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="bfd21-128">Parameter</span></span>    | <span data-ttu-id="bfd21-129">Typ</span><span class="sxs-lookup"><span data-stu-id="bfd21-129">Type</span></span> |<span data-ttu-id="bfd21-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bfd21-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bfd21-131">userId</span><span class="sxs-lookup"><span data-stu-id="bfd21-131">userId</span></span>|<span data-ttu-id="bfd21-132">String</span><span class="sxs-lookup"><span data-stu-id="bfd21-132">String</span></span>|<span data-ttu-id="bfd21-133">ID des Besitzers.</span><span class="sxs-lookup"><span data-stu-id="bfd21-133">ID of the owner.</span></span>|
|<span data-ttu-id="bfd21-134">type</span><span class="sxs-lookup"><span data-stu-id="bfd21-134">type</span></span>|<span data-ttu-id="bfd21-135">String</span><span class="sxs-lookup"><span data-stu-id="bfd21-135">String</span></span>|<span data-ttu-id="bfd21-136">Art der Objekte zurückgegeben. `Group` ist derzeit der einzige unterstützte Wert.</span><span class="sxs-lookup"><span data-stu-id="bfd21-136">Type of owned objects to return; `Group` is currently the only supported value.</span></span>|


## <a name="response"></a><span data-ttu-id="bfd21-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="bfd21-137">Response</span></span>

<span data-ttu-id="bfd21-138">Zurückgeben der erfolgreiche Anforderungen `200 OK` Antwortcodes; Response-Objekt enthält die Eigenschaften des [Verzeichnisses (Gelöschte Objekte)](../resources/directory.md) .</span><span class="sxs-lookup"><span data-stu-id="bfd21-138">Successful requests return `200 OK` response codes; the response object includes [directory (deleted items)](../resources/directory.md) properties.</span></span>

## <a name="example"></a><span data-ttu-id="bfd21-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bfd21-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bfd21-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bfd21-140">Request</span></span>

<span data-ttu-id="bfd21-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bfd21-141">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/directory/deletedItems/getUserOwnedObjects
Content-type: application/json
```

``` json
{
  "userId":"55ac777c-109e-4022-b58c-470c8fcb6892",
  "type":"group"
}
```

###### <a name="response"></a><span data-ttu-id="bfd21-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="bfd21-142">Response</span></span>

<span data-ttu-id="bfd21-143">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bfd21-143">Here is an example of the response.</span></span> <span data-ttu-id="bfd21-144">Hinweis: Dieses Antwortobjekt der Kürze halber werden möglicherweise abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="bfd21-144">Note: This response object may be truncated for brevity.</span></span> <span data-ttu-id="bfd21-145">Alle unterstützte Eigenschaften werden von tatsächlichen Anrufe zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bfd21-145">All supported properties are returned from actual calls.</span></span>

``` http
HTTP/1.1 200
Content-type: application/json
Content-length: 1249

{
"value": [
          {
              "@odata.type": "#microsoft.graph.group",
              "id": "bfa7033a-7367-4644-85f5-95aaf385cbd7",
              "deletedDateTime": 2018-04-01T12:39:16Z,
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


