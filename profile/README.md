# **OroBundle – OroCommerce Extensions Repository**

OroBundle stores reusable extensions and integration bundles for **OroCommerce** and **OroPlatform**.

This organization hosts open-source, versioned, Composer-installable packages that expand or enhance the capabilities of the OroCommerce core application and are available to Oro implementation **partners** and Oro **customers**.

**How to get access:** Request access to a specific extension via our Support portal\
**Extensions Catalog:** [https://extensions.oroinc.com](https://extensions.oroinc.com)\
**OroCommerce Documentation:** [https://doc.oroinc.com](https://doc.oroinc.com)\
**OroCommerce Repo:** [https://github.com/oroinc](https://github.com/oroinc)

---

## **What You’ll Find Here**

### **OroCommerce Extensions**

Feature modules are packaged as bundles with migrations, UI components, configuration, jobs, and integrations.

All repositories under the *OroBundle* organization are provided **AS-IS**, without SLA, warranty, or guaranteed feature roadmap.
For commercial support, please use your **Oro Support contract** or partner channel.

---

## **Installing Extensions**

Most bundles can be added to any OroCommerce project via Composer:

```bash
composer require vendor/bundle-name
```

After installation, apply migrations and clear the cache:

```bash
php bin/console cache:clear --env=prod
php bin/console oro:migration:load --force --env=prod
```

Some bundles may require:

* Search reindexing
* Message Queue consumers
* Additional configuration
* Asset build steps

Always check the bundle’s **README** for exact installation instructions.

---

## **Versioning & Compatibility**

Each extension follows **Semantic Versioning**:

```
MAJOR.MINOR.PATCH → v1.2.3
```

### **Branches**

* `main` → development for the next compatible OroCommerce minor
* `maintenance/X.Y` → stable line compatible with OroCommerce **X.Y**

### **Tags**

* `vX.Y.Z` → release built for OroCommerce X.Y

Composer constraints in `composer.json` define platform compatibility.
Check each repository’s README for its detailed **compatibility matrix**.

---

## **Reporting Issues**

Follow `CONTRIBUTING.md` and `SECURITY.md` guidelines.

---

## **Contributing to OroBundle**

We welcome contributions.
Follow `CONTRIBUTING.md` for contribution rules, code style, branching, and testing.

---

## **Governance & Support**

* **License:** OSL-3.0 for all repositories unless stated otherwise
* **Maintainers:** Oro engineering
* **Support posture:** AS-IS, no warranty, no SLA
* **Community support:** via GitHub Issues (best-effort basis)

If you are an Oro partner and want to maintain or publish an extension here, contact your **Oro Partner Manager**.

---

## **Stay Connected**

* **OroCommerce Website:** [https://oroinc.com/b2b-ecommerce](https://oroinc.com/b2b-ecommerce)
* **Partner Program:** [https://oroinc.com/partners](https://oroinc.com/partners)
* **Documentation:** [https://doc.oroinc.com](https://doc.oroinc.com)
* **Extensions Catalog:** [https://extensions.oroinc.com](https://extensions.oroinc.com)
