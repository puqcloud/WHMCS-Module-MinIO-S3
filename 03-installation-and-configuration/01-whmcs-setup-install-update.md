# WHMCS setup (install/update)

## System requirements

The module uses ionCube encoding. Your server must meet the following requirements:

| Requirement | Minimum |
|-------------|---------|
| PHP | 8.2 or higher |
| WHMCS | 9.x or higher |
| ionCube Loader | v13 or newer (v14, v15) |

### Older module versions for WHMCS 8

Older versions of the module are available for download, sorted by PHP version:

- PHP 7.4: [https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-MinIO-S3/php74/](https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-MinIO-S3/php74/)
- PHP 8.1: [https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-MinIO-S3/php81/](https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-MinIO-S3/php81/)

---

## Step 1 — Download the latest version of the module

```bash
wget http://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-MinIO-S3/php82/PUQ_WHMCS-MinIO-S3-latest.zip
```

All versions of the module are available via the link: [http://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-MinIO-S3/](http://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-MinIO-S3/)

---

## Step 2 — Unzip the archive with the module

```bash
unzip PUQ_WHMCS-MinIO-S3-latest.zip
```

---

## Step 3 — Copy and Replace

Copy the `puqMinIOS3` directory from the extracted `PUQ_WHMCS-MinIO-S3` archive to your WHMCS installation:

```
WHMCS_WEB_DIR/modules/servers/
```

> **Note:** To install and update a module, you must perform one and the same action — download and copy the latest version over the existing files.
