# CounterDesk business workflow

CounterDesk is an offline desktop retail pilot for general stores, cosmetics and stationery counters.

## Catalog and opening stock

Create products with a unique SKU/barcode, category, unit, purchase cost, selling price and opening stock. Prices are references for new documents; saved item lines preserve their transaction prices. Product photos are optional. Opening/adjusted stock is a direct quantity edit, not a purchase or stock-count document.

Add supplier and customer contacts. Give every purchase and bill a traceable reference. Select a named customer whenever a balance will remain unpaid.

## Receiving stock

Create a Supplier purchase with supplier, received date and line items. Confirm actual purchase prices: reference cost is only a starting value. Saving increases product quantities atomically and computes the total from lines. Record money already paid to the supplier; further supplier payments use the same payment collection action on that purchase. These amounts are purchasing outflows, not customer revenue.

## Selling and collecting

Create a Sales record, add products and quantities, verify the line prices and initial payment. Saving computes the bill and deducts stock; insufficient quantities must be rejected by the shared store. Print the invoice. Use Collect payment for later customer receipts and mark the sale Completed when finished.

Unpaid cancellation reverses the transaction's stock movement. A purchase cannot safely be cancelled if its stock has already been consumed by later sales. Paid documents cannot be cancelled because the pilot has no refund module. Keep refunds and exceptional adjustments outside the pilot with supporting records until that workflow is implemented.

## Reports and limits

Purchases, sales and expenses are separate ledgers. Sales totals are not profit; this pilot does not compute cost of goods, taxes, discounts or stock valuation. SKU entry exists but there is no dedicated scan-to-cart barcode screen. Batch expiry, serial tracking, electronic scales, purchase returns, refunds and stock-adjustment history are not implemented. Verify opening stock and reconciliation in a shop trial.

Initial payments explicitly select cash, card or bank. This choice belongs to the receipt created with the record; later collections choose their own method and do not rewrite earlier payment entries.

The initial retail pilot uses whole-unit stock and line quantities. Fractional weight/volume sales need a later workflow.
