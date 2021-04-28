---
title: Доступ на основе ролей центра партнеров Insights
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Сведения о конкретных ролях, необходимых для просмотра отчетов центра партнеров. К ним относятся роли средства просмотра отчетов руководителя и средства просмотра отчетов.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a6af9c7d674d1956332a564628b6b2ea0b1796f6
ms.sourcegitcommit: 078eac1456f68585ff1003b21e5e1fe777af314b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "108120789"
---
# <a name="role-based-access-control-to-the-partner-center-insights-dashboard"></a><span data-ttu-id="81be3-104">Управление доступом на основе ролей на панели мониторинга центра партнеров</span><span class="sxs-lookup"><span data-stu-id="81be3-104">Role-based access control to the Partner Center Insights dashboard</span></span>

<span data-ttu-id="81be3-105">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="81be3-105">**Appropriate roles**</span></span>

- <span data-ttu-id="81be3-106">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="81be3-106">Global admin</span></span>
- <span data-ttu-id="81be3-107">Агент по администрированию</span><span class="sxs-lookup"><span data-stu-id="81be3-107">Admin agent</span></span>
- <span data-ttu-id="81be3-108">Средство просмотра отчетов</span><span class="sxs-lookup"><span data-stu-id="81be3-108">Report viewer</span></span>
- <span data-ttu-id="81be3-109">Средство просмотра исполнительных отчетов</span><span class="sxs-lookup"><span data-stu-id="81be3-109">Executive report viewer</span></span>

<span data-ttu-id="81be3-110">Панель мониторинга Insights использует две новые роли в центре партнеров для управления доступом сотрудников к диспетчеру отчетов и средству просмотра отчетов.</span><span class="sxs-lookup"><span data-stu-id="81be3-110">The Insights dashboard uses two new roles in Partner Center to manage employee access to the reports - Executive Report Viewer and Report Viewer.</span></span>  <span data-ttu-id="81be3-111">Пользователи в роли средства просмотра отчетов руководителя имеют доступ ко всем наборам данных отчетов, а пользователи в роли средства просмотра отчетов не будут иметь доступ к конфиденциальным наборам, таким как доход, а также персональные данные клиентов и сотрудников.</span><span class="sxs-lookup"><span data-stu-id="81be3-111">Users in the Executive Report Viewer role have access to all reporting datasets, while users in the Report Viewer role will not have access to sensitive data sets such as revenue and customer/employee personal data.</span></span>  

<span data-ttu-id="81be3-112">Как и в случае с другими ролями центра партнеров, глобальный администратор или администратор учетной записи сможет назначить пользователей этим ролям на странице Управление пользователями.</span><span class="sxs-lookup"><span data-stu-id="81be3-112">As with other Partner Center roles, the Global admin or the Account admin will be able to assign users to those roles on the User management page.</span></span> <span data-ttu-id="81be3-113">Роли могут быть применимы ко всей компании или к конкретным MPN расположениям.</span><span class="sxs-lookup"><span data-stu-id="81be3-113">The roles can be applicable across the entire company or for specific MPN location(s).</span></span> <span data-ttu-id="81be3-114">Роли, назначенные для конкретных расположений MPN, ограничивают пользователя Просмотр данных отчетов, связанных только с выбранными расположениями MPN.</span><span class="sxs-lookup"><span data-stu-id="81be3-114">Roles assigned for specific MPN location(s) limit the user to viewing reporting data associated only with the selected MPN location(s).</span></span> <span data-ttu-id="81be3-115">Партнер может выбрать одно или несколько расположений из приведенного ниже представления.</span><span class="sxs-lookup"><span data-stu-id="81be3-115">Partner can select one or multiple locations from the below view.</span></span>

:::image type="content" source="images/pci/roles.png" alt-text="Отображает параметры ролей центра Insights, зависящих от расположения, для средства просмотра отчетов и для средства просмотра отчетов руководителя.":::

>[!Note]
> <span data-ttu-id="81be3-117">Пользователи, MPN администраторов на 20 января, 2020 автоматически добавляются в роль **средства просмотра отчетов руководителя** Организации для всех расположений для этого клиента.</span><span class="sxs-lookup"><span data-stu-id="81be3-117">Users who are MPN admins as of Jan 20th, 2020 are automatically added to the company-wide **Executive Report Viewer** role for all locations for that tenant.</span></span> <span data-ttu-id="81be3-118">Таким образом, эти пользователи могут получить доступ к отчетам в качестве средства просмотра отчетов руководителя без явного действия, необходимого глобальному администратору или администратору учетной записи. Глобальные администраторы и администраторы учетных записей могут переопределять автоматические назначенные роли этих пользователей для дальнейшего увеличения или ограничения их возможностей.</span><span class="sxs-lookup"><span data-stu-id="81be3-118">These users are thus able to access the reports as an Executive Report viewer without any explicit action required by Global admin or Account admin. The Global admins and Account admins can override the auto-assigned roles of these users to further increase or limit their capabilities.</span></span>

## <a name="next-steps"></a><span data-ttu-id="81be3-119">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="81be3-119">Next steps</span></span>

- <span data-ttu-id="81be3-120">Дополнительные сведения о [партнерских аналитиках](partner-center-insights.md) и различных отчетах.</span><span class="sxs-lookup"><span data-stu-id="81be3-120">Learn more about [Partner Center Insights](partner-center-insights.md) and its various reports.</span></span>
