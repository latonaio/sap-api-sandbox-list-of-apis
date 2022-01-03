<p align="center"> <img src="https://user-images.githubusercontent.com/91356865/144049159-1ebbd095-87d2-4a3c-81cb-277cc1d4c7b7.png" width="300"> </p> <p align="center"> Starting Up the API Environment on a "Full-of-Beans" SandBox </p>

***

# sap-sandbox-list-of-apis  
sap-sandbox-list-of-apis は、[sap-sandbox](https://github.com/latonaio/sap-sandbox) で 整備された SAP APIs（及び対応する 各 APIサービスランタイム の package responses） をまとめたリポジトリです。  
sap-sandbox-list-of-apis の 「sandbox」は、Netflix 韓国ドラマ 「START-UP」 より、すべての開発者のための 地ならし になればという想いから命名されました。  
なお、各リソースは、そのままクラウド環境におけるアプリケーションにも適用可能です。  

# 前提条件  
sap-sandbox-list-of-apis は、オンプレミス版である（＝クラウド版ではない）SAPS4HANA API の利用を前提としています。  
クラウド版APIを利用する場合は、ご注意ください。  

# READS の List of APIs  

## Central Functions ##

### Business Partner ###

* A_BusinessPartner / [general.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads/blob/main/SAP_API_Caller/responses/general.go)
* A_BusinessPartnerRole / [role.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads/blob/main/SAP_API_Caller/responses/role.go)
* A_BusinessPartnerAddress / [address.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads/blob/main/SAP_API_Caller/responses/address.go)
* A_BusinessPartnerBank / [bank.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads/blob/main/SAP_API_Caller/responses/bank.go)
* ToRole / [to_role.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads/blob/main/SAP_API_Caller/responses/to_role.go)
* ToAddress / [to_address.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads/blob/main/SAP_API_Caller/responses/to_address.go)
* ToBank / [to_bank.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads/blob/main/SAP_API_Caller/responses/to_bank.go)

## Logistics ##

### Product Master ###

* A_Product / [general.go](https://github.com/latonaio/sap-api-integrations-product-master-reads/blob/main/SAP_API_Caller/responses/general.go)
* A_ProductPlant / [plant.go](https://github.com/latonaio/sap-api-integrations-product-master-reads/blob/main/SAP_API_Caller/responses/plant.go)
* A_ProductPlantSales / [sales_plant.go](https://github.com/latonaio/sap-api-integrations-product-master-reads/blob/main/SAP_API_Caller/responses/sales_plant.go)
* A_ProductPlantProcurement / [procurement.go](https://github.com/latonaio/sap-api-integrations-product-master-reads/blob/main/SAP_API_Caller/responses/procurement.go)
* A_ProductPlantMRPArea / [mrp_area.go](https://github.com/latonaio/sap-api-integrations-product-master-reads/blob/main/SAP_API_Caller/responses/mrp_area.go)
* A_ProductWorkScheduling / [work_scheduling.go](https://github.com/latonaio/sap-api-integrations-product-master-reads/blob/main/SAP_API_Caller/responses/work_scheduling.go)
* A_ProductSalesDelivery / [sales_organization.go](https://github.com/latonaio/sap-api-integrations-product-master-reads/blob/main/SAP_API_Caller/responses/sales_organization.go)
* A_ProductValuationAccount / [accounting.go](https://github.com/latonaio/sap-api-integrations-product-master-reads/blob/main/SAP_API_Caller/responses/accounting.go)
* A_ProductDescription / [product_desc.go](https://github.com/latonaio/sap-api-integrations-product-master-reads/blob/main/SAP_API_Caller/responses/product_desc.go)

### Batch Master Record ###
* Batch / [batch.go](https://github.com/latonaio/sap-api-integrations-batch-master-record-reads/blob/main/SAP_API_Caller/responses/batch.go)

## Inventory Management ##

### Material Stock ###

* A_MatlStkInAcctMod / [material_stock.go](https://github.com/latonaio/sap-api-integrations-material-stock-reads/blob/main/SAP_API_Caller/responses/material_stock.go)
* ToMaterialStock / [to_material_stock.go](https://github.com/latonaio/sap-api-integrations-material-stock-reads/blob/main/SAP_API_Caller/responses/to_material_stock.go)

### Reservation Document ###

* A_ReservationDocumentHeader / [header.go](https://github.com/latonaio/sap-api-integrations-reservation-document-reads/blob/main/SAP_API_Caller/responses/header.go)
* A_ReservationDocumentItem / [item.go](https://github.com/latonaio/sap-api-integrations-reservation-document-reads/blob/main/SAP_API_Caller/responses/item.go)

### Inbound Delivery ###
* A_InbDeliveryHeader / [header.go](https://github.com/latonaio/sap-api-integrations-inbound-delivery-reads/blob/main/SAP_API_Caller/responses/header.go)
* ToPartner / [to_partner.go](https://github.com/latonaio/sap-api-integrations-inbound-delivery-reads/blob/main/SAP_API_Caller/responses/to_partner.go)
* ToAddress / [to_address.go](https://github.com/latonaio/sap-api-integrations-inbound-delivery-reads/blob/main/SAP_API_Caller/responses/to_address.go)
* ToItem / [to_item.go](https://github.com/latonaio/sap-api-integrations-inbound-delivery-reads/blob/main/SAP_API_Caller/responses/to_item.go)

### Material Document ###

* A_MaterialDocumentHeader / [header.go](https://github.com/latonaio/sap-api-integrations-material-document-reads/blob/main/SAP_API_Caller/responses/header.go)
* A_MaterialDocumentHeaderItem / [item.go](https://github.com/latonaio/sap-api-integrations-material-document-reads/blob/main/SAP_API_Caller/responses/item.go)
* ToItem / [to_item.go](https://github.com/latonaio/sap-api-integrations-material-document-reads/blob/main/SAP_API_Caller/responses/to_item.go)

## Sales Management ##

### Customer Master ###

* A_BusinessPartner / [general.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads-customer/blob/main/SAP_API_Caller/responses/general.go)
* A_BusinessPartnerRole / [role.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads-customer/blob/main/SAP_API_Caller/responses/role.go)
* A_BusinessPartnerAddress / [address.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads-customer/blob/main/SAP_API_Caller/responses/address.go)
* A_BusinessPartnerBank / [bank.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads-customer/blob/main/SAP_API_Caller/responses/bank.go)
* A_Customer / [customer.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads-customer/blob/main/SAP_API_Caller/responses/customer.go)
* A_CustomerSalesArea / [sales_area.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads-customer/blob/main/SAP_API_Caller/responses/sales_area.go)
* A_CustomerCompany / [company.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads-customer/blob/main/SAP_API_Caller/responses/company.go)
* ToRole / [to_role.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads-customer/blob/main/SAP_API_Caller/responses/to_role.go)
* ToAddress / [to_address.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads-customer/blob/main/SAP_API_Caller/responses/to_address.go)
* ToBank / [to_bank.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads-customer/blob/main/SAP_API_Caller/responses/to_bank.go)
* ToCustomer / [to_customer.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads-customer/blob/main/SAP_API_Caller/responses/to_customer.go)
* ToSalesArea / [to_sales_area.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads-customer/blob/main/SAP_API_Caller/responses/to_sales_area.go)
* ToPartnerFunction / [to_partner_function.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads-customer/blob/main/SAP_API_Caller/responses/to_partner_function.go)
* ToCompany / [to_company.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads-customer/blob/main/SAP_API_Caller/responses/to_company.go)

### Sales Pricing ###

* A_SlsPrcgCndnRecdValidity / [pricing_condition_validity.go](https://github.com/latonaio/sap-api-integrations-sales-pricing-reads/blob/main/SAP_API_Caller/responses/pricing_condition_validity.go)
* ToConditionRecord / [to_condition_record.go](https://github.com/latonaio/sap-api-integrations-sales-pricing-reads/blob/main/SAP_API_Caller/responses/to_condition_record.go)

### Sales Inquiry ###
* A_SalesInquiry / [header.go](https://github.com/latonaio/sap-api-integrations-sales-inquiry-reads/blob/main/SAP_API_Caller/responses/header.go)
* A_SalesInquiryItem / [item.go](https://github.com/latonaio/sap-api-integrations-sales-inquiry-reads/blob/main/SAP_API_Caller/responses/item.go)
* ToHeaderPartner / [to_header_partner.go](https://github.com/latonaio/sap-api-integrations-sales-inquiry-reads/blob/main/SAP_API_Caller/responses/to_header_partner.go)
* ToItem / [to_item.go](https://github.com/latonaio/sap-api-integrations-sales-inquiry-reads/blob/main/SAP_API_Caller/responses/item.go)
* ToItemPricingElement / [to_item_pricing_element.go](https://github.com/latonaio/sap-api-integrations-sales-inquiry-reads/blob/main/SAP_API_Caller/responses/to_item_pricing_element.go)

### Sales Quotation ###
* A_SalesQuotation / [header.go](https://github.com/latonaio/sap-api-integrations-sales-quotation-reads/blob/main/SAP_API_Caller/responses/header.go)
* A_SalesQuotationItem / [item.go](https://github.com/latonaio/sap-api-integrations-sales-quotation-reads/blob/main/SAP_API_Caller/responses/item.go)
* ToHeaderPartner / [to_header_partner.go](https://github.com/latonaio/sap-api-integrations-sales-quotation-reads/blob/main/SAP_API_Caller/responses/to_header_partner.go)
* ToItem / [to_item.go](https://github.com/latonaio/sap-api-integrations-sales-quotation-reads/blob/main/SAP_API_Caller/responses/to_item.go)
* ToItemPricingElement / [to_item_pricing_element.go](https://github.com/latonaio/sap-api-integrations-sales-quotation-reads/blob/main/SAP_API_Caller/responses/to_item_pricing_element.go)

### Sales Order ###
* A_SalesOrder / [header.go](https://github.com/latonaio/sap-api-integrations-sales-order-reads/blob/main/SAP_API_Caller/responses/header.go)
* A_SalesOrderItem / [item.go](https://github.com/latonaio/sap-api-integrations-sales-order-reads/blob/main/SAP_API_Caller/responses/item.go)
* ToHeaderPartner / [to_header_partner.go](https://github.com/latonaio/sap-api-integrations-sales-order-reads/blob/main/SAP_API_Caller/responses/to_header_partner.go)
* ToItem / [to_item.go](https://github.com/latonaio/sap-api-integrations-sales-order-reads/blob/main/SAP_API_Caller/responses/to_item.go)
* ToItemScheduleLine / [to_item_schedule_line.go](https://github.com/latonaio/sap-api-integrations-sales-order-reads/blob/main/SAP_API_Caller/responses/to_item_schedule_line.go)
* ToItemPricingElement / [to_item_pricing_element.go](https://github.com/latonaio/sap-api-integrations-sales-order-reads/blob/main/SAP_API_Caller/responses/to_item_pricing_element.go)

### Sales Contract ###
* A_SalesContract / [header.go](https://github.com/latonaio/sap-api-integrations-sales-contract-reads/blob/main/SAP_API_Caller/responses/header.go)
* A_SalesContractItem / [item.go](https://github.com/latonaio/sap-api-integrations-sales-contract-reads/blob/main/SAP_API_Caller/responses/item.go)
* ToHeaderPartner / [to_header_partner.go](https://github.com/latonaio/sap-api-integrations-sales-contract-reads/blob/main/SAP_API_Caller/responses/to_header_partner.go)
* ToItem / [to_item.go](https://github.com/latonaio/sap-api-integrations-sales-contract-reads/blob/main/SAP_API_Caller/responses/to_item.go)
* ToItemPricingElement / [to_item_pricing_element.go](https://github.com/latonaio/sap-api-integrations-sales-contract-reads/blob/main/SAP_API_Caller/responses/to_item_pricing_element.go)

### Sales Scheduling Agreement ###
* A_SchAgrmtHeader / [header.go](https://github.com/latonaio/sap-api-integrations-sales-scheduling-agreement-reads/blob/main/SAP_API_Caller/responses/header.go)
* A_SchAgrmtItem / [item.go](https://github.com/latonaio/sap-api-integrations-sales-scheduling-agreement-reads/blob/main/SAP_API_Caller/responses/item.go)
* ToHeaderPartner / [to_header_partner.go](https://github.com/latonaio/sap-api-integrations-sales-scheduling-agreement-reads/blob/main/SAP_API_Caller/responses/to_header_partner.go)
* ToItem / [to_item.go](https://github.com/latonaio/sap-api-integrations-sales-scheduling-agreement-reads/blob/main/SAP_API_Caller/responses/to_item.go)
* ToItemDeliverySchedule / [to_item_delivery_schedule.go](https://github.com/latonaio/sap-api-integrations-sales-scheduling-agreement-reads/blob/main/SAP_API_Caller/responses/to_item_delivery_schedule.go)
* ToItemScheduleLine / [to_item_schedule_line.go](https://github.com/latonaio/sap-api-integrations-sales-scheduling-agreement-reads/blob/main/SAP_API_Caller/responses/to_item_schedule_line.go)
* ToItemPricingElement / [to_item_pricing_element.go](https://github.com/latonaio/sap-api-integrations-sales-scheduling-agreement-reads/blob/main/SAP_API_Caller/responses/to_item_pricing_element.go)

### Outbound Delivery ###
* A_OutbDeliveryHeader / [header.go](https://github.com/latonaio/sap-api-integrations-outbound-delivery-reads/blob/main/SAP_API_Caller/responses/header.go)
* A_OutbDeliveryHeader('{DeliveryDocument}')/to_DeliveryDocumentPartner / [header_partner.go](https://github.com/latonaio/sap-api-integrations-outbound-delivery-reads/blob/main/SAP_API_Caller/responses/header_partner.go)
* A_OutbDeliveryPartner(PartnerFunction='{PartnerFunction}',SDDocument='{SDDocument}')/to_Address2 / [partner_address.go](https://github.com/latonaio/sap-api-integrations-outbound-delivery-reads/blob/main/SAP_API_Caller/responses/partner_address.go)
* A_OutbDeliveryItem / [item.go](https://github.com/latonaio/sap-api-integrations-outbound-delivery-reads/blob/main/SAP_API_Caller/responses/item.go)
* ToHeaderPartner / [to_header_partner.go](https://github.com/latonaio/sap-api-integrations-outbound-delivery-reads/blob/main/SAP_API_Caller/responses/to_header_partner.go)
* ToPartnerAddress / [to_partner_address.go](https://github.com/latonaio/sap-api-integrations-outbound-delivery-reads/blob/main/SAP_API_Caller/responses/to_partner_address.go)
* ToItem / [to_item.go](https://github.com/latonaio/sap-api-integrations-outbound-delivery-reads/blob/main/SAP_API_Caller/responses/to_item.go)
* ToItemDocumentFlow / [to_item_document_flow.go](https://github.com/latonaio/sap-api-integrations-outbound-delivery-reads/blob/main/SAP_API_Caller/responses/to_item_document_flow.go)

### Billing Document ###
* A_BillingDocument / [header.go](https://github.com/latonaio/sap-api-integrations-billing-document-reads/blob/main/SAP_API_Caller/responses/header.go)
* A_BillingDocumentItem / [item.go](https://github.com/latonaio/sap-api-integrations-billing-document-reads/blob/main/SAP_API_Caller/responses/item.go)
* A_BillingDocument('{BillingDocument}')/to_Partner / [partner_function.go](https://github.com/latonaio/sap-api-integrations-billing-document-reads/blob/main/SAP_API_Caller/responses/partner_function.go)

## Procurement Management ##

### Supplier Master ###

* A_BusinessPartner / [general.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads-supplier/blob/main/SAP_API_Caller/responses/general.go)
* A_BusinessPartnerRole / [role.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads-supplier/blob/main/SAP_API_Caller/responses/role.go)
* A_BusinessPartnerAddress / [address.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads-supplier/blob/main/SAP_API_Caller/responses/address.go)
* A_BusinessPartnerBank / [bank.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads-supplier/blob/main/SAP_API_Caller/responses/bank.go)
* A_Supplier / [supplier.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads-supplier/blob/main/SAP_API_Caller/responses/supplier.go)
* A_SupplierPurchasingOrg / [purchasing_organization.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads-supplier/blob/main/SAP_API_Caller/responses/purchasing_organization.go)
* A_SupplierCompany / [company.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads-supplier/blob/main/SAP_API_Caller/responses/company.go)
* ToRole / [to_role.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads-supplier/blob/main/SAP_API_Caller/responses/to_role.go)
* ToAddress / [to_address.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads-supplier/blob/main/SAP_API_Caller/responses/to_address.go)
* ToBank / [to_bank.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads-supplier/blob/main/SAP_API_Caller/responses/to_bank.go)
* ToSupplier / [to_supplier.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads-supplier/blob/main/SAP_API_Caller/responses/to_supplier.go)
* ToPurchasingOrganization / [to_purchasing_organization.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads-supplier/blob/main/SAP_API_Caller/responses/to_purchasing_organization.go)
* ToPartnerFunction / [to_partner_function.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads-supplier/blob/main/SAP_API_Caller/responses/to_partner_function.go)
* ToCompany / [to_company.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads-supplier/blob/main/SAP_API_Caller/responses/to_company.go)

### Purchasing Source List ###
* A_PurchasingSource / [purchasing_source_list.go](https://github.com/latonaio/sap-api-integrations-purchasing-source-list-reads/blob/main/SAP_API_Caller/responses/purchasing_source_list.go)

### Purchasing Info Record ###
* A_PurchasingInfoRecord / [general.go](https://github.com/latonaio/sap-api-integrations-purchasing-info-record-reads/blob/main/SAP_API_Caller/responses/general.go)
* A_PurchasingOrganizationPlant / [purchasing_organization_plant.go](https://github.com/latonaio/sap-api-integrations-purchasing-info-record-reads/blob/main/SAP_API_Caller/responses/purchasing_organization_plant.go)
* ToPurgInfoRecdOrgPlantData / [to_purg_info_recd_org_plant_data.go](https://github.com/latonaio/sap-api-integrations-purchasing-info-record-reads/blob/main/SAP_API_Caller/responses/to_purg_info_recd_org_plant_data.go)
* ToPurInfoRecdPrcgCndnValidity / [to_pur_info_recd_prcg_cndn_validity.go](https://github.com/latonaio/sap-api-integrations-purchasing-info-record-reads/blob/main/SAP_API_Caller/responses/to_pur_info_recd_prcg_cndn_validity.go)
* to_pur_info_recd_prcg_cndn_validity / [to_pur_info_recd_prcg_cndn.go](https://github.com/latonaio/sap-api-integrations-purchasing-info-record-reads/blob/main/SAP_API_Caller/responses/to_pur_info_recd_prcg_cndn.go)

### Purchasing Requisition ###
* A_PurchaseRequisitionHeader / [header.go](https://github.com/latonaio/sap-api-integrations-purchase-requisition-reads/blob/main/SAP_API_Caller/responses/header.go)
* A_PurchaseRequisitionItem / [item.go](https://github.com/latonaio/sap-api-integrations-purchase-requisition-reads/blob/main/SAP_API_Caller/responses/item.go)
* A_PurReqAddDelivery / [item_delivery_address.go](https://github.com/latonaio/sap-api-integrations-purchase-requisition-reads/blob/main/SAP_API_Caller/responses/item_delivery_address.go)
* A_PurReqnAcctAssgmt / [item_account.go](https://github.com/latonaio/sap-api-integrations-purchase-requisition-reads/blob/main/SAP_API_Caller/responses/item_account.go)
* ToItem / [to_item.go](https://github.com/latonaio/sap-api-integrations-purchase-requisition-reads/blob/main/SAP_API_Caller/responses/to_item.go)
* ToItemDeliveryAddress / [to_item_delivery_address.go](https://github.com/latonaio/sap-api-integrations-purchase-requisition-reads/blob/main/SAP_API_Caller/responses/to_item_delivery_address.go)
* ToItemAccount / [to_item_account.go](https://github.com/latonaio/sap-api-integrations-purchase-requisition-reads/blob/main/SAP_API_Caller/responses/to_item_account.go)

### Purchase Order ###
* A_PurchaseOrder / [header.go](https://github.com/latonaio/sap-api-integrations-purchase-order-reads/blob/main/SAP_API_Caller/responses/header.go)
* A_PurchaseOrderItem / [item.go](https://github.com/latonaio/sap-api-integrations-purchase-order-reads/blob/main/SAP_API_Caller/responses/item.go)
* A_PurchaseOrderScheduleLine / [item_shedule_line.go](https://github.com/latonaio/sap-api-integrations-purchase-order-reads/blob/main/SAP_API_Caller/responses/item_shedule_line.go)
* A_PurOrdPricingElement / [item_pricing_element.go](https://github.com/latonaio/sap-api-integrations-purchase-order-reads/blob/main/SAP_API_Caller/responses/item_pricing_element.go)
* A_PurOrdAccountAssignment / [item_account.go](https://github.com/latonaio/sap-api-integrations-purchase-order-reads/blob/main/SAP_API_Caller/responses/item_account.go)
* ToItem / [to_item.go](https://github.com/latonaio/sap-api-integrations-purchase-order-reads/blob/main/SAP_API_Caller/responses/to_item.go)
* ToItemScheduleLine / [to_item_shedule_line.go](https://github.com/latonaio/sap-api-integrations-purchase-order-reads/blob/main/SAP_API_Caller/responses/to_item_shedule_line.go)
* ToItemPricingElement / [to_item_pricing_element.go](https://github.com/latonaio/sap-api-integrations-purchase-order-reads/blob/main/SAP_API_Caller/responses/to_item_pricing_element.go)
* ToItemAccount / [to_item_account.go](https://github.com/latonaio/sap-api-integrations-purchase-order-reads/blob/main/SAP_API_Caller/responses/to_item_account.go)

### Purchase Contract ###
* A_PurchaseContract / [header.go](https://github.com/latonaio/sap-api-integrations-purchase-contract-reads/blob/main/SAP_API_Caller/responses/header.go)
* A_PurchaseContractItem / [item.go](https://github.com/latonaio/sap-api-integrations-purchase-contract-reads/blob/main/SAP_API_Caller/responses/item.go)
* ToItem / [to_item.go](https://github.com/latonaio/sap-api-integrations-purchase-contract-reads/blob/main/SAP_API_Caller/responses/to_item.go)
* ToItemAddress / [to_item_address.go](https://github.com/latonaio/sap-api-integrations-purchase-contract-reads/blob/main/SAP_API_Caller/responses/to_item_address.go)
* ToItemCondition / [to_item_condition.go](https://github.com/latonaio/sap-api-integrations-purchase-contract-reads/blob/main/SAP_API_Caller/responses/to_item_condition.go)

### Purchase Scheduling Agreement ###
* A_SchAgrmtHeader / [header.go](https://github.com/latonaio/sap-api-integrations-purchase-scheduling-agreement-reads/blob/main/SAP_API_Caller/responses/header.go)
* A_SchAgrmtItem  / [item.go](https://github.com/latonaio/sap-api-integrations-purchase-scheduling-agreement-reads/blob/main/SAP_API_Caller/responses/item.go)
* ToHeaderPartner / [to_header_partner](https://github.com/latonaio/sap-api-integrations-purchase-scheduling-agreement-reads/blob/main/SAP_API_Caller/responses/to_header_partner.go)
* ToItem / [to_item.go](https://github.com/latonaio/sap-api-integrations-purchase-scheduling-agreement-reads/blob/main/SAP_API_Caller/responses/to_item.go)
* ToItemDeliveryAddress / [to_item_delivery_address.go](https://github.com/latonaio/sap-api-integrations-purchase-scheduling-agreement-reads/blob/main/SAP_API_Caller/responses/to_item_delivery_address.go)
* ToItemScheduleLine / [to_item_schedule_line.go](https://github.com/latonaio/sap-api-integrations-purchase-scheduling-agreement-reads/blob/main/SAP_API_Caller/responses/to_item_schedule_line.go)

### Supplier Invoice ###
* A_SupplierInvoice / [header.go](https://github.com/latonaio/sap-api-integrations-supplier-invoice-reads/blob/main/SAP_API_Caller/responses/header.go)
* A_SupplierInvoice(SupplierInvoice='{SupplierInvoice}',FiscalYear='{FiscalYear}')/to_SupplierInvoiceItemGLAcct / [tax.go](https://github.com/latonaio/sap-api-integrations-supplier-invoice-reads/blob/main/SAP_API_Caller/responses/tax.go)
* A_SuplrInvcItemPurOrdRef / [purchase_order.go](https://github.com/latonaio/sap-api-integrations-supplier-invoice-reads/blob/main/SAP_API_Caller/responses/purchase_order.go)
* A_SuplrInvcItemAcctAssgmt / [account.go](https://github.com/latonaio/sap-api-integrations-supplier-invoice-reads/blob/main/SAP_API_Caller/responses/account.go)

### Bill Of Material ###
* MaterialBOM / [header.go](https://github.com/latonaio/sap-api-integrations-bill-of-material-reads/blob/main/SAP_API_Caller/responses/header.go)
* MaterialBOMItem / [item.go](https://github.com/latonaio/sap-api-integrations-bill-of-material-reads/blob/main/SAP_API_Caller/responses/item.go)
* ToItem / [to_item.go](https://github.com/latonaio/sap-api-integrations-bill-of-material-reads/blob/main/SAP_API_Caller/responses/to_item.go)

### Work Center ###
* WorkCenterCapacity(WorkCenterInternalID='{WorkCenterInternalID}',WorkCenterTypeCode='{WorkCenterTypeCode}',CapacityCategoryAllocation='{CapacityCategoryAllocation}',CapacityInternalID='{CapacityInternalID}')/_Header / [work_center.go](https://github.com/latonaio/sap-api-integrations-work-center-reads/blob/main/SAP_API_Caller/responses/work_center.go)

### Production Routing ###
* ProductionRoutingHeader / [header.go](https://github.com/latonaio/sap-api-integrations-production-routing-reads/blob/main/SAP_API_Caller/responses/header.go)
* ProductionRoutingMatlAssgmt / [material_assignment.go](https://github.com/latonaio/sap-api-integrations-production-routing-reads/blob/main/SAP_API_Caller/responses/material_assignment.go)
* ToMatlAssgmt / [to_matl_assgmt.go](https://github.com/latonaio/sap-api-integrations-production-routing-reads/blob/main/SAP_API_Caller/responses/to_matl_assgmt.go)
* ToOperation / [to_operation.go](https://github.com/latonaio/sap-api-integrations-production-routing-reads/blob/main/SAP_API_Caller/responses/to_operation.go)
* ToSequence / [to_sequence.go](https://github.com/latonaio/sap-api-integrations-production-routing-reads/blob/main/SAP_API_Caller/responses/to_sequence.go)
* ToComponentAllocation / [to_component_allocation.go](https://github.com/latonaio/sap-api-integrations-production-routing-reads/blob/main/SAP_API_Caller/responses/to_component_allocation.go)

### Planned Independent Requirement ###
* PlannedIndepRqmt / [header.go](https://github.com/latonaio/sap-api-integrations-planned-independent-requirement-reads/blob/main/SAP_API_Caller/responses/header.go)
* ToItem / [to_item.go](https://github.com/latonaio/sap-api-integrations-planned-independent-requirement-reads/blob/main/SAP_API_Caller/responses/to_item.go)

### Planned Order ###
* PlannedOrderHeader / [header.go](https://github.com/latonaio/sap-api-integrations-planned-order-reads/blob/main/SAP_API_Caller/responses/header.go)
* PlannedOrderComponent / [component.go](https://github.com/latonaio/sap-api-integrations-planned-order-reads/blob/main/SAP_API_Caller/responses/component.go)

### Production Order ###
* A_ProductionOrder_2 / [general.go](https://github.com/latonaio/sap-api-integrations-production-order-reads/blob/main/SAP_API_Caller/responses/general.go)
* ToProductionOrderStatus / [to_production_order_status.go](https://github.com/latonaio/sap-api-integrations-production-order-reads/blob/main/SAP_API_Caller/responses/to_production_order_status.go)
* ToProductionOrderComponent / [to_production_order_component.go](https://github.com/latonaio/sap-api-integrations-production-order-reads/blob/main/SAP_API_Caller/responses/to_production_order_component.go)
* ToProductionOrderOperation / [to_production_order_operation.go](https://github.com/latonaio/sap-api-integrations-production-order-reads/blob/main/SAP_API_Caller/responses/to_production_order_operation.go)
* ToProductionOrderItem / [to_production_order_item.go](https://github.com/latonaio/sap-api-integrations-production-order-reads/blob/main/SAP_API_Caller/responses/to_production_order_item.go)

### Production Order Confirmation ###
* ProdnOrdConf2 / [confirmation.go](https://github.com/latonaio/sap-api-integrations-production-order-confirmation-reads/blob/main/SAP_API_Caller/responses/confirmation.go)
* ProdnOrdConfMatlDocItm / [material_movements.go](https://github.com/latonaio/sap-api-integrations-production-order-confirmation-reads/blob/main/SAP_API_Caller/responses/material_movements.go)
* ProdnOrderConfBatchCharc / [batch_characteristic.go](https://github.com/latonaio/sap-api-integrations-production-order-confirmation-reads/blob/main/SAP_API_Caller/responses/batch_characteristic.go)
* ToMaterialMovements / [to_material_movements.go](https://github.com/latonaio/sap-api-integrations-production-order-confirmation-reads/blob/main/SAP_API_Caller/responses/to_material_movements.go)
* ToBatchCharacteristic / [to_batch_characteristic.go](https://github.com/latonaio/sap-api-integrations-production-order-confirmation-reads/blob/main/SAP_API_Caller/responses/to_batch_characteristic.go)
