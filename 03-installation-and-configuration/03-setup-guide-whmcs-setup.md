# Setup guide: WHMCS setup

## System requirements

The module is encoded with ionCube.

| Requirement | Minimum |
|-------------|---------|
| PHP | 8.2 or higher |
| WHMCS | 9.x or higher |
| ionCube Loader | v13 or newer (v14, v15) |

### Older module versions for WHMCS 8

- PHP 7.4: [https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-MinIO-S3/php74/](https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-MinIO-S3/php74/)
- PHP 8.1: [https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-MinIO-S3/php81/](https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-MinIO-S3/php81/)

> To install and update a module, you must perform one and the same action.

---

## Step 1 — Download

```bash
wget http://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-MinIO-S3/php82/PUQ_WHMCS-MinIO-S3-latest.zip
```

All versions available via: [http://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-MinIO-S3/](http://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-MinIO-S3/)

---

## Step 2 — Extract

```bash
unzip PUQ_WHMCS-MinIO-S3-latest.zip
```

---

## Step 3 — Deploy

Copy and replace the `puqMinIOS3` directory from `PUQ_WHMCS-MinIO-S3` to `WHMCS_WEB_DIR/modules/servers/`

---

## Step 4 — Server Configuration

Create a new MinIO S3 server in WHMCS:

Navigate to: **System Settings → Products/Services → Servers**

1. Click **Add New Server**
2. Enter the correct **Name** and **Hostname**
3. In the **Server Details** section, select the **PUQ MinIO S3** module and enter the correct username and password for the MinIO web interface
4. Click the **Test connection** button to verify

![Add server - General settings](../img/05-add-server-1.png)

![Add server - Module settings](../img/06-add-server-2.png)

---

## Step 5 — Create Product

Navigate to: **System Settings → Products/Services → Create a New Product**

In the **Module Settings** section, select the **PUQ MinIO S3** module and configure the product options.

![WHMCS setup](../img/05-add-server-1.png)
