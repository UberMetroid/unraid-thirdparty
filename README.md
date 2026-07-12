# Unraid Third-Party Application Templates

This repository hosts community-maintained Docker XML templates for third-party servers and applications optimized for Unraid.

---

## 🚀 How to Add This Repository to Unraid

To use these templates on your Unraid server:

1. Copy the repository URL:
   ```text
   https://github.com/UberMetroid/unraid-thirdparty
   ```
2. Navigate to your Unraid WebGUI.
3. Go to the **Apps** tab (Community Applications).
4. Click on **Repositories** in the left sidebar or at the top.
5. Paste the URL into the repository input field and add it.

Once added, the applications below will appear in your Community Applications search results.

---

## 📦 Available Templates

| Application | Description | Category | Port Mapping (Host:Container) | Default Storage Path | Template XML |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **[OpenRepo](https://github.com/openkilt/openrepo)** | A lightweight package repository server hosting Debian (`.deb`), RedHat (`.rpm`), and generic files. Consolidates Nginx, Django, and Celery. | Tools, Backup, Web | `7376:8080` (Web UI) | `/mnt/user/appdata/openrepo` | [openrepo.xml](templates/openrepo.xml) |
| **[Gitea](https://github.com/go-gitea/gitea)** | A painless self-hosted Git service written in Go. A lightweight, resource-friendly community fork of Gogs. | Developer, Productivity | `3000:3000` (Web UI)<br>`2222:22` (SSH) | `/mnt/user/appdata/gitea` | [gitea.xml](templates/gitea.xml) |

---

## 🤝 Support & Contributions

If you encounter issues or want to submit updates to these templates, please open an issue or pull request.

- **Issues**: [GitHub Issues](https://github.com/UberMetroid/unraid-thirdparty/issues)
- **Pull Requests**: [GitHub Pull Requests](https://github.com/UberMetroid/unraid-thirdparty/pulls)

---

## 📄 License

This repository is licensed under the [MIT License](LICENSE).
