## Core idea

This system is designed around one core principle:
pricing and stock should be derived from actual events,
not from manual decisions.

The system treats humans as operators,
not as calculators.

## Pricing logic

Prices are calculated automatically based on product quantity.
If a discount condition is met, the system applies it without requiring
manual promotion selection.

This reduces human error and keeps pricing consistent.

## Stock model

Stock is updated only by events:
- sale
- stock-in
- transfer between warehouse and store

Direct manual stock editing is intentionally avoided.

## Warehouse and store separation

Warehouse stock and store stock are treated as separate entities.
A transfer is an explicit event that decreases warehouse stock
and increases store stock.

## Non-goals

This project does not aim to:
- support complex promotion trees
- provide a polished user interface
- replace enterprise POS systems
