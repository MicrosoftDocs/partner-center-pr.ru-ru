---
title: Резервирования Azure & серверные подписки
ms.topic: article
ms.date: 11/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Узнайте о возможностях поставщиков облачных решений по приобретению, подготовке и управлению резервированиями Azure и серверными подписками для клиентов.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0434ad2e6494f5efc1b1e5e2aa003dc6587d7b4e
ms.sourcegitcommit: 6ed7268356445939db8613f2af96016707c55d64
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/17/2020
ms.locfileid: "94691356"
---
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a><span data-ttu-id="56b44-103">Получение, инициализация, & управление зарезервированными экземплярами виртуальных машин Azure (RI) и серверными подписками для клиентов</span><span class="sxs-lookup"><span data-stu-id="56b44-103">Acquire, provision, & manage Azure reserved VM instances (RI) + server subscriptions for customers</span></span>


<span data-ttu-id="56b44-104">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="56b44-104">**Appropriate roles**</span></span>

- <span data-ttu-id="56b44-105">Агент по администрированию</span><span class="sxs-lookup"><span data-stu-id="56b44-105">Admin agent</span></span>
- <span data-ttu-id="56b44-106">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="56b44-106">Global admin</span></span>
- <span data-ttu-id="56b44-107">Агент службы технической поддержки</span><span class="sxs-lookup"><span data-stu-id="56b44-107">Helpdesk agent</span></span>
- <span data-ttu-id="56b44-108">Агент по продажам</span><span class="sxs-lookup"><span data-stu-id="56b44-108">Sales agent</span></span>
- <span data-ttu-id="56b44-109">Администратор управления пользователями</span><span class="sxs-lookup"><span data-stu-id="56b44-109">User management admin</span></span>


## <a name="what-are-azure-reservations"></a><span data-ttu-id="56b44-110">Общие сведения о резервированиях в Azure</span><span class="sxs-lookup"><span data-stu-id="56b44-110">What are Azure Reservations?</span></span>

<span data-ttu-id="56b44-111">Резервирование Azure помогает экономить деньги за счет предварительной оплаты за один или три года виртуальной машины, объема вычислений базы данных SQL, Azure Cosmos DB пропускной способности или других ресурсов Azure.</span><span class="sxs-lookup"><span data-stu-id="56b44-111">Azure Reservations help you save money by pre-paying for one-year or three-years of virtual machine, SQL Database compute capacity, Azure Cosmos DB throughput, or other Azure resources.</span></span> <span data-ttu-id="56b44-112">Предоплата позволяет получить скидку на использование ресурсов.</span><span class="sxs-lookup"><span data-stu-id="56b44-112">Pre-paying allows you to get a discount on the resources you use.</span></span> <span data-ttu-id="56b44-113">Резервирования могут значительно снизить объем виртуальной машины, вычисление базы данных SQL, Azure Cosmos DB и другие затраты на ресурсы до 72% по сравнению с ценами оплаты по мере использования.</span><span class="sxs-lookup"><span data-stu-id="56b44-113">Reservations can significantly reduce your virtual machine, SQL database compute, Azure Cosmos DB, and other resource costs up to 72% compared to pay-as-you-go prices.</span></span> <span data-ttu-id="56b44-114">Резервирования предоставляют скидку при выставлении счетов и не влияют на состояние выполнения ваших ресурсов.</span><span class="sxs-lookup"><span data-stu-id="56b44-114">Reservations provide a billing discount and don't affect the runtime state of your resources.</span></span> <span data-ttu-id="56b44-115">Дополнительные сведения см. в статье [что такое резервирование Azure?](/azure/billing/billing-save-compute-costs-reservations)</span><span class="sxs-lookup"><span data-stu-id="56b44-115">For more information see [What are Azure Reservations?](/azure/billing/billing-save-compute-costs-reservations)</span></span>

## <a name="why-should-customers-buy-a-reservation"></a><span data-ttu-id="56b44-116">Почему клиенты должны приобрести резервирование?</span><span class="sxs-lookup"><span data-stu-id="56b44-116">Why should customers buy a reservation?</span></span>

<span data-ttu-id="56b44-117">Если у клиентов есть виртуальные машины, Azure Cosmos DB или базы данных SQL, работающие в течение длительного периода времени, приобретение резервирования дает им наиболее экономичный вариант.</span><span class="sxs-lookup"><span data-stu-id="56b44-117">If customers have virtual machines, Azure Cosmos DB or SQL databases that run for long periods of time, purchasing a reservation gives them the most cost-effective option.</span></span> <span data-ttu-id="56b44-118">Например, если клиент непрерывно запускает четыре экземпляра службы без резервирования, плата взимается по тарифам с оплатой по мере использования.</span><span class="sxs-lookup"><span data-stu-id="56b44-118">For example, if a customer continuously runs four instances of a service without a reservation, they are charged at pay-as-you-go rates.</span></span> <span data-ttu-id="56b44-119">Если они приобретают резервирование для этих ресурсов, они незамедлительно получают скидку на резервирование.</span><span class="sxs-lookup"><span data-stu-id="56b44-119">If they purchase a reservation for those resources, they immediately get the reservation discount.</span></span> <span data-ttu-id="56b44-120">К ресурсам больше не будут применяться ставки оплаты по мере использования.</span><span class="sxs-lookup"><span data-stu-id="56b44-120">The resources are no longer charged at the pay-as-you-go rates.</span></span>

### <a name="compelling-new-azure-offer-in-csp"></a><span data-ttu-id="56b44-121">Новое интересное предложение Azure в программе CSP</span><span class="sxs-lookup"><span data-stu-id="56b44-121">Compelling New Azure offer in CSP</span></span>

<span data-ttu-id="56b44-122">Выполнив резервирование Azure и серверные подписки на свою программу CSP, корпорация Майкрософт лучше позволяет своим партнерам решать быстро растущие потребности клиентов, обеспечивая более экономичные решения для поддержки строго предсказуемых и устойчивых облачных рабочих нагрузок.</span><span class="sxs-lookup"><span data-stu-id="56b44-122">By bringing Azure Reservations and Server Subscriptions to its CSP program, Microsoft is better enabling its partners to address fast-growing customer demand for more cost-effective solutions to support highly predictable, persistent cloud workloads.</span></span> <span data-ttu-id="56b44-123">Программа CSP позволяет партнерам получать, подготавливать резервирования Azure и серверные подписки и управлять ими от имени коммерческих клиентов через центр партнеров Майкрософт и портал Azure.</span><span class="sxs-lookup"><span data-stu-id="56b44-123">The CSP program enables partners to acquire, provision and manage Azure Reservations and Server Subscriptions on behalf of commercial customers via Microsoft Partner Center and Azure portal.</span></span>
<span data-ttu-id="56b44-124">Мы даже предоставляем партнерам в нашей программе CSP сведения о том, как можно приобрести резервирования Azure.</span><span class="sxs-lookup"><span data-stu-id="56b44-124">We even give partners in our CSP program choices about how Azure reservations can be purchased.</span></span> <span data-ttu-id="56b44-125">Партнеры CSP могут [купить резервирование Azure от имени клиента](azure-reservations-buying.md) или [позволить клиенту покупать собственные резервирования](give-customers-permission.md) из предыдущей подписки Azure, приобретенной для них партнером.</span><span class="sxs-lookup"><span data-stu-id="56b44-125">CSP partners can [buy Azure reservations on behalf of a customer](azure-reservations-buying.md) or they can [allow the customer to buy their own reservations](give-customers-permission.md) from a prior Azure subscription the partner has purchased for them.</span></span>

<span data-ttu-id="56b44-126">Резервирование Azure предоставляет клиентам гибкие возможности виртуализации для широкого спектра вычислительных решений, включая разработку и тестирование, запуск приложений и расширение центра обработки данных.</span><span class="sxs-lookup"><span data-stu-id="56b44-126">Azure Reservations give customers the flexibility of virtualization for a wide range of computing solutions, including development and testing, running applications and extending the data center.</span></span>

<span data-ttu-id="56b44-127">С [Azure reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) , например, коммерческие клиенты могут сэкономить до 72% по сравнению с оплатой по мере использования, используя цены на виртуальные машины Azure по мере покупки или "резервирования" — виртуальную машину на 1-или 3-летний период.</span><span class="sxs-lookup"><span data-stu-id="56b44-127">With [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) for example, commercial customers can now save up to 72% versus pay-as-you-go Azure VM pricing simply by purchasing - or "reserving" - the virtual machine for a 1- or 3-year period.</span></span> <span data-ttu-id="56b44-128">Клиенты с Windows Server, которые уже успели оценить преимущества гибридного использования Azure и поддержки Software Assurance, могут сэкономить до 80% по сравнению с моделью оплаты по мере использования.</span><span class="sxs-lookup"><span data-stu-id="56b44-128">Windows Server customers with Azure Hybrid Benefit, included with Software Assurance, will be able to save up to 80% versus pay-as-you-go pricing.</span></span>

<span data-ttu-id="56b44-129">Благодаря несовпадающей комбинации привлекательной цены и несовпадающей гибкости развертывания клиенты увидят лучшее общее значение при выборе резервирования Azure.</span><span class="sxs-lookup"><span data-stu-id="56b44-129">With an unmatched combination of compelling pricing and unmatched deployment flexibility, customers will see the best overall value when they choose Azure Reservations.</span></span>

- <span data-ttu-id="56b44-130">См. раздел [резервирования покупок](https://docs.microsoft.com/azure/cost-management-billing/reservations/prepare-buy-reservation#purchase-reservations) на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="56b44-130">See [Purchase Reservations](https://docs.microsoft.com/azure/cost-management-billing/reservations/prepare-buy-reservation#purchase-reservations) on the Azure Portal.</span></span>

- <span data-ttu-id="56b44-131">Просмотрите **список коммерческих цен Azure RI CSP** в категории **Microsoft Azure зарезервированные экземпляры** на странице [цены и предложения](https://partner.microsoft.com/dashboard/sell/pricingandoffers) в центре партнеров для подписок на программное обеспечение и годовых подписок независимых поставщиков по Linux.</span><span class="sxs-lookup"><span data-stu-id="56b44-131">See the **Azure RI CSP Commercial Price List** under the **Microsoft Azure Reserved Instances** category on the [Pricing and Offers](https://partner.microsoft.com/dashboard/sell/pricingandoffers) page in Partner Center for software subscriptions and Linux ISV annual subscriptions.</span></span>


 
<span data-ttu-id="56b44-132">**Ежегодные подписки независимых поставщиков по Linux**</span><span class="sxs-lookup"><span data-stu-id="56b44-132">**Linux ISV annual subscriptions**</span></span>

- <span data-ttu-id="56b44-133">SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="56b44-133">SUSE Linux</span></span>
- <span data-ttu-id="56b44-134">Red Hat Enterprise Linux</span><span class="sxs-lookup"><span data-stu-id="56b44-134">Red Hat Enterprise Linux</span></span>
- <span data-ttu-id="56b44-135">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="56b44-135">Azure Red Hat OpenShift</span></span>

<span data-ttu-id="56b44-136">**Ежегодные подписки ISV**</span><span class="sxs-lookup"><span data-stu-id="56b44-136">**ISV annual subscriptions**</span></span>

- <span data-ttu-id="56b44-137">Решение VMware в Azure от CloudSimple</span><span class="sxs-lookup"><span data-stu-id="56b44-137">Azure VMware Solution by CloudSimple</span></span>

## <a name="getting-started"></a><span data-ttu-id="56b44-138">Начало работы</span><span class="sxs-lookup"><span data-stu-id="56b44-138">Getting started</span></span>

<span data-ttu-id="56b44-139">Чтобы понять, как можно разместить резервирование Azure для клиентов и быстро приступить к работе, мы рекомендуем использовать следующий подход для просмотра материалов о готовности:</span><span class="sxs-lookup"><span data-stu-id="56b44-139">To understand how you can position Azure Reservations with your customers and get up and running operationally as quickly as possible, we recommend the following approach to review the readiness materials:</span></span>

1. <span data-ttu-id="56b44-140">Ознакомьтесь с [новым руководством по созданию коммерческих операций в центре партнеров](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf).</span><span class="sxs-lookup"><span data-stu-id="56b44-140">Review and understand the [Partner Center new commerce operations guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf).</span></span>

2. <span data-ttu-id="56b44-141">Сведения об обновлениях для резервирования Azure и серверных подписок в [API центра партнеров (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances).</span><span class="sxs-lookup"><span data-stu-id="56b44-141">Understand updates for Azure Reservations and Server Subscriptions in the [Partner Center API (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances).</span></span>


### <a name="sales-readiness"></a><span data-ttu-id="56b44-142">Готовность к продажам</span><span class="sxs-lookup"><span data-stu-id="56b44-142">Sales readiness</span></span>

- [<span data-ttu-id="56b44-143">Клиентская лицензия службы удаленных рабочих столов (RDS) (объявление)</span><span class="sxs-lookup"><span data-stu-id="56b44-143">Remote Desktop Services (RDS) Client Access License (CAL) (announcement)</span></span>](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)

- [<span data-ttu-id="56b44-144">Azure Reserved VM Instances (портал Azure)</span><span class="sxs-lookup"><span data-stu-id="56b44-144">Azure Reserved VM Instances (Azure portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances)

- [<span data-ttu-id="56b44-145">Серверные подписки</span><span class="sxs-lookup"><span data-stu-id="56b44-145">Server Subscriptions</span></span>](https://docs.microsoft.com/partner-center/csp-software-subscriptions)

- [<span data-ttu-id="56b44-146">Резервирования базы данных SQL (портал Azure)</span><span class="sxs-lookup"><span data-stu-id="56b44-146">SQL DB Reservations (Azure portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-reserved-capacity)

- [<span data-ttu-id="56b44-147">Azure Cosmos DB (портал Azure)</span><span class="sxs-lookup"><span data-stu-id="56b44-147">Azure Cosmos DB (Azure portal)</span></span>](https://docs.microsoft.com/azure/cosmos-db/cosmos-db-reserved-capacity)

- [<span data-ttu-id="56b44-148">Управляемый экземпляр SQL (портал Azure)</span><span class="sxs-lookup"><span data-stu-id="56b44-148">SQL Managed Instance (Azure portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-managed-instance)

- [<span data-ttu-id="56b44-149">SUSE и Red Hat Enterprise Linux (портал Azure)</span><span class="sxs-lookup"><span data-stu-id="56b44-149">SUSE and Red Hat Enterprise Linux (Azure portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/linux/prepay-suse-software-charges)

- [<span data-ttu-id="56b44-150">Red Hat Linux в Azure</span><span class="sxs-lookup"><span data-stu-id="56b44-150">Red Hat Linux on Azure</span></span>](https://azure.com/redhat)

- [<span data-ttu-id="56b44-151">SUSE Linux в Azure</span><span class="sxs-lookup"><span data-stu-id="56b44-151">SUSE Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/suse/)

- [<span data-ttu-id="56b44-152">Linux в Azure</span><span class="sxs-lookup"><span data-stu-id="56b44-152">Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/)

- [<span data-ttu-id="56b44-153">Общие сведения о ценах на Azure</span><span class="sxs-lookup"><span data-stu-id="56b44-153">Azure Pricing Overview</span></span>](https://azure.microsoft.com/pricing/)

- [<span data-ttu-id="56b44-154">Калькулятор стоимости — оцените свои расходы</span><span class="sxs-lookup"><span data-stu-id="56b44-154">Azure Pricing Calculator</span></span>](https://azure.microsoft.com/pricing/calculator)

- [<span data-ttu-id="56b44-155">Azure Databricks резервирования единиц измерения</span><span class="sxs-lookup"><span data-stu-id="56b44-155">Azure Databricks unit reservations</span></span>](https://docs.microsoft.com/azure/billing/billing-prepay-databricks-reserved-capacity)


## <a name="training"></a><span data-ttu-id="56b44-156">Обучение</span><span class="sxs-lookup"><span data-stu-id="56b44-156">Training</span></span>

<span data-ttu-id="56b44-157">Зарегистрируйтесь для просмотра веб- [семинаров о готовности к лицензированию](https://commercial-licensing.eventbuilder.com/FY2019_ALL) и событиях по требованию.</span><span class="sxs-lookup"><span data-stu-id="56b44-157">Register to view [Commercial Licensing Readiness webinars](https://commercial-licensing.eventbuilder.com/FY2019_ALL) and on-demand events.</span></span>
<span data-ttu-id="56b44-158">Ранее записанные события готовности к лицензированию по требованию включают такие темы:</span><span class="sxs-lookup"><span data-stu-id="56b44-158">Previously recorded Licensing Readiness on-demand events include topics like:</span></span>

- <span data-ttu-id="56b44-159">Веб-службы CSP, Azure CSP и общие обновления лицензирования, включая Azure (Ноябрь 2018)</span><span class="sxs-lookup"><span data-stu-id="56b44-159">CSP Online Services, CSP Azure, and general licensing updates, including Azure (November 2018)</span></span>

- <span data-ttu-id="56b44-160">Зарезервированная емкость базы данных SQL & гибкость размера экземпляра (2018 августа)</span><span class="sxs-lookup"><span data-stu-id="56b44-160">SQL DB Reserved Capacity & Instance Size Flexibility (August 2018)</span></span>

- <span data-ttu-id="56b44-161">Серверные подписки в CSP (Июль 2018)</span><span class="sxs-lookup"><span data-stu-id="56b44-161">Server Subscriptions in CSP (July 2018)</span></span>

- <span data-ttu-id="56b44-162">Обзор резервирования Azure в CSP (Май 2018)</span><span class="sxs-lookup"><span data-stu-id="56b44-162">Azure Reservations Overview in CSP (May 2018)</span></span>

## <a name="operations"></a><span data-ttu-id="56b44-163">Operations</span><span class="sxs-lookup"><span data-stu-id="56b44-163">Operations</span></span>

<span data-ttu-id="56b44-164">[Центр партнеров новое руководство по коммерческим операциям](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf). исчерпывающее руководство по ключевым политикам и рабочим аспектам, таким как соглашения, упорядочение по центру партнеров, счет, сведения о прайс-листах, поощрения, файл СВЕРКИ, API/SDK, песочница и общие службы партнеров Azure.</span><span class="sxs-lookup"><span data-stu-id="56b44-164">[Partner Center new commerce operations guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf):  Comprehensive guide covering key policy and operational aspects such as agreements, ordering through Partner Center, invoice, price list details, incentives, reconciliation file, API/SDK, Sandbox, and Azure Partner Shared Services.</span></span>

## <a name="azure-hybrid-benefit"></a><span data-ttu-id="56b44-165">Преимущество гибридного использования Azure</span><span class="sxs-lookup"><span data-stu-id="56b44-165">Azure Hybrid Benefit</span></span>

<span data-ttu-id="56b44-166">[Преимущество гибридного использования Azure](https://azure.microsoft.com/pricing/hybrid-benefit) является преимуществом ценообразования для клиентов, имеющих лицензии с Software Assurance, что позволяет максимально повысить ценность существующих локальных и (или) SQL Serverных инвестиций при миграции в Azure.</span><span class="sxs-lookup"><span data-stu-id="56b44-166">The [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) is a pricing benefit for customers who have licenses with Software Assurance, which helps maximize the value of existing on-premises Windows Server and/or SQL Server license investments when migrating to Azure.</span></span> <span data-ttu-id="56b44-167">Подходящие клиенты могут сэкономить до 40% \* на виртуальных машинах Azure (инфраструктура как услуга или IaaS) и сэкономить до 55% в базе данных SQL Azure (платформа как услуга или PaaS) и SQL Server на виртуальных машинах Azure (IaaS) с Преимущество гибридного использования Azure, что повышает до 80% при объединении с зарезервированными экземплярами Azure.</span><span class="sxs-lookup"><span data-stu-id="56b44-167">Eligible customers can save up to 40%\* on Azure Virtual Machines (infrastructure as a service, or IaaS), and save up to 55% on Azure SQL Database (platform as a service, or PaaS) and SQL Server on Azure Virtual Machines (IaaS) with Azure Hybrid Benefit, which increases to up to 80% when combined with Azure Reserved Instances.</span></span>

## <a name="next-steps"></a><span data-ttu-id="56b44-168">Следующие шаги</span><span class="sxs-lookup"><span data-stu-id="56b44-168">Next steps</span></span>

- [<span data-ttu-id="56b44-169">Вопросы и ответы о программе "Преимущество гибридного использования Azure"</span><span class="sxs-lookup"><span data-stu-id="56b44-169">Azure Hybrid Benefit FAQ</span></span>](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)

<span data-ttu-id="56b44-170">\* Фактическая экономия может варьироваться в зависимости от региона, типа экземпляра или использования.</span><span class="sxs-lookup"><span data-stu-id="56b44-170">\*Actual savings may vary based on region, instance type, or usage.</span></span>
