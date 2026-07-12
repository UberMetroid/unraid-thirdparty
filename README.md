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

## 📦 Included Applications

| Application | Description | Category | Template |
| :--- | :--- | :--- | :--- |
| **[OpenRepo](https://github.com/openkilt/openrepo)** | A lightweight package repository server hosting Debian (`.deb`), RedHat (`.rpm`), and generic files. Consolidates Nginx, Django, and Celery into a single-container design. | Tools, Backup, Web | [Template](templates/openrepo.xml) |
| **[Gitea](https://github.com/go-gitea/gitea)** | A painless self-hosted Git service written in Go. A lightweight, resource-friendly community fork of Gogs. | Developer, Productivity | [Template](templates/gitea.xml) |

---

## 🛠️ Configuration Details

### OpenRepo
- **Port mapping**: External port `7376` maps to internal port `8080`.
- **Secret Key**: Requires a secure custom secret key (`DJANGO_SECRET_KEY`) for Django sessions.
- **Storage**: Maps application data (including SQLite DB and package storage) to `/mnt/user/appdata/openrepo`.

### Gitea
- **Port mapping**: Web interface defaults to port `3000`. SSH operations map to host port `2222`.
- **Permissions**: Runs under Unraid's default `nobody:users` (UID `99`, GID `100`) to avoid filesystem permission conflicts.

---

## 🤝 Support & Contributions

If you encounter issues or want to submit updates to these templates, please open an issue or pull request in this repository.

- **Issues**: [GitHub Issues](https://github.com/UberMetroid/unraid-thirdparty/issues)
- **Pull Requests**: [GitHub Pull Requests](https://github.com/UberMetroid/unraid-thirdparty/pulls)

---

## 📄 License

This repository is licensed under the [MIT License](LICENSE).
