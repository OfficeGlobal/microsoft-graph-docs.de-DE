---
title: Berechtigungen
description: 'Ruft eine Liste der kürzlich gelöschter Objekte Besitz des angegebenen Benutzers.  '
ms.openlocfilehash: affdd67d48056c4459e651fd5c64168d8356abe8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016578"
---
# <a name="list-deleted-items-owned-by-a-user"></a><span data-ttu-id="dd357-103">**Gelöschte Listenelemente Besitz eines Benutzers**</span><span class="sxs-lookup"><span data-stu-id="dd357-103">**List deleted items owned by a user**</span></span>

<span data-ttu-id="dd357-104">Ruft eine Liste der kürzlich gelöschter Objekte Besitz des angegebenen Benutzers.</span><span class="sxs-lookup"><span data-stu-id="dd357-104">Retrieves a list of recently deleted items owned by the specified user.</span></span>  

<span data-ttu-id="dd357-105">Liste gelöschter Elemente Funktionalität ist derzeit nur für Ressourcen der [Gruppe](../resources/group.md) Besitz des Benutzers unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dd357-105">Currently, list deleted items functionality is supported only for [group](../resources/group.md) resources owned by the user.</span></span>

<span data-ttu-id="dd357-106">Dies ist eine Service-Aktion, was bedeutet, dass es keine Paginierung unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dd357-106">This is a service action, which means it does not support pagination.</span></span>  <span data-ttu-id="dd357-107">Die API gibt bis zu 1.000 Gelöschte Objekte Besitz des Benutzers, sortiert nach ID zurück.</span><span class="sxs-lookup"><span data-stu-id="dd357-107">The API returns up to 1,000 deleted objects owned by the user, sorted by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd357-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="dd357-108">Permissions</span></span>

<span data-ttu-id="dd357-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="dd357-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

| <span data-ttu-id="dd357-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dd357-111">Permission type</span></span> | <span data-ttu-id="dd357-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dd357-112">Permissions (from least to most privileged)</span></span> |
| --- | --- |
| <span data-ttu-id="dd357-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dd357-113">Delegated (work or school account)</span></span> | <span data-ttu-id="dd357-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd357-114">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="dd357-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dd357-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="dd357-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dd357-116">Not supported.</span></span> |
| <span data-ttu-id="dd357-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dd357-117">Application</span></span> | <span data-ttu-id="dd357-118">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd357-118">Group.Read.All, Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="dd357-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dd357-119">HTTP request</span></span>

``` http
POST /directory/deletedItems/getUserOwnedObjects
```

## <a name="request-headers"></a><span data-ttu-id="dd357-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dd357-120">Request headers</span></span>

| <span data-ttu-id="dd357-121">Name</span><span class="sxs-lookup"><span data-stu-id="dd357-121">Name</span></span>          | <span data-ttu-id="dd357-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dd357-122">Description</span></span>               |
| ------------- | ------------------------- |
| <span data-ttu-id="dd357-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd357-123">Authorization</span></span> | <span data-ttu-id="dd357-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="dd357-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd357-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dd357-126">Request body</span></span>

```json
{
  "userId":"{id}",
  "type":"Group"
}
```

<span data-ttu-id="dd357-127">Textkörper der Anforderung erfordert die folgenden Parameter:</span><span class="sxs-lookup"><span data-stu-id="dd357-127">The request body requires the following parameters:</span></span>

| <span data-ttu-id="dd357-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="dd357-128">Parameter</span></span>    | <span data-ttu-id="dd357-129">Typ</span><span class="sxs-lookup"><span data-stu-id="dd357-129">Type</span></span> |<span data-ttu-id="dd357-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dd357-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dd357-131">userId</span><span class="sxs-lookup"><span data-stu-id="dd357-131">userId</span></span>|<span data-ttu-id="dd357-132">String</span><span class="sxs-lookup"><span data-stu-id="dd357-132">String</span></span>|<span data-ttu-id="dd357-133">ID des Besitzers.</span><span class="sxs-lookup"><span data-stu-id="dd357-133">ID of the owner.</span></span>|
|<span data-ttu-id="dd357-134">Typ</span><span class="sxs-lookup"><span data-stu-id="dd357-134">type</span></span>|<span data-ttu-id="dd357-135">String</span><span class="sxs-lookup"><span data-stu-id="dd357-135">String</span></span>|<span data-ttu-id="dd357-136">Art der Objekte zurückgegeben. `Group` ist derzeit der einzige unterstützte Wert.</span><span class="sxs-lookup"><span data-stu-id="dd357-136">Type of owned objects to return; `Group` is currently the only supported value.</span></span>|


## <a name="response"></a><span data-ttu-id="dd357-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="dd357-137">Response</span></span>

<span data-ttu-id="dd357-138">Zurückgeben der erfolgreiche Anforderungen `200 OK` Antwortcodes; Response-Objekt enthält die Eigenschaften des [Verzeichnisses (Gelöschte Objekte)](../resources/directory.md) .</span><span class="sxs-lookup"><span data-stu-id="dd357-138">Successful requests return `200 OK` response codes; the response object includes [directory (deleted items)](../resources/directory.md) properties.</span></span>

## <a name="example"></a><span data-ttu-id="dd357-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dd357-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="dd357-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dd357-140">Request</span></span>

<span data-ttu-id="dd357-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dd357-141">Here is an example of the request.</span></span>

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

###### <a name="response"></a><span data-ttu-id="dd357-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="dd357-142">Response</span></span>

<span data-ttu-id="dd357-143">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="dd357-143">Here is an example of the response.</span></span> <span data-ttu-id="dd357-144">Hinweis: Dieses Antwortobjekt der Kürze halber werden möglicherweise abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="dd357-144">Note: This response object may be truncated for brevity.</span></span> <span data-ttu-id="dd357-145">Alle unterstützte Eigenschaften werden von tatsächlichen Anrufe zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dd357-145">All supported properties are returned from actual calls.</span></span>

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


