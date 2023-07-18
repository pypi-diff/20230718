# Comparing `tmp/odoo12_addon_epi-12.0.0.0.1.99.dev7-py3-none-any.whl.zip` & `tmp/odoo12_addon_epi-12.0.0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,13 @@
-Zip file size: 6065 bytes, number of entries: 9
+Zip file size: 8906 bytes, number of entries: 11
 -rw-r--r--  2.0 unx        0 b- defN 23-Jan-13 10:32 odoo/addons/epi/__init__.py
--rw-r--r--  2.0 unx      429 b- defN 23-Feb-10 15:16 odoo/addons/epi/__manifest__.py
--rw-r--r--  2.0 unx     7331 b- defN 23-Feb-10 15:16 odoo/addons/epi/views/report_invoice.xml
+-rw-r--r--  2.0 unx      429 b- defN 23-Jul-18 10:47 odoo/addons/epi/__manifest__.py
+-rw-r--r--  2.0 unx     5856 b- defN 23-Feb-16 16:53 odoo/addons/epi/i18n/ca_ES.po
+-rw-r--r--  2.0 unx     5844 b- defN 23-Jul-17 15:55 odoo/addons/epi/i18n/es.po
+-rw-r--r--  2.0 unx     9199 b- defN 23-May-04 12:20 odoo/addons/epi/views/report_invoice.xml
 -rw-r--r--  2.0 unx     1388 b- defN 23-Feb-10 15:16 odoo/addons/epi/views/report_templates.xml
--rw-r--r--  2.0 unx     5999 b- defN 23-Feb-10 15:16 odoo/addons/epi/views/sale_report_templates.xml
--rw-r--r--  2.0 unx      478 b- defN 23-Feb-10 15:17 odoo12_addon_epi-12.0.0.0.1.99.dev7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-10 15:17 odoo12_addon_epi-12.0.0.0.1.99.dev7.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Feb-10 15:17 odoo12_addon_epi-12.0.0.0.1.99.dev7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      852 b- defN 23-Feb-10 15:17 odoo12_addon_epi-12.0.0.0.1.99.dev7.dist-info/RECORD
-9 files, 16574 bytes uncompressed, 4553 bytes compressed:  72.5%
+-rw-r--r--  2.0 unx    10096 b- defN 23-May-04 12:01 odoo/addons/epi/views/sale_report_templates.xml
+-rw-r--r--  2.0 unx      470 b- defN 23-Jul-18 10:49 odoo12_addon_epi-12.0.0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-18 10:49 odoo12_addon_epi-12.0.0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jul-18 10:49 odoo12_addon_epi-12.0.0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      990 b- defN 23-Jul-18 10:49 odoo12_addon_epi-12.0.0.0.2.dist-info/RECORD
+11 files, 34369 bytes uncompressed, 7196 bytes compressed:  79.1%
```

## zipnote {}

```diff
@@ -1,28 +1,34 @@
 Filename: odoo/addons/epi/__init__.py
 Comment: 
 
 Filename: odoo/addons/epi/__manifest__.py
 Comment: 
 
+Filename: odoo/addons/epi/i18n/ca_ES.po
+Comment: 
+
+Filename: odoo/addons/epi/i18n/es.po
+Comment: 
+
 Filename: odoo/addons/epi/views/report_invoice.xml
 Comment: 
 
 Filename: odoo/addons/epi/views/report_templates.xml
 Comment: 
 
 Filename: odoo/addons/epi/views/sale_report_templates.xml
 Comment: 
 
-Filename: odoo12_addon_epi-12.0.0.0.1.99.dev7.dist-info/METADATA
+Filename: odoo12_addon_epi-12.0.0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: odoo12_addon_epi-12.0.0.0.1.99.dev7.dist-info/WHEEL
+Filename: odoo12_addon_epi-12.0.0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: odoo12_addon_epi-12.0.0.0.1.99.dev7.dist-info/top_level.txt
+Filename: odoo12_addon_epi-12.0.0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo12_addon_epi-12.0.0.0.1.99.dev7.dist-info/RECORD
+Filename: odoo12_addon_epi-12.0.0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/epi/__manifest__.py

```diff
@@ -1,10 +1,10 @@
 {
     'name': "Odoo Epi customizations",
-    'version': '12.0.0.0.1',
+    'version': '12.0.0.0.2',
     'depends': ['account'],
     'author': "Coopdevs Treball SCCL",
     'website': 'https://coopdevs.org',
     'category': "Cooperative management",
     'description': "Odoo Epi customizations",
     "license": "AGPL-3",
     'data': [
```

## odoo/addons/epi/views/report_invoice.xml

### odoo/addons/epi/views/report_invoice.xml

```diff
@@ -1,98 +1,144 @@
 <?xml version="1.0" encoding="utf-8"?>
 <odoo>
   <data>
     <template id="epi_report_invoice_document" inherit_id="account.report_invoice_document">
+      <t t-set="o" t-value="o.with_context(lang=lang)"/>
       <xpath expr="//div[@class='page']" position="replace">
-        <div class="page">
+        <div name="wrapper" style="min-height:100%; position:relative;">
           <div class="row pt-1" style="border-top: 1px solid #bbb; font-size: 14px;">
             <div id="invoice_no" class="col-6">
               <p>
-                <strong t-if="o.type == 'out_invoice' and o.state in ('open', 'in_payment', 'paid')">Factura</strong>
+                <strong t-if="o.type == 'out_invoice' and o.state in ('open', 'in_payment', 'paid')">Invoice</strong>
+                <strong t-if="o.type == 'out_invoice' and o.state == 'draft'">Draft Invoice</strong>
+                <strong t-if="o.type == 'out_invoice' and o.state == 'cancel'">Cancelled Invoice</strong>
+                <strong t-if="o.type == 'out_refund'">Credit Note</strong>
+                <strong t-if="o.type == 'in_refund'">Vendor Credit Note</strong>
+                <strong t-if="o.type == 'in_invoice'">Vendor Bill</strong>
                 <span t-field="o.number"/>
               </p>
             </div>
             <div id="date" class="col-6">
               <div t-if="o.date_invoice" name="invoice_date">
                 <strong class="float-right">
-                  Data
+                  Invoice Date
                   <span t-field="o.date_invoice"/>
                 </strong>
               </div>
             </div>
           </div>
           <div class="row pb-1" style="border-bottom: 2px solid #bbb; font-size: 14px;">
             <div class="col-12" t-if="o.date_due and o.type == 'out_invoice' and o.state in ('open', 'in_payment', 'paid')" name="due_date">
               <p class="text-right">
-                Data de venciment
+                Due Date
                 <span t-field="o.date_due"/>
               </p>
             </div>
           </div>
           <div class="row py-3" style="font-size: 14px;">
             <div id="client_details" class="col-6">
               <strong t-field="o.partner_id.name"/>
               <p class="m-0" t-field="o.partner_id.street"/>
               <p class="m-0" t-field="o.partner_id.city"/>
               <p class="m-0" t-field="o.partner_id.country_id"/>
               <p class="m-0" t-field="o.partner_id.vat"/>
             </div>
             <div id="bank_account" class="col-6">
-              <strong class="float-right">Pagament per transferència al compte</strong>
+              <strong class="float-right">Payment by bank transference</strong>
               <p class="float-right" t-field="o.partner_bank_id"/>
             </div>
           </div>
-          <table style="font-size: 14px;">
-            <thead style="border-bottom: 2px solid #bbb;">
-              <tr>
-                <th name="th_description" class="col-3">
-                  <span>Nom de producte o servei</span>
-                </th>
-                <th name="th_quantity" class="col-3">
-                  <span>Quantitat</span>
-                </th>
-                <th name="th_priceunit" class="col-3">
-                  <span>Preu</span>
-                </th>
-                <th name="th_subtotal" class="col-3">
-                  <span>Import</span>
-                </th>
-              </tr>
-            </thead>
-            <tbody>
-              <t t-foreach="o.invoice_line_ids" t-as="line">
-                <tr t-att-class="'bg-200 font-weight-bold o_line_section' if line.display_type == 'line_section' else 'font-italic o_line_note' if line.display_type == 'line_note' else ''">
-                  <t t-if="not line.display_type" name="account_invoice_line_accountable">
-                    <td class="col-3" name="account_invoice_line_name">
-                      <span t-field="line.name"/>
-                    </td>
-                    <td class="col-3 text-right">
-                      <span t-field="line.quantity"/>
-                    </td>
-                    <td class="col-3 text-right">
-                      <span t-field="line.price_unit"/>
-                    </td>
-                    <td class="col-3 text-right">
-                      <span t-field="line.price_unit"/>
-                    </td>
+          <div name="container" style="width:960px; margin:0 auto; padding-bottom:150px; min-height:800px;">
+            <t t-set="display_discount" t-value="any([l.discount for l in o.invoice_line_ids])"/>
+            <table style="font-size: 14px;">
+              <thead style="border-bottom: 2px solid #bbb;">
+                <tr>
+                  <th name="th_description" class="col-3">
+                    <span>Description</span>
+                  </th>
+                  <th name="th_quantity" class="col-3">
+                    <span>Quantity</span>
+                  </th>
+                  <th name="th_priceunit" class="col-3">
+                    <span>Price</span>
+                  </th>
+                  <t t-if="display_discount">
+                    <th name="th_discount" class="col-3">
+                      <span>Discount</span>
+                    </th>
                   </t>
+                  <th name="th_subtotal" class="col-3">
+                    <span>Amount</span>
+                  </th>
                 </tr>
-              </t>
-            </tbody>
-          </table>
-          <div style="border-top: 1px solid #bbb; font-size: 14px; width: 100%; position: absolute; top: 750px;">
+              </thead>
+              <tbody>
+                <t t-foreach="o.invoice_line_ids" t-as="line">
+                  <tr t-att-class="'bg-200 font-weight-bold o_line_section' if line.display_type == 'line_section' else 'font-italic o_line_note' if line.display_type == 'line_note' else ''">
+                    <t t-if="not line.display_type" name="account_invoice_line_accountable">
+                      <td class="col-3" name="account_invoice_line_name">
+                        <span t-field="line.name"/>
+                      </td>
+                      <td class="col-3 text-right">
+                        <span t-field="line.quantity" t-options="{'widget': 'float', 'precision': 0}"/>
+                      </td>
+                      <td class="col-3 text-right">
+                        <span t-field="line.price_unit" t-options="{'widget': 'monetary', 'display_currency': o.currency_id}"/>
+                      </td>
+                      <t t-if="display_discount">
+                        <td class="col-3 text-right">
+                          <span t-field="line.discount"/>
+                          %
+                        </td>
+                      </t>
+                      <td class="col-3 text-right">
+                        <span t-field="line.price_subtotal" t-options="{'widget': 'monetary', 'display_currency': o.currency_id}"/>
+                      </td>
+                    </t>
+                    <t t-if="line.display_type == 'line_section'">
+                      <td colspan="99">
+                        <span t-field="line.name"/>
+                      </td>
+                      <t t-set="current_section" t-value="line"/>
+                      <t t-set="current_subtotal" t-value="0"/>
+                    </t>
+                    <t t-if="line.display_type == 'line_note'">
+                      <td colspan="99">
+                        <span class="font-weight-bold">NOTE</span>
+                        <span t-field="line.name"/>
+                      </td>
+                    </t>
+                  </tr>
+                </t>
+              </tbody>
+            </table>
+          </div>
+          <div style="border-top: 1px solid #bbb; font-size: 14px; height: 100px; width: 100%; position: absolute; bottom: 0;">
             <div class="row">
               <p class="col-8"/>
               <p class="col-2 text-right">Subtotal</p>
               <span class="col-2 text-right" t-field="o.amount_untaxed"/>
             </div>
             <div class="row">
-              <p class="col-8"/>
-              <p class="col-2 text-right">IVA 21%</p>
-              <span class="col-2 text-right" t-field="o.amount_tax"/>
+              <t t-foreach="o.amount_by_group" t-as="amount_by_group">
+                <t t-if="len(o.tax_line_ids) == 1 and o.amount_untaxed == amount_by_group[2]">
+                  <p class="col-8"/>
+                  <p class="col-2 text-right" t-esc="amount_by_group[0]"/>
+                  <span class="col-2 text-right" t-esc="amount_by_group[3]"/>
+                </t>
+                <t t-else="">
+                  <span t-esc="amount_by_group[0]"/>
+                  <span>
+                    &amp;nbsp;
+                    <span>on</span>
+                    <t t-esc="amount_by_group[4]"/>
+                  </span>
+                  <span t-esc="amount_by_group[3]"/>
+                </t>
+              </t>
             </div>
             <div class="row bg-light pt-2">
               <p class="col-8"/>
               <p class="col-2 text-right font-weight-bold">Import total</p>
               <span class="col-2 text-right font-weight-bold" t-field="o.amount_total"/>
             </div>
           </div>
@@ -100,49 +146,13 @@
           <div id="total">
             <div>
               <table/>
             </div>
           </div>
         </div>
         <div class="footer o_standard_footer">
-          <div class="text-center" style="padding-top: 2px; font-size: 12px;">ENERGÍA POR LA IGUALDAD, SCCL, Ins. al Reg. General de Cooperatives de Catalunya, Inscripció 14.751 com a Serveis.</div>
+          <div class="text-center" style="padding-top: 20px; font-size: 12px;">ENERGÍA POR LA IGUALDAD, SCCL, Ins. al Reg. General de Cooperatives de Catalunya, Inscripció 14.751 com a Serveis.</div>
         </div>
       </xpath>
     </template>
-    <template id="web.external_layout_standard">
-      <div class="header">
-        <div class="row">
-          <div class="col-5 mb4">
-            <img t-if="company.logo" t-att-src="image_data_uri(company.logo)" style="width:346px;height:149px" alt="Logo"/>
-          </div>
-          <div class="col-7" name="company_address">
-            <div style="margin: 10px; padding:10px; border: solid black 1px; font-size: 14px; line-height: 30px;">
-              <div>
-                <strong>NIF:</strong>
-                F-66799057
-              </div>
-              <div>
-                <strong>OFICINA CENTRAL:</strong>
-                Av. Estatut, 130, 08191, Rubí
-              </div>
-              <div>
-                <strong>SEU SOCIAL:</strong>
-                Primer de Maig, 1, 3r B, 43870, Amposta
-              </div>
-              <div>
-                <strong>CONTACTE:</strong>
-                93 193 73 90 · suma@epi.coop
-              </div>
-            </div>
-          </div>
-          <div class="col-9 text-right" style="margin-top:22px;" t-field="company.report_header" name="moto"/>
-        </div>
-      </div>
-      <div class="article o_report_layout_standard" t-att-data-oe-model="o and o._name" t-att-data-oe-id="o and o.id" t-att-data-oe-lang="o and o.env.context.get('lang')">
-        <t t-raw="0"/>
-      </div>
-      <div class="footer o_standard_footer">
-        <div class="text-center" style="border: 1px solid black; padding-top: 2px; font-size: 12px;">ENERGÍA POR LA IGUALDAD, SCCL, Ins. al Reg. General de Cooperatives de Catalunya, Inscripció 14.751 com a Serveis.</div>
-      </div>
-    </template>
   </data>
 </odoo>
```

## odoo/addons/epi/views/sale_report_templates.xml

### odoo/addons/epi/views/sale_report_templates.xml

```diff
@@ -1,83 +1,130 @@
 <?xml version="1.0" encoding="utf-8"?>
 <odoo>
   <data>
     <template id="epi_report_saleorder_document" inherit_id="sale.report_saleorder_document">
+      <t t-set="doc" t-value="doc.with_context(lang=doc.partner_id.lang)"/>
       <xpath expr="//div[@class='page']" position="replace">
-        <div class="page">
+        <div name="wrapper" style="min-height:100%; position:relative;">
           <div class="row pt-1" style="border-top: 1px solid #bbb; border-bottom: 2px solid #bbb; font-size: 14px;">
             <div id="quotation_no" class="col-6">
-              <p>
-                <span class="font-weight-bold">Pressupost</span>
-                <span t-field="doc.name"/>
-              </p>
+              <t t-if="not (env.context.get('proforma', False) or is_pro_forma)">
+                <span t-if="doc.state not in ['draft','sent']">Order</span>
+                <span t-if="doc.state in ['draft','sent']">Quotation</span>
+              </t>
+              <t t-if="env.context.get('proforma', False) or is_pro_forma">
+                <span>Pro-Forma Invoice</span>
+              </t>
+              <span t-field="doc.name"/>
             </div>
             <div id="date" class="col-6">
-              <div t-if="doc.date_order" name="quotation_date">
+              <div t-if="doc.confirmation_date and doc.state not in ['draft','sent']" name="order_date">
+                <p class="text-right">
+                  <span class="font-weight-bold">Order Date</span>
+                  <span t-field="doc.confirmation_date" t-options="{&quot;widget&quot;: &quot;date&quot;,&quot;format&quot;: &quot;dd/MM/yyyy&quot;}"/>
+                </p>
+              </div>
+              <div t-if="doc.date_order and doc.state in ['draft','sent']" name="quotation_date">
                 <p class="text-right">
-                  <span class="font-weight-bold">Data</span>
-                  <span t-field="doc.validity_date"/>
+                  <span class="font-weight-bold">Quotation Date</span>
+                  <span t-field="doc.date_order" t-options="{&quot;widget&quot;: &quot;date&quot;,&quot;format&quot;: &quot;dd/MM/yyyy&quot;}"/>
                 </p>
               </div>
             </div>
           </div>
           <div class="row py-3" style="font-size: 14px;">
             <div id="client_details" class="col-5">
               <strong t-field="doc.partner_id.name"/>
               <p class="m-0" t-field="doc.partner_id.street"/>
               <p class="m-0" t-field="doc.partner_id.city"/>
               <p class="m-0" t-field="doc.partner_id.country_id"/>
               <p class="m-0" t-field="doc.partner_id.vat"/>
             </div>
             <div id="bank_account" class="col-7">
-              <p class="m-0 text-right font-weight-bold">Condicions de pagament</p>
-              <p class="m-0 text-right">Pagament per transferència al compte</p>
+              <p class="m-0 text-right font-weight-bold">Payment conditions</p>
+              <p class="m-0 text-right">Payment by bank transference</p>
               <p class="m-0 text-right">ES96 3025 0014 0614 0006 8284</p>
-              <p class="m-0 text-right">Data de venciment (30 dies)</p>
+              <t t-if="doc.payment_term_id.name">
+                <p class="m-0 text-right">
+                  Due date (
+                  <span t-field="doc.payment_term_id.name"/>
+                  )
+                </p>
+              </t>
             </div>
           </div>
-          <table style="font-size: 14px;">
-            <thead style="border-bottom: 2px solid #bbb;">
-              <tr>
-                <th name="th_description" class="col-3">
-                  <span>Nom de producte o servei</span>
-                </th>
-                <th name="th_quantity" class="col-3">
-                  <span>Quantitat</span>
-                </th>
-                <th name="th_priceunit" class="col-3">
-                  <span>Preu</span>
-                </th>
-                <th name="th_subtotal" class="col-3">
-                  <span>Import</span>
-                </th>
-              </tr>
-            </thead>
-            <tbody>
-              <t t-foreach="doc.order_line" t-as="line">
-                <tr t-att-class="'bg-200 font-weight-bold o_line_section' if line.display_type == 'line_section' else 'font-italic o_line_note' if line.display_type == 'line_note' else ''">
-                  <t t-if="not line.display_type" name="account_invoice_line_accountable">
-                    <td class="col-3" name="account_invoice_line_name">
-                      <span t-field="line.name"/>
-                    </td>
-                    <td class="col-3 text-right">
-                      <span t-field="line.product_uom_qty"/>
-                    </td>
-                    <td class="col-3 text-right">
-                      <span t-field="line.price_unit"/>
-                    </td>
-                    <td class="col-3 text-right">
-                      <span t-field="line.price_unit"/>
-                    </td>
+          <div name="container" style="width:960px; margin:0 auto; padding-bottom:150px; min-height:580px;">
+            <t t-set="display_discount" t-value="any([l.discount for l in doc.order_line])"/>
+            <table style="font-size: 14px;">
+              <thead style="border-bottom: 2px solid #bbb;">
+                <tr>
+                  <th name="th_description" class="col-3">
+                    <span>Description</span>
+                  </th>
+                  <th name="th_quantity" class="col-3">
+                    <span>Quantity</span>
+                  </th>
+                  <th name="th_priceunit" class="col-3">
+                    <span>Price</span>
+                  </th>
+                  <t t-if="display_discount">
+                    <th name="th_discount" class="col-3" groups="sale.group_discount_per_so_line">
+                      <span>Discount</span>
+                    </th>
                   </t>
+                  <th name="th_subtotal" class="col-3">
+                    <span>Amount</span>
+                  </th>
                 </tr>
-              </t>
-            </tbody>
-          </table>
-          <div style="border-top: 1px solid #bbb; font-size: 14px; width: 100%; position: absolute; top: 550px;">
+              </thead>
+              <tbody>
+                <t t-set="current_subtotal" t-value="0"/>
+                <t t-foreach="doc.order_line" t-as="line">
+                  <t t-set="current_subtotal" t-value="current_subtotal + line.price_subtotal" groups="account.group_show_line_subtotals_tax_excluded"/>
+                  <t t-set="current_subtotal" t-value="current_subtotal + line.price_total" groups="account.group_show_line_subtotals_tax_included"/>
+                  <tr t-att-class="'bg-200 font-weight-bold o_line_section' if line.display_type == 'line_section' else 'font-italic o_line_note' if line.display_type == 'line_note' else ''">
+                    <t t-if="not line.display_type" name="account_invoice_line_accountable">
+                      <td class="col-3" name="account_invoice_line_name">
+                        <span t-field="line.name"/>
+                      </td>
+                      <td class="col-3 text-right">
+                        <span t-field="line.product_uom_qty" t-options="{'widget': 'float', 'precision': 0}"/>
+                      </td>
+                      <td class="col-3 text-right">
+                        <span t-field="line.price_unit" t-options="{'widget': 'monetary', 'display_currency': doc.currency_id}"/>
+                      </td>
+                      <t t-if="display_discount" groups="sale.group_discount_per_so_line">
+                        <td class="col-3 text-right">
+                          <span t-field="line.discount"/>
+                          %
+                        </td>
+                      </t>
+                      <td class="col-3 text-right">
+                        <span t-field="line.price_subtotal" groups="account.group_show_line_subtotals_tax_excluded" t-options="{'widget': 'monetary', 'display_currency': doc.currency_id}"/>
+                      </td>
+                    </t>
+                    <t t-if="line.display_type == 'line_section'">
+                      <td name="td_section_line" colspan="99">
+                        <span t-field="line.name"/>
+                      </td>
+                      <t t-set="current_section" t-value="line"/>
+                      <t t-set="current_subtotal" t-value="0"/>
+                    </t>
+                    <t t-if="line.display_type == 'line_note'">
+                      <td name="td_note_line" colspan="99">
+                        <span class="font-weight-bold">NOTE:</span>
+                        <span t-field="line.name"/>
+                      </td>
+                    </t>
+                  </tr>
+                </t>
+              </tbody>
+            </table>
+          </div>
+          <div style="border-top: 1px solid #bbb; font-size: 14px; height:100px; width: 100%; position: absolute; bottom: 0;">
             <div class="row">
               <p class="col-8"/>
               <p class="col-2 text-right">Subtotal</p>
               <span class="col-2 text-right" t-field="doc.amount_untaxed"/>
             </div>
             <div class="row">
               <p class="col-8"/>
@@ -85,21 +132,22 @@
               <span class="col-2 text-right" t-field="doc.amount_tax"/>
             </div>
             <div class="row bg-light pt-2 mb-2">
               <p class="col-8"/>
               <p class="col-2 text-right font-weight-bold">Import total</p>
               <span class="col-2 text-right font-weight-bold" t-field="doc.amount_total"/>
             </div>
-            <div class="row" style="border-bottom: 1px solid #bbb;">
-              <div class="col-12 mb-3">
-                <p class="m-0 font-weight-bold">Condicions:</p>
-                <p style="font-size: 12px;" class="m-0 font-weight-bold">10% Inici d'obra</p>
-                <p style="font-size: 12px;" class="mt-0 font-weight-bold">90% Finalització obra</p>
+            <t t-if="doc.note">
+              <div class="row" style="border-bottom: 1px solid #bbb;">
+                <div class="col-12 mb-3">
+                  <p class="m-0 font-weight-bold">Condicions:</p>
+                  <p style="font-size: 12px;" class="m-0 font-weight-bold" t-field="doc.note"/>
+                </div>
               </div>
-            </div>
+            </t>
             <div class="row">
               <div class="col-6 mt-3">
                 <p>Acceptació del pressupost</p>
                 <p class="m-0 font-weight-bold">RAÓ SOCIAL:</p>
                 <p class="m-0 font-weight-bold">RESPONSABLE:</p>
                 <p class="m-0 font-weight-bold">CÀRREC:</p>
                 <p class="m-0 font-weight-bold">DATA:</p>
```

## Comparing `odoo12_addon_epi-12.0.0.0.1.99.dev7.dist-info/RECORD` & `odoo12_addon_epi-12.0.0.0.2.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 odoo/addons/epi/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-odoo/addons/epi/__manifest__.py,sha256=oCBTa-BFOyurbyMr7gUwVWVuLfdVvutFmJzghbtpfRs,429
-odoo/addons/epi/views/report_invoice.xml,sha256=bv421hP0DtWpARDUvKGh4mIlk-95gJ8_42LOL8Bx7hg,7331
+odoo/addons/epi/__manifest__.py,sha256=8eulHfHChgZOk7QiCddhqjNjaAat3zsHRbiCWLz1oSw,429
+odoo/addons/epi/i18n/ca_ES.po,sha256=duiBgWt6xq_JgV6aVAWcDOk_47_td1KG2SX9BFOjgfE,5856
+odoo/addons/epi/i18n/es.po,sha256=O_ZLp8l59Yyz03T9eETC86WfowvhPPSElTRU4101Ouc,5844
+odoo/addons/epi/views/report_invoice.xml,sha256=-mRCykkYHUu87zEJnGI527F9ZQCQiR-Wo2YlDpUftKM,9199
 odoo/addons/epi/views/report_templates.xml,sha256=9vb1FQjbYJ0ogQfSc0AkT6sMw5bU1HZKtGDF--gZUJU,1388
-odoo/addons/epi/views/sale_report_templates.xml,sha256=gQG2PtMoRHY7x_m6BSsI2WPsBGSEbPay810GknNBsOE,5999
-odoo12_addon_epi-12.0.0.0.1.99.dev7.dist-info/METADATA,sha256=smG1cOEbkBmOdrmpaaLOR89AF7LM6DYiN46DhL5yLGw,478
-odoo12_addon_epi-12.0.0.0.1.99.dev7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-odoo12_addon_epi-12.0.0.0.1.99.dev7.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo12_addon_epi-12.0.0.0.1.99.dev7.dist-info/RECORD,,
+odoo/addons/epi/views/sale_report_templates.xml,sha256=XcSWe-LPoVQImhzn8G_aQrNX_01bjfe6RPvt7kiPQ24,10096
+odoo12_addon_epi-12.0.0.0.2.dist-info/METADATA,sha256=Gs58R3yBesTkNCH6Qjp7Rx9YpMtzIzPDFazUvL_gPHk,470
+odoo12_addon_epi-12.0.0.0.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+odoo12_addon_epi-12.0.0.0.2.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo12_addon_epi-12.0.0.0.2.dist-info/RECORD,,
```

