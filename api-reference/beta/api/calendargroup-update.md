---
title: CalendarGroup aktualisieren
description: Mit dieser API können Sie die Eigenschaften eines Objekts des Typs „calendargroup“ aktualisieren.
ms.openlocfilehash: a201981d53b581085bd765dbe5a280adeb747fcf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058062"
---
# <a name="update-calendargroup"></a><span data-ttu-id="0b683-103">CalendarGroup aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0b683-103">Update calendargroup</span></span>

> <span data-ttu-id="0b683-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0b683-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0b683-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0b683-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0b683-106">Mit dieser API können Sie die Eigenschaften eines Objekts des Typs „calendargroup“ aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="0b683-106">Update the properties of calendargroup object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b683-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0b683-107">Permissions</span></span>

<span data-ttu-id="0b683-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b683-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0b683-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0b683-110">Permission type</span></span>                        | <span data-ttu-id="0b683-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0b683-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="0b683-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0b683-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="0b683-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0b683-113">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="0b683-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0b683-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b683-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0b683-115">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="0b683-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0b683-116">Application</span></span>                            | <span data-ttu-id="0b683-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0b683-117">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="0b683-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0b683-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="0b683-119">Eine [calendarGroup](../resources/calendargroup.md) eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="0b683-119">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
PATCH /me/calendarGroups/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0b683-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0b683-120">Request headers</span></span>

| <span data-ttu-id="0b683-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0b683-121">Header</span></span>        | <span data-ttu-id="0b683-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0b683-122">Value</span></span>                       |
| :------------ | :-------------------------- |
| <span data-ttu-id="0b683-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b683-123">Authorization</span></span> | <span data-ttu-id="0b683-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0b683-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="0b683-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0b683-126">Content-Type</span></span>  | <span data-ttu-id="0b683-p104">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="0b683-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0b683-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0b683-129">Request body</span></span>

<span data-ttu-id="0b683-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="0b683-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0b683-133">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0b683-133">Property</span></span> | <span data-ttu-id="0b683-134">Typ</span><span class="sxs-lookup"><span data-stu-id="0b683-134">Type</span></span>   | <span data-ttu-id="0b683-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0b683-135">Description</span></span>     |
| :------- | :----- | :-------------- |
| <span data-ttu-id="0b683-136">name</span><span class="sxs-lookup"><span data-stu-id="0b683-136">name</span></span>     | <span data-ttu-id="0b683-137">String</span><span class="sxs-lookup"><span data-stu-id="0b683-137">String</span></span> | <span data-ttu-id="0b683-138">Der Gruppenname.</span><span class="sxs-lookup"><span data-stu-id="0b683-138">The group name.</span></span> |

## <a name="response"></a><span data-ttu-id="0b683-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="0b683-139">Response</span></span>

<span data-ttu-id="0b683-140">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [calendarGroup](../resources/calendargroup.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0b683-140">If successful, this method returns a `200 OK` response code and updated [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b683-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0b683-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0b683-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0b683-142">Request</span></span>

<span data-ttu-id="0b683-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0b683-143">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_calendargroup"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/calendarGroups/{id}
Content-type: application/json
Content-length: 30

{
  "name": "name-value"
}
```

##### <a name="response"></a><span data-ttu-id="0b683-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="0b683-144">Response</span></span>

<span data-ttu-id="0b683-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0b683-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 110

{
  "name": "name-value",
  "classId": "11b0131d-43c8-4bbb-b2c8-e80f9a50834a",
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "Update calendargroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
