# 📦 SimpleInventoryPy

A beginner-friendly, Excel-based inventory management system built with Python. Track products, manage stock levels, generate PDF reports, and control user access (Admin/Staff mode) — all in one simple script!

---

## 🧰 Features

✅ Add new products  
✅ Update stock with remarks  
✅ Edit existing product info  
✅ Delete products (admin-only, only if stock = 0)  
✅ Auto-status for low stock  
✅ Export inventory report to PDF  
✅ View inventory in the console  
✅ Track stock history in a `Logs` sheet  
✅ Search products by ID or Name  
✅ Role-based access (Admin / Staff)  

---

## 🔐 User Roles

| Role   | Permissions                                   |
|--------|-----------------------------------------------|
| Admin  | Full access: add, update, edit, delete, view |
| Staff  | Limited access: add, update, view, search     |

> Staff **cannot delete or edit products**

---

## 📁 Excel File Structure

The script uses a file called `inventory.xlsx` with two sheets:

### `Sheet1` (Main Inventory)

| Product ID | Product Name | Stock | Unit | Last Updated | Status |
|------------|--------------|-------|------|---------------|--------|

### `Logs` (Auto-created)

| Date | Product ID | Change | New Stock | Action | Remark/User |

---

## 📦 Requirements

Install required packages via pip:

```bash
pip install openpyxl reportlab
