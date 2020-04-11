---
title: Резервирование Azure и серверные подписки | Центр партнеров
ms.topic: article
ms.date: 04/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Узнайте о возможностях поставщиков облачных решений по приобретению, подготовке и управлению резервированиями Azure и серверными подписками для своих клиентов.
author: LauraBrenner
ms.author: labrenne
keywords: Azure, подписки, виртуальная машина, резервирование, зарезервированный экземпляр
ms.localizationpriority: medium
ms.openlocfilehash: d0a3fde651db86f8aeed160764fc330a25c0df04
ms.sourcegitcommit: ee7f8600f566799838bda64e26c54799137f2cd5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "81123277"
---
<!-- Mike Aasen wrote and owns this topic -->

# <a name="azure-reserved-vm-instances-ri--server-subscriptions-for-azure"></a><span data-ttu-id="65fc0-104">Azure Reserved VM Instances (RI) + серверные подписки на Azure</span><span class="sxs-lookup"><span data-stu-id="65fc0-104">Azure reserved VM instances (RI) + server subscriptions for Azure</span></span>

<span data-ttu-id="65fc0-105">Область применения:</span><span class="sxs-lookup"><span data-stu-id="65fc0-105">Applies to:</span></span>

- <span data-ttu-id="65fc0-106">Партнерский центр</span><span class="sxs-lookup"><span data-stu-id="65fc0-106">Partner Center</span></span>

<span data-ttu-id="65fc0-107">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="65fc0-107">**Appropriate roles**</span></span>

- <span data-ttu-id="65fc0-108">Агент по администрированию</span><span class="sxs-lookup"><span data-stu-id="65fc0-108">Admin agent</span></span>
- <span data-ttu-id="65fc0-109">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="65fc0-109">Global admin</span></span>
- <span data-ttu-id="65fc0-110">Агент службы технической поддержки</span><span class="sxs-lookup"><span data-stu-id="65fc0-110">Helpdesk agent</span></span>
- <span data-ttu-id="65fc0-111">Агент по продажам</span><span class="sxs-lookup"><span data-stu-id="65fc0-111">Sales agent</span></span>
- <span data-ttu-id="65fc0-112">Администратор управления пользователями</span><span class="sxs-lookup"><span data-stu-id="65fc0-112">User management admin</span></span>
 
## <a name="what-are-azure-reservations"></a><span data-ttu-id="65fc0-113">Что такое резервирование Azure?</span><span class="sxs-lookup"><span data-stu-id="65fc0-113">What are Azure Reservations?</span></span>

<span data-ttu-id="65fc0-114">Резервирование Azure помогает экономить деньги за счет предварительной оплаты за один или три года виртуальной машины, объема вычислений базы данных SQL, Azure Cosmos DB пропускной способности или других ресурсов Azure.</span><span class="sxs-lookup"><span data-stu-id="65fc0-114">Azure Reservations help you save money by pre-paying for one-year or three-years of virtual machine, SQL Database compute capacity, Azure Cosmos DB throughput, or other Azure resources.</span></span> <span data-ttu-id="65fc0-115">Предварительная оплата позволяет получить скидку на используемые ресурсы.</span><span class="sxs-lookup"><span data-stu-id="65fc0-115">Pre-paying allows you to get a discount on the resources you use.</span></span> <span data-ttu-id="65fc0-116">Резервирования помогают значительно снизить затраты на виртуальную машину, вычислительную мощность базы данных SQL, Azure Cosmos DB и другие ресурсы до 72% по сравнению с оплатой по мере использования.</span><span class="sxs-lookup"><span data-stu-id="65fc0-116">Reservations can significantly reduce your virtual machine, SQL database compute, Azure Cosmos DB, and other resource costs up to 72% compared to pay-as-you-go prices.</span></span> <span data-ttu-id="65fc0-117">Резервирование обеспечивает скидку при выставлении счетов и не влияет на состояние среды выполнения ресурсов.</span><span class="sxs-lookup"><span data-stu-id="65fc0-117">Reservations provide a billing discount and don't affect the runtime state of your resources.</span></span> <span data-ttu-id="65fc0-118">Дополнительные сведения см. в статье [что такое резервирование Azure?](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)</span><span class="sxs-lookup"><span data-stu-id="65fc0-118">For more information, see [What are Azure Reservations?](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)</span></span>

## <a name="why-should-customers-buy-a-reservation"></a><span data-ttu-id="65fc0-119">Почему клиенты должны приобрести резервирование?</span><span class="sxs-lookup"><span data-stu-id="65fc0-119">Why should customers buy a reservation?</span></span>

<span data-ttu-id="65fc0-120">Если у клиентов есть виртуальные машины, Azure Cosmos DB или базы данных SQL, работающие в течение длительного периода времени, приобретение резервирования дает им наиболее экономичный вариант.</span><span class="sxs-lookup"><span data-stu-id="65fc0-120">If customers have virtual machines, Azure Cosmos DB or SQL databases that run for long periods of time, purchasing a reservation gives them the most cost-effective option.</span></span> <span data-ttu-id="65fc0-121">Например, если клиент непрерывно запускает четыре экземпляра службы без резервирования, плата взимается по тарифам с оплатой по мере использования.</span><span class="sxs-lookup"><span data-stu-id="65fc0-121">For example, if a customer continuously runs four instances of a service without a reservation, they are charged at pay-as-you-go rates.</span></span> <span data-ttu-id="65fc0-122">Если они приобретают резервирование для этих ресурсов, они незамедлительно получают скидку на резервирование.</span><span class="sxs-lookup"><span data-stu-id="65fc0-122">If they purchase a reservation for those resources, they immediately get the reservation discount.</span></span> <span data-ttu-id="65fc0-123">Ресурсы больше не оплачиваются по тарифам с оплатой по мере использования.</span><span class="sxs-lookup"><span data-stu-id="65fc0-123">The resources are no longer charged at the pay-as-you-go rates.</span></span>

### <a name="compelling-new-azure-offer-in-csp"></a><span data-ttu-id="65fc0-124">Новое интересное предложение Azure в программе CSP</span><span class="sxs-lookup"><span data-stu-id="65fc0-124">Compelling New Azure offer in CSP</span></span>

<span data-ttu-id="65fc0-125">Применяя к своей программе CSP резервирование Azure и серверные подписки, корпорация Майкрософт позволяет партнерам более эффективно обращаться к быстро растущему запросу клиентов.</span><span class="sxs-lookup"><span data-stu-id="65fc0-125">By bringing Azure Reservations and Server Subscriptions to its CSP program, Microsoft allows partners to better address fast-growing customer demand.</span></span> <span data-ttu-id="65fc0-126">Это включает повышение спроса на клиентов для получения более экономичных решений для поддержки высокопрогнозируемых и устойчивых облачных рабочих нагрузок.</span><span class="sxs-lookup"><span data-stu-id="65fc0-126">This includes increased customer demand for more cost-effective solutions to support highly predictable, persistent cloud workloads.</span></span> <span data-ttu-id="65fc0-127">Программа CSP позволяет партнерам получать, подготавливать резервирования Azure и серверные подписки и управлять ими от имени коммерческих клиентов.</span><span class="sxs-lookup"><span data-stu-id="65fc0-127">The CSP program enables partners to acquire, provision, and manage Azure Reservations and Server Subscriptions on behalf of commercial customers.</span></span> <span data-ttu-id="65fc0-128">Партнеры могут выполнять эти задачи с помощью центра партнеров Майкрософт и портал Azure.</span><span class="sxs-lookup"><span data-stu-id="65fc0-128">Partners can perform these tasks via Microsoft Partner Center and the Azure portal.</span></span>

<span data-ttu-id="65fc0-129">Резервирование Azure предоставляет клиентам гибкие возможности виртуализации для широкого спектра вычислительных решений.</span><span class="sxs-lookup"><span data-stu-id="65fc0-129">Azure Reservations give customers the flexibility of virtualization for a wide range of computing solutions.</span></span> <span data-ttu-id="65fc0-130">Такие решения могут включать разработку и тестирование, запуск приложений и расширение центра обработки данных.</span><span class="sxs-lookup"><span data-stu-id="65fc0-130">Such solutions can include development and testing, running applications and extending the data center.</span></span>

<span data-ttu-id="65fc0-131">С Azure Reserved VM Instances, например, коммерческие клиенты теперь могут сэкономить до 72% по сравнению с оплатой по мере использования и платить-по мере использования для виртуальных машин Azure просто путем приобретения или "резервирования" — виртуальной машины в течение 1 или 3 лет.</span><span class="sxs-lookup"><span data-stu-id="65fc0-131">With Azure Reserved VM Instances, for example, commercial customers can now save up to 72% versus pay-as-you-go Azure VM pricing simply by purchasing - or "reserving" - the virtual machine for a 1- or 3-year period.</span></span> <span data-ttu-id="65fc0-132">Клиенты Windows Server с Преимущество гибридного использования Azure, входящими в состав программы Software Assurance, могут сэкономить до 80% по сравнению с ценами с оплатой по мере использования.</span><span class="sxs-lookup"><span data-stu-id="65fc0-132">Windows Server customers with Azure Hybrid Benefit, included with Software Assurance, can save up to 80% versus pay-as-you-go pricing.</span></span>

<span data-ttu-id="65fc0-133">Благодаря несовпадающей комбинации привлекательной цены и несовпадающей гибкости развертывания клиенты увидят лучшее общее значение при выборе резервирования Azure:</span><span class="sxs-lookup"><span data-stu-id="65fc0-133">With an unmatched combination of compelling pricing and unmatched deployment flexibility, customers will see the best overall value when they choose Azure Reservations:</span></span>

#### <a name="azure-reservations"></a><span data-ttu-id="65fc0-134">Резервирования Azure</span><span class="sxs-lookup"><span data-stu-id="65fc0-134">Azure reservations</span></span>

- <span data-ttu-id="65fc0-135">Azure Reserved VM Instances</span><span class="sxs-lookup"><span data-stu-id="65fc0-135">Azure Reserved VM Instances</span></span>
- <span data-ttu-id="65fc0-136">Резервирования базы данных SQL</span><span class="sxs-lookup"><span data-stu-id="65fc0-136">SQL DB Reservations</span></span>
- <span data-ttu-id="65fc0-137">Управляемый экземпляр SQL</span><span class="sxs-lookup"><span data-stu-id="65fc0-137">SQL Managed Instance</span></span>
- <span data-ttu-id="65fc0-138">Azure Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="65fc0-138">Azure Cosmos DB</span></span>
- <span data-ttu-id="65fc0-139">Хранилище данных SQL Azure</span><span class="sxs-lookup"><span data-stu-id="65fc0-139">Azure SQL Data Warehouse</span></span>
- <span data-ttu-id="65fc0-140">Службы приложений</span><span class="sxs-lookup"><span data-stu-id="65fc0-140">App Services</span></span>
- <span data-ttu-id="65fc0-141">Azure Databricks резервирования единиц измерения</span><span class="sxs-lookup"><span data-stu-id="65fc0-141">Azure Databricks unit reservations</span></span>
- <span data-ttu-id="65fc0-142">Управляемый диск</span><span class="sxs-lookup"><span data-stu-id="65fc0-142">Managed Disk</span></span>
- <span data-ttu-id="65fc0-143">Blockblob</span><span class="sxs-lookup"><span data-stu-id="65fc0-143">Blockblob</span></span>
- <span data-ttu-id="65fc0-144">MySQL</span><span class="sxs-lookup"><span data-stu-id="65fc0-144">MySQL</span></span>
- <span data-ttu-id="65fc0-145">Обозреватель данных Azure</span><span class="sxs-lookup"><span data-stu-id="65fc0-145">Azure Data explorer</span></span>
- <span data-ttu-id="65fc0-146">MariaDB</span><span class="sxs-lookup"><span data-stu-id="65fc0-146">MariaDB</span></span>
- <span data-ttu-id="65fc0-147">PostgreSQL</span><span class="sxs-lookup"><span data-stu-id="65fc0-147">PostgreSQL</span></span>

#### <a name="server-subscriptions"></a><span data-ttu-id="65fc0-148">Серверные подписки</span><span class="sxs-lookup"><span data-stu-id="65fc0-148">Server subscriptions</span></span>

- <span data-ttu-id="65fc0-149">Windows Server</span><span class="sxs-lookup"><span data-stu-id="65fc0-149">Windows Server</span></span>
- <span data-ttu-id="65fc0-150">Клиентские лицензии службы удаленных рабочих столов (RDS)</span><span class="sxs-lookup"><span data-stu-id="65fc0-150">Remote Desktop Services (RDS) CALs</span></span>
- <span data-ttu-id="65fc0-151">SQL Server</span><span class="sxs-lookup"><span data-stu-id="65fc0-151">SQL Server</span></span>

#### <a name="linux-isv-annual-subscriptions"></a><span data-ttu-id="65fc0-152">Ежегодные подписки независимых поставщиков по Linux</span><span class="sxs-lookup"><span data-stu-id="65fc0-152">Linux ISV annual subscriptions</span></span>

- <span data-ttu-id="65fc0-153">SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="65fc0-153">SUSE Linux</span></span>
- <span data-ttu-id="65fc0-154">Red Hat Enterprise Linux</span><span class="sxs-lookup"><span data-stu-id="65fc0-154">Red Hat Enterprise Linux</span></span>
- <span data-ttu-id="65fc0-155">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="65fc0-155">Azure Red Hat OpenShift</span></span>

#### <a name="isv-annual-subscriptions"></a><span data-ttu-id="65fc0-156">Ежегодные подписки ISV</span><span class="sxs-lookup"><span data-stu-id="65fc0-156">ISV annual subscriptions</span></span>

- <span data-ttu-id="65fc0-157">Решение VMware для Azure от Клаудсимпле</span><span class="sxs-lookup"><span data-stu-id="65fc0-157">Azure VMware Solution by CloudSimple</span></span>

## <a name="getting-started"></a><span data-ttu-id="65fc0-158">Начало работы</span><span class="sxs-lookup"><span data-stu-id="65fc0-158">Getting started</span></span>

<span data-ttu-id="65fc0-159">Чтобы понять, как можно разместить резервирование Azure для клиентов и быстро приступить к работе, мы рекомендуем использовать следующий подход для просмотра материалов о готовности:</span><span class="sxs-lookup"><span data-stu-id="65fc0-159">To understand how you can position Azure Reservations with your customers and get up and running operationally as quickly as possible, we recommend the following approach to review the readiness materials:</span></span>

1. <span data-ttu-id="65fc0-160">Просмотрите обзорную презентацию и сопутствующий вебинар о позиционировании и формировании предложений для клиентов</span><span class="sxs-lookup"><span data-stu-id="65fc0-160">Review the Overview Presentations and associated webinars for the customer value proposition and positioning</span></span>
2. <span data-ttu-id="65fc0-161">Изучите руководство по современной коммерции</span><span class="sxs-lookup"><span data-stu-id="65fc0-161">Review and understand the Modern Commerce Operating Guide</span></span>
3. <span data-ttu-id="65fc0-162">Изучите раздел "Подписки на Azure RI и серверные подписки: вопросы и ответы"</span><span class="sxs-lookup"><span data-stu-id="65fc0-162">Review the Azure RI and Server Subscriptions FAQ</span></span>
4. <span data-ttu-id="65fc0-163">Ознакомьтесь с информацией об обновлении резервирований Azure и серверных подписок в документе [API Центра партнеров (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)</span><span class="sxs-lookup"><span data-stu-id="65fc0-163">Understand updates for Azure Reservations and Server Subscriptions in the [Partner Center API (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)</span></span>

## <a name="resources"></a><span data-ttu-id="65fc0-164">Ресурсы</span><span class="sxs-lookup"><span data-stu-id="65fc0-164">Resources</span></span>

<span data-ttu-id="65fc0-165">Ниже приведен полный список ресурсов, которые помогут вам быстро приступить к работе с резервированиями Azure в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="65fc0-165">Below is a comprehensive list of resources to help you onboard quickly to transacting Azure Reservations through Partner Center:</span></span>

### <a name="sales-readiness"></a><span data-ttu-id="65fc0-166">Готовность к продажам</span><span class="sxs-lookup"><span data-stu-id="65fc0-166">Sales readiness</span></span>

- [<span data-ttu-id="65fc0-167">Резервирование Azure и серверные подписки с обзором Преимущество гибридного использования Azure</span><span class="sxs-lookup"><span data-stu-id="65fc0-167">Azure Reservations and Server Subscriptions with Azure Hybrid Benefit Overview</span></span>](https://assetsprod.microsoft.com/Azure-reservations-and-server-subscriptions-with-azure-hybrid-benefit.pptx)
- [<span data-ttu-id="65fc0-168">Информационный листок</span><span class="sxs-lookup"><span data-stu-id="65fc0-168">Sales Sheet</span></span>](https://assetsprod.microsoft.com/mpn/Azure-RI-Sales-Sheet-CSP.pdf)
- [<span data-ttu-id="65fc0-169">Часто задаваемые вопросы о резервировании Azure для партнеров</span><span class="sxs-lookup"><span data-stu-id="65fc0-169">Partner FAQ for Azure Reservations</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations.docx)
- [<span data-ttu-id="65fc0-170">Раздел вопросов и ответов для партнеров по резервированиям Azure и базе данных SQL (обновлено)</span><span class="sxs-lookup"><span data-stu-id="65fc0-170">Partner FAQ for Azure Reservations and SQL DB</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations-sql-db.docx)
- [<span data-ttu-id="65fc0-171">Клиентские лицензии службы удаленных рабочих столов (RDS) (объявление)</span><span class="sxs-lookup"><span data-stu-id="65fc0-171">Remote Desktop Services (RDS) CALs (announcement)</span></span>](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)
- [<span data-ttu-id="65fc0-172">Azure Reserved VM Instances (портал Azure)</span><span class="sxs-lookup"><span data-stu-id="65fc0-172">Azure Reserved VM Instances (Azure portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances)
- [<span data-ttu-id="65fc0-173">Серверные подписки</span><span class="sxs-lookup"><span data-stu-id="65fc0-173">Server Subscriptions</span></span>](https://docs.microsoft.com/partner-center/csp-software-subscriptions)
- [<span data-ttu-id="65fc0-174">Общие сведения о базе данных SQL в Azure</span><span class="sxs-lookup"><span data-stu-id="65fc0-174">SQL DB in Azure Overview</span></span>](https://assetsprod.microsoft.com/Sql-db-in-azure-overview.pptx)
- [<span data-ttu-id="65fc0-175">Резервирования базы данных SQL (портал Azure)</span><span class="sxs-lookup"><span data-stu-id="65fc0-175">SQL DB Reservations (Azure portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-reserved-capacity)
- [<span data-ttu-id="65fc0-176">Azure Cosmos DB (портал Azure)</span><span class="sxs-lookup"><span data-stu-id="65fc0-176">Azure Cosmos DB (Azure portal)</span></span>](https://docs.microsoft.com/azure/cosmos-db/cosmos-db-reserved-capacity)
- [<span data-ttu-id="65fc0-177">Управляемый экземпляр SQL (портал Azure)</span><span class="sxs-lookup"><span data-stu-id="65fc0-177">SQL Managed Instance (Azure portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-managed-instance)
- [<span data-ttu-id="65fc0-178">SUSE и Red Hat Enterprise Linux (портал Azure)</span><span class="sxs-lookup"><span data-stu-id="65fc0-178">SUSE and Red Hat Enterprise Linux (Azure portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/linux/prepay-suse-software-charges)
- [<span data-ttu-id="65fc0-179">Red Hat Linux в Azure</span><span class="sxs-lookup"><span data-stu-id="65fc0-179">Red Hat Linux on Azure</span></span>](https://azure.com/redhat)
- [<span data-ttu-id="65fc0-180">SUSE Linux в Azure</span><span class="sxs-lookup"><span data-stu-id="65fc0-180">SUSE Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/suse/)
- [<span data-ttu-id="65fc0-181">Linux в Azure</span><span class="sxs-lookup"><span data-stu-id="65fc0-181">Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/)
- [<span data-ttu-id="65fc0-182">Общие сведения о ценах на Azure</span><span class="sxs-lookup"><span data-stu-id="65fc0-182">Azure Pricing Overview</span></span>](https://azure.microsoft.com/pricing/)
- [<span data-ttu-id="65fc0-183">Калькулятор цен для Azure</span><span class="sxs-lookup"><span data-stu-id="65fc0-183">Azure Pricing Calculator</span></span>](https://azure.microsoft.com/pricing/calculator)
- [<span data-ttu-id="65fc0-184">Azure Databricks резервирования единиц измерения</span><span class="sxs-lookup"><span data-stu-id="65fc0-184">Azure Databricks unit reservations</span></span>](https://docs.microsoft.com/azure/billing/billing-prepay-databricks-reserved-capacity)
- <span data-ttu-id="65fc0-185">Прайс-страницы CSP. списки **Microsoft Azure зарезервированные экземпляры** и цены на **программное обеспечение** находятся на странице цен на центр партнеров [& предложения](https://partner.microsoft.com/pcv/sales) .</span><span class="sxs-lookup"><span data-stu-id="65fc0-185">CSP Price lists:  The **Microsoft Azure Reserved Instances** and **Software Subscriptions** price lists are both located on the Partner Center [Pricing & Offers](https://partner.microsoft.com/pcv/sales) page.</span></span>

### <a name="training"></a><span data-ttu-id="65fc0-186">Обучение</span><span class="sxs-lookup"><span data-stu-id="65fc0-186">Training</span></span>

<span data-ttu-id="65fc0-187">Зарегистрируйтесь для просмотра веб- [семинаров о готовности к лицензированию](https://commercial-licensing.eventbuilder.com/FY2019_ALL) и событиях по требованию.</span><span class="sxs-lookup"><span data-stu-id="65fc0-187">Register to view [Commercial Licensing Readiness webinars](https://commercial-licensing.eventbuilder.com/FY2019_ALL) and on-demand events.</span></span>

<span data-ttu-id="65fc0-188">События готовности к лицензированию по требованию включают такие темы:</span><span class="sxs-lookup"><span data-stu-id="65fc0-188">Licensing Readiness on-demand events include topics like:</span></span>

- <span data-ttu-id="65fc0-189">Веб-службы CSP, Azure CSP и общие обновления лицензирования, включая Azure (Ноябрь 2018)</span><span class="sxs-lookup"><span data-stu-id="65fc0-189">CSP Online Services, CSP Azure, and general licensing updates, including Azure (November 2018)</span></span>
- <span data-ttu-id="65fc0-190">Зарезервированная емкость базы данных SQL & гибкость размера экземпляра (2018 августа)</span><span class="sxs-lookup"><span data-stu-id="65fc0-190">SQL DB Reserved Capacity & Instance Size Flexibility (August 2018)</span></span>
- <span data-ttu-id="65fc0-191">Серверные подписки в CSP (Июль 2018)</span><span class="sxs-lookup"><span data-stu-id="65fc0-191">Server Subscriptions in CSP (July 2018)</span></span>
- <span data-ttu-id="65fc0-192">Обзор резервирования Azure в CSP (Май 2018)</span><span class="sxs-lookup"><span data-stu-id="65fc0-192">Azure Reservations Overview in CSP (May 2018)</span></span>

<span data-ttu-id="65fc0-193">Другое полезное обучение включает в себя [модуль лицензирования Azure в университете Partner](https://aka.ms/azure_partner_licensing).</span><span class="sxs-lookup"><span data-stu-id="65fc0-193">Other useful training includes the [Azure Licensing Module on Partner University](https://aka.ms/azure_partner_licensing).</span></span>

### <a name="operations"></a><span data-ttu-id="65fc0-194">Операции</span><span class="sxs-lookup"><span data-stu-id="65fc0-194">Operations</span></span>

- <span data-ttu-id="65fc0-195">[Руководство по современным коммерческим операциям](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (Обновлено): исчерпывающее руководство по ключевым политикам и рабочим аспектам, таким как соглашения, упорядочение по центру партнеров, счета, сведения о прайс-листах, поощрения, файл СВЕРКИ, API/SDK, песочница и общие службы партнеров Azure.</span><span class="sxs-lookup"><span data-stu-id="65fc0-195">[Modern Commerce Operations Guide](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (updated):  A comprehensive guide covering key policy and operational aspects such as agreements, ordering through Partner Center, invoice, price list details, incentives, reconciliation file, API/SDK, Sandbox, and Azure Partner Shared Services.</span></span>
- [<span data-ttu-id="65fc0-196">Последние сведения о доступности предложений в странах и матрица валют для клиентов</span><span class="sxs-lookup"><span data-stu-id="65fc0-196">Modern Offers Country Availability and Customer Currency Matrix</span></span>](https://assetsprod.microsoft.com/modern-offers-country-currency-availability.xlsx)
- [<span data-ttu-id="65fc0-197">Продажа Microsoft Azure зарезервированных экземпляров</span><span class="sxs-lookup"><span data-stu-id="65fc0-197">Sell Microsoft Azure Reserved Instances</span></span>](https://go.microsoft.com/fwlink/?linkid=872806)
- [<span data-ttu-id="65fc0-198">Приобретение резервирований Microsoft Azure от лица клиентов</span><span class="sxs-lookup"><span data-stu-id="65fc0-198">Buy Microsoft Azure reservations on behalf of your customers</span></span>](https://go.microsoft.com/fwlink/?linkid=872807)
- [<span data-ttu-id="65fc0-199">Управление резервированиями Azure от имени клиентов</span><span class="sxs-lookup"><span data-stu-id="65fc0-199">Manage Azure reservations on behalf of your customers</span></span>](https://go.microsoft.com/fwlink/?linkid=872808)
- [<span data-ttu-id="65fc0-200">Выставление счетов за резервирование Azure</span><span class="sxs-lookup"><span data-stu-id="65fc0-200">Billing for Azure reservations</span></span>](azure-plan-billing.md)
- [<span data-ttu-id="65fc0-201">Размеры виртуальных машин для максимального использования резервирования</span><span class="sxs-lookup"><span data-stu-id="65fc0-201">VM sizing for maximum reservation usage</span></span>](https://go.microsoft.com/fwlink/?linkid=872810)
- [<span data-ttu-id="65fc0-202">API центра партнеров (API/SDK)</span><span class="sxs-lookup"><span data-stu-id="65fc0-202">Partner Center API (API/SDK)</span></span>](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)
- [<span data-ttu-id="65fc0-203">Службы удаленных рабочих столов</span><span class="sxs-lookup"><span data-stu-id="65fc0-203">Remote Desktop Services</span></span>](https://docs.microsoft.com/windows-server/remote/remote-desktop-services/welcome-to-rds)

## <a name="azure-hybrid-benefit"></a><span data-ttu-id="65fc0-204">Преимущество гибридного использования Azure</span><span class="sxs-lookup"><span data-stu-id="65fc0-204">Azure Hybrid Benefit</span></span>

<span data-ttu-id="65fc0-205">[Преимущество гибридного использования Azure](https://azure.microsoft.com/pricing/hybrid-benefit) помогает получить дополнительную прибыль от лицензий на Windows Server и сэкономить до \*47 процентов на виртуальных машинах.</span><span class="sxs-lookup"><span data-stu-id="65fc0-205">The [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) helps you get more value from your Windows Server licenses and save up to \*47 percent on virtual machines.</span></span> <span data-ttu-id="65fc0-206">Это преимущество можно использовать с лицензиями Windows Server Datacenter и Standard Edition, зарегистрированными в программе Software Assurance.</span><span class="sxs-lookup"><span data-stu-id="65fc0-206">You can use the benefit with Windows Server Datacenter and Standard edition licenses covered with Software Assurance.</span></span> <span data-ttu-id="65fc0-207">В зависимости от выпуска вы можете преобразовывать или повторно использовать лицензии для запуска виртуальных машин Windows Server в Azure и платить за нижнюю базовую частоту вычислений (тарифы виртуальных машин Linux).</span><span class="sxs-lookup"><span data-stu-id="65fc0-207">Depending on the edition, you can convert or reuse your licenses to run Windows Server virtual machines in Azure and pay a lower base compute rate (Linux virtual machine rates).</span></span>

<span data-ttu-id="65fc0-208">См. также [Преимущество гибридного использования Azure — вопросы и ответы](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span><span class="sxs-lookup"><span data-stu-id="65fc0-208">See also [Azure Hybrid Benefit FAQ](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span></span>

<span data-ttu-id="65fc0-209">\* Фактическая экономия может варьироваться в зависимости от региона, типа экземпляра или использования.</span><span class="sxs-lookup"><span data-stu-id="65fc0-209">\*Actual savings may vary based on region, instance type, or usage.</span></span>
