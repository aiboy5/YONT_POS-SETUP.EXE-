# 🚀 YONT POS System - Complete Guide

**YONT POS** is a professional Point of Sale (POS) system designed for restaurants, cafes, shops, and retail businesses. It features a modern dark-themed interface with multilingual support (English, Shan, Myanmar), comprehensive inventory management, and advanced reporting capabilities.

---

## 📋 Table of Contents

1. [System Requirements](#system-requirements)
2. [Installation Guide](#installation-guide)
3. [Getting Started](#getting-started)
4. [Main Menu Overview](#main-menu-overview)
5. [Features & Modules](#features--modules)
6. [Settings Configuration](#settings-configuration)
7. [User Roles & Permissions](#user-roles--permissions)
8. [Troubleshooting](#troubleshooting)
9. [Support & Updates](#support--updates)

---

## 💻 System Requirements

### Minimum Requirements:
- **Operating System**: Windows 10 or later (64-bit)
- **RAM**: 4 GB minimum
- **Storage**: 2 GB free disk space
- **Display**: 1024x768 resolution minimum (recommended: 1920x1080 or higher for optimal experience)
- **Internet**: Optional (for email receipts and backups)

### Recommended Requirements:
- **Operating System**: Windows 11 (64-bit)
- **RAM**: 8 GB or more
- **Storage**: SSD (5 GB available)
- **Display**: Full HD (1920x1080) or higher
- **Printer**: Thermal receipt printer (ESC/POS compatible) or standard printer

---

## 📦 Installation Guide

### Step 1: Download the Installer

1. Obtain the **YONT_POS_Setup.exe** file from your vendor
2. Save it to your Desktop or Downloads folder

### Step 2: Pre-Installation Preparation

**IMPORTANT**: Follow these steps to ensure proper installation at **C:/YONT_POS**

1. **Create the installation folder**:
   - Press `Windows Key + R`
   - Type: `C:\` and press Enter
   - Right-click in empty space → **New** → **Folder**
   - Name the folder: `YONT_POS`
   - This creates: `C:\YONT_POS`

2. **Set folder permissions** (if prompted):
   - Right-click `C:\YONT_POS` folder
   - Select **Properties** → **Security** → **Edit**
   - Select your username
   - Click **Full Control** → **Apply** → **OK**

### Step 3: Run the Installer

1. **Close all running applications** (especially antivirus temporary scans)
2. **Double-click** `YONT_POS_Setup.exe`
3. **Windows may show a security warning**:
   - Click **"More info"** if prompted
   - Click **"Run anyway"**

### Step 4: Follow Installation Wizard

**Installation Step-by-Step**:

| Step | Action | Notes |
|------|--------|-------|
| **Welcome** | Click **Next** | Review license terms if shown |
| **Installation Path** | Type or Browse to: `C:\YONT_POS` | ⚠️ **CRITICAL**: Do NOT use `Program Files` |
| **Select Components** | Select all components | Keep defaults selected |
| **Shortcuts** | Choose preferred options | You can uncheck if you don't want desktop/start menu shortcuts |
| **Ready to Install** | Click **Install** | Installation will begin |
| **Completing Setup** | Click **Finish** | Application may launch automatically |

### Step 5: Verify Installation

After installation completes:

1. **Check installation folder**:
   - Press `Windows Key + E` (File Explorer)
   - Navigate to: `C:\YONT_POS`
   - Verify you see: `main.exe`, `settings.json`, fonts folder, locales folder, and other configuration files

2. **Create Database Backup** (IMPORTANT):
   - Create a folder: `C:\YONT_POS\backups`
   - This folder will store automatic backups of your database

3. **Verify shortcuts** (if created):
   - Desktop should have **YONT POS** shortcut
   - Start Menu → **YONT POS** folder with shortcuts

### Step 6: First Launch

1. **Double-click** the **YONT POS** icon on Desktop, OR
2. **Open Start Menu** → Find **YONT POS** → Click **YONT POS**
3. Wait for the application to load (first launch may take 5-10 seconds)

### Changing Installation Location

**If you accidentally installed to Program Files**:

1. Uninstall: Settings → Apps → Apps & Features → Find **YONT POS** → **Uninstall**
2. Delete: `C:\Program Files\YONT_POS` folder (if it exists)
3. Follow the installation steps above, but change the path to `C:\YONT_POS`

**DO NOT install to**:
- ❌ `Program Files` or `Program Files (x86)` (permission issues)
- ❌ Desktop (data loss risk)
- ❌ Temporary folders (auto-cleanup will delete data)

---

## 🔐 Getting Started

### First Login

**Default Admin Credentials** (First Time Only):

```
Username: admin
Password: admin123
```

⚠️ **IMPORTANT**: Change the default password immediately after first login!

### Login Screen

1. **Username**: Enter your username
2. **Password**: Enter your password
3. **Remember me**: Check to stay logged in on this computer
4. **Sign In**: Click to proceed

**After successful login**, you'll see the **Main Menu** with available options based on your user role.

---

## 🎯 Main Menu Overview

The main menu displays as a grid of colored cards. Each card represents a menu section. The menu items you see depend on your **user role** (Admin, Cashier, Manager, Inventory Manager).

### Admin View (All Modules)
An Admin user sees all available modules:

```
┌─────────────┬─────────────┬─────────────┬─────────────┐
│   Sales     │  Products   │   Reports   │    Bills    │
│    (Green)  │    (Blue)   │   (Orange)  │    (Blue)   │
├─────────────┼─────────────┼─────────────┼─────────────┤
│    Shift    │   Stock     │  Customers  │   Barcode   │
│  (Teal)     │ Manager(Y)  │   (Blue)    │  Manager(G) │
└─────────────┴─────────────┴─────────────┴─────────────┘
```

### Cashier View (Limited)
A Cashier user typically sees:

```
┌─────────────┬─────────────┐
│   Sales     │  Products   │
│    (Green)  │    (Blue)   │
└─────────────┴─────────────┘
```

### Menu Toolbar (Top Right)
Regardless of role, all users have:
- **Settings** icon (⚙️) - Access to configuration and preferences
- **Log out** button - Exit the application

---

## 📱 Features & Modules

### 1. 💳 **SALES** (Green Card)
**Purpose**: Process customer transactions and manage orders

**Features**:
- ✅ Create new sales orders
- ✅ Add products to cart
- ✅ Apply discounts
- ✅ Process payments
- ✅ Print receipts (optional thermal printer support)
- ✅ Email receipts to customers
- ✅ Void/return items
- ✅ Hold orders temporarily (for later)

**Who Can Access**: Admins, Cashiers, Managers
**Requires**: Active shift (for Cashiers)

**How to Use**:
1. Click **Sales** card
2. Select or create customer
3. Select products/items
4. Adjust quantities and prices if needed
5. Apply discounts if applicable
6. Proceed to checkout
7. Choose payment method
8. Print receipt or email to customer

---

### 2. 📦 **PRODUCTS** (Blue Card)
**Purpose**: Manage product catalog and inventory items

**Features**:
- ✅ Add new products
- ✅ Edit product details (name, price, category)
- ✅ Set product images
- ✅ Manage product categories
- ✅ Track product stock levels
- ✅ Set minimum stock alerts
- ✅ Search and filter products
- ✅ Bulk import/export products

**Who Can Access**: Admins, Managers
**Data Required**: Product name, price, category

**How to Use**:
1. Click **Products** card
2. View list of all products
3. **Add New**: Enter product details and click Save
4. **Edit**: Select product → Modify details → Save
5. **Delete**: Select product → Delete (careful: cannot undo)
6. **Search**: Use search bar to find products quickly

---

### 3. 📊 **REPORTS** (Orange/Accent Card)
**Purpose**: Generate sales and business analytics

**Features**:
- ✅ Daily/Weekly/Monthly sales reports
- ✅ Sales by category
- ✅ Top-selling products
- ✅ Revenue analysis
- ✅ Customer purchase history
- ✅ Payment method breakdown
- ✅ Profit analysis
- ✅ Export reports to Excel

**Who Can Access**: Admins, Managers
**Time Period**: Customizable date range

**How to Use**:
1. Click **Reports** card
2. Select report type from dropdown
3. Choose date range (Today, This Week, This Month, Custom)
4. Click **Generate Report**
5. View data in chart/table format
6. **Export**: Click Export button to save as Excel file

---

### 4. 💰 **BILLS** (Blue Card)
**Purpose**: Manage pending bills and partial payments

**Features**:
- ✅ View outstanding bills
- ✅ Track payment status
- ✅ Record partial payments
- ✅ Add notes to bills
- ✅ Bill reminders
- ✅ Payment history

**Who Can Access**: Admins, Managers
**Status**: Pending, Partial, Paid

**How to Use**:
1. Click **Bills** card
2. View pending bills list
3. Click bill to view details
4. Record payment → Enter amount → Submit
5. Mark as paid when complete

---

### 5. 🕐 **SHIFT** (Teal Card)
**Purpose**: Manage cashier shifts and cash handling

**Features**:
- ✅ Open new shift
- ✅ View active shifts
- ✅ Record shift start amount (float)
- ✅ Record shift end amount
- ✅ View sales during shift
- ✅ Close shift (with discrepancy reporting)
- ✅ Print shift summary

**Who Can Access**: Admins, Cashiers, Managers
**Requirement**: Cashiers MUST open shift before selling

**How to Use**:
1. Click **Shift** card
2. **Open Shift**: Enter starting cash amount → Confirm
3. Proceed with sales (only available when shift is active)
4. **Close Shift**: When finished for the day
   - Enter ending cash amount
   - System calculates discrepancies
   - Review and confirm

---

### 6. 📦 **STOCK MANAGER** (Yellow/Success Card)
**Purpose**: Track and manage inventory levels

**Features**:
- ✅ Add stock to products
- ✅ Remove stock (damage/loss)
- ✅ Track stock levels in real-time
- ✅ Low stock alerts
- ✅ Stock history/audit trail
- ✅ Physical count vs System count
- ✅ Transfer stock between locations
- ✅ Generate stock reports

**Who Can Access**: Admins, Inventory Managers, Managers
**Critical**: Keep accurate stock for accurate reports

**How to Use**:
1. Click **Stock Manager** card
2. Search for product by name/barcode
3. **Add Stock**:
   - Enter quantity
   - Add notes (optional)
   - Click Save
4. **Remove Stock**:
   - Enter quantity to remove
   - Select reason (damage/sale adjustment/loss)
   - Click Save
5. View stock history for each product

---

### 7. 👥 **CUSTOMERS** (Blue Card)
**Purpose**: Manage customer database and purchase history

**Features**:
- ✅ Add new customers
- ✅ View customer profile
- ✅ Track customer purchases
- ✅ Email address management
- ✅ Phone number tracking
- ✅ Customer loyalty points
- ✅ Credit management
- ✅ Customer notes

**Who Can Access**: Admins, Managers, Cashiers
**Uses**: Email receipts, loyalty tracking, credit sales

**How to Use**:
1. Click **Customers** card
2. **Add New Customer**:
   - Enter name
   - Enter email (for receipt sending)
   - Enter phone number
   - Add optional notes
   - Click Save
3. View customer purchase history
4. Update customer details

---

### 8. 📱 **BARCODE MANAGER** (Green Card)
**Purpose**: Manage product barcodes and QR codes

**Features**:
- ✅ Generate barcodes for products
- ✅ Print barcode labels
- ✅ Scan barcodes at POS
- ✅ Generate QR codes
- ✅ Bulk barcode printing
- ✅ Customize label format
- ✅ Import barcodes from CSV

**Who Can Access**: Admins
**Printer Required**: Label printer recommended

**How to Use**:
1. Click **Barcode Manager** card
2. Select products for barcodes
3. Choose barcode format (Code128, EAN-13, QR)
4. **Preview**: See how labels will look
5. **Print**: Send to barcode printer
6. Adjust label size/format if needed in Settings

---

## ⚙️ Settings Configuration

### How to Access Settings

**Option 1**: From Main Menu
- Click **Settings** button (⚙️) in top right

**Option 2**: Using Menu Bar
- Click **Menu** → **Settings**

### Settings Tabs

#### 1. **General Settings**
- Business name
- Currency (default: MMK)
- Language
- Date/Time format
- Default tax rate

#### 2. **Receipt Settings**
- Shop name for receipts
- Receipt header text
- Receipt footer text
- Logo position
- Paper width (80mm or 58mm thermal printers)
- Receipt company information

#### 3. **Printer Settings**
- Select printer type:
  - **Network Printer**: For standard office printers
  - **Thermal Printer**: For ESC/POS receipt printers
  - **PDF**: Save receipts as PDF files
- Configure printer margins
- Page size selection
- Test print function

#### 4. **Language Settings**
- Current language: English, Shan (မျ), Myanmar (ြ)
- Font selection for non-English text
- Text encoding

#### 5. **Password Settings**
- Change your user password
- Set password complexity requirements
- Force password change on next login

#### 6. **Colors & Themes**
- **Background Color**: Dark theme (default)
- **Text Color**: Light text for readability
- **Primary Color**: Main action button color (Green by default)
- **Secondary Color**: Secondary UI elements (Blue)
- **Accent Color**: Warning/Important elements (Orange)
- **Success Color**: Positive actions (Green)
- **Warning Color**: Cautions (Orange)
- **Error Color**: Errors/Deletions (Red)

#### 7. **Menu Colors**
- Customize individual menu card colors:
  - Sales button color
  - Products button color
  - Reports button color
  - Each menu item has its own color picker

#### 8. **Menu Layout**
- **Tile Width**: Width of menu cards (240px-400px)
- **Tile Height**: Height of menu cards (auto-calculated)
- **Tile Padding**: Space between cards
- **Icon Size**: Size of icons on menu cards
- **Text Size**: Font size for menu labels
- **Responsive Breakpoints**: Auto-adjust for screen size

#### 9. **User Roles & Permissions**
- **Manage Roles**: Admin, Cashier, Manager, Inventory Manager
- **Set Permissions** per role:
  - sales: Can process sales
  - products: Can manage products
  - reports: Can view reports
  - bills: Can manage bills
  - customers: Can manage customer database
  - stock: Can manage inventory
  - barcode: Can manage barcodes
  - shifts: Can open/close shifts
  - users: Can manage other users (Admin only)
  - settings: Can access settings

#### 10. **UI Settings**
- Window size/zoom level
- Start maximized option
- Animation speed
- Touch-friendly button sizes
- Font scaling

#### 11. **Advanced Settings**
- Backup location
- Auto-backup frequency
- Database optimization
- Clear application data (⚠️ Use with caution)
- Debug mode
- Log level

#### 12. **Email Settings** (Optional)
- **Gmail Integration**:
  - Enable email receipts
  - Configure Gmail account
  - SMTP settings
  - Email signature
- **Test Email**: Send test receipt to verify setup

---

## 👥 User Roles & Permissions

### Role Types and Access Levels

#### 1. **ADMIN** (Full Access)
A system administrator with complete control

| Feature | Access | Details |
|---------|--------|---------|
| Sales | ✅ Full | Can create/modify/void sales |
| Products | ✅ Full | Add/edit/delete products |
| Customers | ✅ Full | Manage all customer data |
| Reports | ✅ Full | View all business analytics |
| Stock Manager | ✅ Full | Full inventory control |
| Shifts | ✅ Full | Manage all shifts |
| Bills | ✅ Full | Full bill management |
| Barcode | ✅ Full | Create/print barcodes |
| Users | ✅ Full | Create/edit/delete users |
| Settings | ✅ Full | Access all settings |
| Backup | ✅ Full | Manual backup/restore |

**Can Do**:
- Override cashier restrictions
- Create/modify/delete users and roles
- Modify system settings and colors
- View all reports and analytics
- Manage entire inventory
- Sell without active shift (with confirmation)

---

#### 2. **CASHIER** (Limited Sales)
A checkout operator for processing customer transactions

| Feature | Access | Details |
|---------|--------|---------|
| Sales | ✅ Full | Process transactions only |
| Products | ✅ View | View product list only |
| Customers | ⚠️ Limited | View only (Admin creates) |
| Reports | ❌ No | Cannot view |
| Stock Manager | ❌ No | Cannot access |
| Shifts | ✅ Required | MUST open shift first |
| Bills | ❌ No | Cannot access |
| Barcode | ❌ No | Cannot access |
| Users | ❌ No | Cannot access |
| Settings | ❌ No | Cannot access |

**Restrictions**:
- ❌ **CANNOT SELL** without opening a shift first
- ❌ Cannot access product editing
- ❌ Cannot view reports
- ❌ Cannot manage inventory
- ✅ Can only see their own shift sales

**Best Practice**: One cashier per shift

---

#### 3. **MANAGER** (Reporting & Control)
Mid-level access for business operations oversight

| Feature | Access | Details |
|---------|--------|---------|
| Sales | ✅ View | View sales only |
| Products | ✅ Full | Manage products |
| Customers | ✅ Full | Manage customer data |
| Reports | ✅ Full | View all reports |
| Stock Manager | ✅ Full | Full inventory control |
| Shifts | ✅ Full | Manage all shifts |
| Bills | ✅ Full | Manage bills |
| Barcode | ❌ No | Cannot manage |
| Users | ❌ No | Cannot manage users |
| Settings | ⚠️ Limited | View only, no changes |

**Can Do**:
- ✅ Analyze business performance via reports
- ✅ Manage inventory and stock levels
- ✅ Create/edit products and categories
- ✅ Manage customer information
- ✅ Monitor cashier shifts

---

#### 4. **INVENTORY MANAGER** (Stock Only)
Specialized role for inventory and stock management

| Feature | Access | Details |
|---------|--------|---------|
| Sales | ❌ No | Cannot access |
| Products | ✅ Full | Manage products |
| Customers | ❌ No | Cannot access |
| Reports | ⚠️ Stock Only | Stock reports only |
| Stock Manager | ✅ Full | Full inventory control |
| Shifts | ❌ No | Cannot access |
| Bills | ❌ No | Cannot access |
| Barcode | ✅ Full | Create/print barcodes |
| Users | ❌ No | Cannot manage users |
| Settings | ❌ No | Cannot access |

**Ideal For**:
- Warehouse managers
- Stock takers
- Inventory auditors

---

### Creating & Managing Users

**Only ADMIN can manage users**

#### Add New User:
1. Click **Settings** ⚙️
2. Go to **User Roles & Permissions** tab
3. Click **Add New User**
4. Fill in:
   - **Username**: Unique identifier
   - **Password**: Strong password (min 8 chars recommended)
   - **Display Name**: Full name for welcome messages
   - **Role**: Select Admin/Cashier/Manager/Inventory Manager
   - **Email**: For notifications (optional)
5. Click **Create User**

#### Modify User:
1. In **User Roles & Permissions** tab
2. Find user in list
3. Click **Edit**
4. Change details
5. Click **Save**

#### Delete User:
1. Select user
2. Click **Delete**
3. Confirm deletion (⚠️ Cannot undo)

#### Change User Password:
- User can change their own: Settings → Password → Enter old & new password
- Admin can reset: User Roles tab → Select user → Reset Password

---

## 🔧 Troubleshooting

### Application Won't Start

**Problem**: YONT_POS.exe won't launch

**Solution**:
1. Check if already running (Ctrl+Shift+Esc → Task Manager → Search "main.exe")
2. Kill any existing process
3. Delete: `C:\YONT_POS\*.ldb` (lock files)
4. Restart application

### Installation Failed Error

**Problem**: "Cannot write to directory" or "Access Denied"

**Solution**:
1. ✅ Verify installation in `C:\YONT_POS` (not Program Files)
2. Right-click folder → Properties → Security → Give Full Control
3. Run installer again

### Database Errors on Startup

**Problem**: "Database file not found" or "Database locked"

**Solution**:
1. Ensure `pos_system.db` exists in `C:\YONT_POS`
2. Delete any `.db-shm` or `.db-wal` files
3. Restart application
4. If corrupted:
   - Restore from backup in `C:\YONT_POS\backups`
   - Or reinstall application

### Login Issues

**Problem**: Cannot login with default credentials

**Solution**:
1. Reset database: Settings → Advanced → Clear POS Data
2. Restart
3. Try default credentials again (admin/admin123)

### Reports Not Showing Data

**Problem**: Reports are blank or showing "No Data"

**Solution**:
1. Verify sales have been recorded
2. Check date range is correct
3. Ensure user has "Reports" permission
4. Try different date range

### Printer Not Printing Receipts

**Problem**: Receipts not printing or buttons grayed out

**Solution**:
1. Check printer is powered and connected
2. Settings → Printer Settings → Select correct printer
3. Test print function
4. Ensure printer drivers are installed
5. For thermal printers: Check ESC/POS compatibility

### Email Receipts Not Sending

**Problem**: "Failed to send email" error

**Solution**:
1. Settings → Email Settings → Check Gmail account is configured
2. Verify customer has email address in profile
3. Check internet connection
4. Test Send → Email Settings tab
5. Enable "Less Secure Apps" if using Gmail
6. Use App Password (not regular Gmail password)

### Slow Performance

**Problem**: Application lags or freezes

**Solution**:
1. Close other programs (reduce RAM usage)
2. Settings → Advanced → Optimize Database
3. Clear logs: Settings → Advanced → Clear application data
4. Restart application
5. Upgrade RAM if running many programs

### Accidental Data Loss

**Problem**: Deleted products/sales by mistake

**Solution**:
1. Check if backup exists: `C:\YONT_POS\backups`
2. Contact Administrator to restore backup
3. **Prevention**: Always verify before deleting
4. Enable: Settings → Advanced → Auto-backup (every day)

---

## 📞 Support & Updates

### Technical Support

**For Issues**:
1. Check error.log file: `C:\YONT_POS\error.log`
2. Contact system administrator with:
   - Error message text
   - Steps that caused the error
   - Screenshot of error
   - Contents of error.log file

### Backup Your Data

**IMPORTANT: Backup Data Regularly**

#### Manual Backup:
1. Settings → Advanced → **Backup Now**
2. Saves to: `C:\YONT_POS\backups\`
3. Keep multiple backups (weekly recommended)

#### Automatic Backup:
1. Settings → Advanced
2. Enable: "Auto Backup"
3. Set frequency: Daily/Weekly
4. Backups auto-save to: `C:\YONT_POS\backups\`

#### Restore from Backup:
1. Settings → Advanced → **Restore from Backup**
2. Select backup file
3. Confirm restoration (⚠️ Will overwrite current data)
4. Application will restart

### Checking System Information

**To view system info and version**:

Status Bar (bottom of screen):
- Shows current language
- Connection status
- Ready status

Menu Bar:
- Version info in About section (if available)

---

## 🎯 Quick Reference: Common Tasks

### Complete Sales Transaction
1. Click **Sales**
2. Search customer (or create new)
3. Scan or select products
4. Adjust quantities
5. Apply discount (if needed)
6. Complete payment
7. Print/Email receipt

### Add New Product
1. Click **Products**
2. Click **Add New**
3. Enter: Name, Price, Category, Stock
4. Add image (optional)
5. Click **Save**

### Open Shift (Cashier)
1. Click **Shift**
2. Click **Open Shift**
3. Enter starting cash amount
4. Confirm

### Close Shift
1. Click **Shift**
2. Click **Close Shift**
3. Enter ending cash amount
4. Review discrepancy
5. Confirm

### Generate Report
1. Click **Reports**
2. Select report type
3. Choose date range
4. Click **Generate**
5. Export as needed

### Change Password
1. Click **Settings** ⚙️
2. Go to **Password** tab
3. Enter old password
4. Enter new password twice
5. Click **Save**

### Change Language
1. Click **Settings** ⚙️
2. Go to **Language** tab
3. Select: English / ဆန် (Shan) / မြန်မာ (Myanmar)
4. Click **Apply**
5. Interface changes immediately

---

## 📝 Notes & Best Practices

### Security Tips
- ✅ Change default admin password immediately
- ✅ Use strong passwords (8+ characters, mixed case, numbers)
- ✅ Log out when leaving workstation
- ✅ Restrict admin account to designated staff
- ✅ Regular backups prevent data loss
- ✅ Keep Windows and drivers updated

### Daily Operations
- ✅ Cashiers open shift at start of day
- ✅ Process sales normally
- ✅ Close shift at end of day
- ✅ Store manager reviews daily reports
- ✅ Backup data weekly (minimum)

### Inventory Management
- ✅ Add stock when items received
- ✅ Remove stock for damage/expires
- ✅ Reconcile stock counts monthly
- ✅ Set low-stock alerts in Products
- ✅ Use Barcode Manager for quick scanning

### Troubleshooting First Steps
1. Check **error.log** file for clues
2. Restart the application
3. Check database backup status
4. Verify user permissions
5. Contact system administrator

---

## 🚀 Getting Help

**For detailed questions or issues**:
- Check menu in-application help
- Review error.log file: `C:\YONT_POS\error.log`
- Contact your system administrator
- Document any error messages with screenshots

---

**YONT POS v1.0.0 © 2024 YONT POS TEAM**

*Last Updated: February 2026*

**Installation Path**: `C:\YONT_POS`  
**Data Path**: `C:\YONT_POS\`  
**Backups**: `C:\YONT_POS\backups\`  
**Logs**: `C:\YONT_POS\logs\`
